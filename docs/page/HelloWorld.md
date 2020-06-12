---
layout: default
title: Hello World
---

This tutorial walks your through a Hello World project. This is the 
simplest project you can deploy to show end-to-end functioning of 
the Data Ingestion Framework (DIF). 

The DIF is the pairing of a specific data format with a 
{{ site.data.vars.Product_Short }} probe. You deploy a DIF data server 
and configure it as a {{ site.data.vars.Product_Short }} via the DIF probe. 
This probe gets the data your target delivers, and uses it to add entities or metric 
values to the {{ site.data.vars.Product_Short }} supply chain. 

This tutorial shows you how to put this all together, to prove 
that you have a valid development environment. You will:

<!--
<ul>
<li><p>Deploy a server that can serve up a JSON string over HTTP or HTTPS</p>
<p>This will be your your DIF data server.  It can reside on any network that 
your {{ site.data.vars.Product_Short }} 
instance can access. You can even deploy the server on your 
{{ site.data.vars.Product_Short }} instance.</p>
</li>
<li><p>Create the data to add a single entity to the {{ site.data.vars.Product_Short }} 
topology</p>
<p>The data format is a JSON string that complies with the JSON Schema we have included 
as part of the DIF. You will create the data to define a Buiness Application 
entity that is named "Hello World".</p>
</li>
<li><p>Validate your data against the JSON schema</p>
<p>As you develop the data you want to load into {{ site.data.vars.Product_Short }}, 
you should use a JSON Schema validator to make sure your data complies with the schema.
</li>
<li><p>Configure your DIF data server as a target in {{ site.data.vars.Product_Short }}</p>
<p>To configure the target, you simply specify the URL to your server that 
will return the JSON string via a <code>GET</code> method. </p>
</li>
</ul>
-->
* Deploy a server that can serve up a JSON string over HTTP or HTTPS
* Create the data to add a single entity to the {{ site.data.vars.Product_Short }}  topology
* Validate your data against the DIF JSON schema
* Configure your DIF data server as a target in {{ site.data.vars.Product_Short }}

# Step 1: Deploy a DIF Data Server

A DIF data server is simply an HTTP or HTTPS server that can return a JSON string on 
request.  The request must be a static URL that {{ site.data.vars.Product_Short }} 
can use to GET this data at regular intervals. Just make sure the URL endpoint 
returns your JSON data.

For this tutorial, the JSON data is static, so you can serve it up from any web server 
that your {{ site.data.vars.Product_Short }} installation can access. This tutorial 
assumes you already have a web server on your network that you can use.  
You must be able to create a new directory on that server, and upload a 
JSON file to it.

For this tutorial, we will assume your web server is on the domain, `MyDomain.com`, 
we assume your {{ site.data.vars.Product_Short }} can reach it either directly or 
through a proxy.

Go into the server and create the directory, `www/dif/`. Your server will serve up 
the JSON data from here.

Note that the DIF data server domain should be a static address. In a real-world 
deployment, the static address ensures the same data server is available 
for the long term.

> **NOTE:** If you don't have a web server handy, you can use the sample node.js 
> that we include in the examples repository.  You can deploy that on any machine in 
> your network that has node installed. You can even install node on your 
> {{ site.data.vars.Product_Short }} machine, and deploy the server there.

# Step 2: Create the JSON Data

For this tutorial you will create a topology with a single Business Application entity. 
This entity will have the name "Hello World Tutorial".  In the `www/dif/` directory you 
created, create a file named `HelloWorld.json`, and give it the following content. 

    {
      "version": "v1",
      "updateTime": 123,
      "scope": "",
      "source": "",
      "topology" : [
        {
          "uniqueId": "Hello_World_BusinessApp",
          "type": "businessApplication",
          "name": "Hello World Tutorial"
        }
      ]
    }

A brief description of the data is in order. The data object begins with 
typical initial information such as version, time of latest update, and 
other descriptors. For complete descriptions, see the the following 
Schema Object description for [Topology Object](Topology.html). 

For these initializing fields, the most important is `updateTime`. 
In a real-world use case, you would 
periodically update your topology data to capture changes in your environment. 
As you do, you should post the update time here. This could be useful for debugging 
in case your management process stops updating the data. For this tutorial, any 
arbitrary integer will do.

The topology itself is an array of entities.  Each entity  must include the following 
fields:

* `uniqueId`: 
    
    This identifies the entity among all the instances of that 
    entity type in your topology. Because the ID must be globally unique, you 
    should use naming conventions that express your namespace for this topology 
    segment that you're creating.
    
* `type`:
    
    The type of entity you are creating. For this tutorial we are creating a 
    a Business Application. DIF currently supports:
    - `businessApplication`
    - `businessTransaction`
    - `service`
    - `databaseServer`
    - `application`

* `name`:

    The display name for the entity. This does not have to be unique, but it is usually 
    convenient to give unique display names.

An entity can include other properties, such as metrics to show utilization of capacity, 
or relationships to other entities to stitch it into the 
{{ site.data.vars.Product_Short }} supply chain.

After you save the file, your DIF data server should be able to serve up the JSON data. 
To test it, use the following command, assuming your own domain, and assuming you 
named the file  `HelloWorld.json`:

`curl MyDomain.com/dif/HelloWorld.json`

The curl output should mirror the data you saved to the file.

# Step 3: Validate Your JSON Data

Your DIF data server is now able to serve a topology to {{ site.data.vars.Product_Short }}. 
But before you do that, you should validate the data to make sure it complies with 
the JSON schema.  As you develop JSON constructs, it is a good idea to validate your 
work. This can save you time, and can avoid problems where you don't get 
the results you expect.

There are many validators implemented against JSON Schema draft 7. You can even 
deploy them in your data process to make sure yoo always generate valid data. 
For this tutorial we will use an online validator at:

<a href="https://www.jsonschemavalidator.net/" target="blank">https://www.jsonschemavalidator.net/</a>

Copy the DIF schema from **FICTION ALERT: NEED SCHEMA LOCATION** to the clipboard. 
Then navigate to the validator and pase the schema in the left-hand panel. Then 
copy the contents of your JSON file and paste it into the right-hand panel. 
You should see no errors.

{% if site.github.pages_hostname == "github.io" %}
<img src="{{ site.github.baseurl }}{{ '/assets/HelloWorld_Validate.gif' | relative_url }}" alt="Validation">
{% else %}
<img src="{{ '/assets/HelloWorld_Validate.gif' | relative_url }}" alt="Validation">
{% endif %}


**FICTION ALERT: THIS ASSUMES THE SCHEMA IS IN A SINGLE FILE. I SPOKE WITH PALLAVI ABOUT THAT.**

# Step 4: Configure the DIF Data Server as a {{ site.data.vars.Product_Short }} Target

Now that you have:

1. A web server with a `dif` directory
2. A DIF data file named `HelloWorld.json` in that directory
3. Validated the DIF data

You can set up the DIF data server as a target. 

Go to your {{ site.data.vars.Product_Short }} user interface, and navigate to 
**SETTINGS > Target Configuration**. From there, click **NEW TARGET** and choose 
the **Custom** target category. Within that category, click the 
**Data Ingestion Framework** target type.

Target configuration requires two fields -- The URL to your DIF data (the 
JSON file you created), and a name for the target.  Assuming you set up your 
web server according to the tutorial steps, you can give the following values:

* URL: `http://MyDomain.com/dif/HelloWorld.json`
* NAME: `Tutorial_Metric_Server`

To finish the configuration, click **ADD**.

If all goes well, {{ site.data.vars.Product_Short }} displays the 
Target Configuration page, and you should see the Tutorial_Metric_Server target 
in the list. It should be green, which means it successfully validated.  

If the target did not validate, make sure that the URL you specified actually 
returns the JSON data. Also, you should ensure that the data is valid 
for the DIF JSON schema.

{{ site.data.vars.Product_Short }} requests data from targets at 10-minute intervals. 
Assuming your target validated, then within about 10 minutes you should see your 
entity in the {{ site.data.vars.Product_Short }} supply chain. In 
{{ site.data.vars.Product_Short }}, navigate to **SEARCH** and select 
**Business Applications**. In the Search field, type `Hello` -- The 
Hello World Tutorial entity should appear in the list. Click on that entry, 
and you should see the entity in the Supply Chain.

{% if site.github.pages_hostname == "github.io" %}
<img src="{{ site.github.baseurl }}{{ '/assets/HelloWorld1_SupplyChain.gif' | relative_url }}" alt="The Supply Chain">
{% else %}
<img src="{{ '/assets/HelloWorld1_SupplyChain.gif' | relative_url }}" alt="The Supply Chain">
{% endif %}


# Wrap Up

This is the simplest possible use of the DIF to load an entity into the 
{{ site.data.vars.Product_Short }} via a custom target. If you got this far, 
you know that you can produce DIF data and validate it. You know that you 
can deploy a DIF data server, and use it to serve up the DIF data. And you 
know that you can configure the data server as target.

For a real-world use case, you will want to create a fuller topology, and 
stitch it in with the rest of your environment. You will also want to track 
utilization of resources, and expose them as metrics in the DIF data.  For 
resources that {{ site.data.vars.Product_Short }} supports natively, these 
metrics contribute to analysis, and your custom entities can participate in 
{{ site.data.vars.Product_Short }} actions and application management.





