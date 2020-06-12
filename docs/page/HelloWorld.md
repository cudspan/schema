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
* Deploy your data to the DIF data server
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
created, create a file named HelloWorld.json, and give it the following content. 

    {
      "version": "v1",
      "updateTime": 123,
      "scope": "",
      "source": "",
      "topology" : [
        {
          "uniqueId": "Hello_World_BusinessApp",
          "type": "businessApplication",
          "name": "Hello World Tutorial",
          "metrics": {
            "kpi": [
              {
                "average": 1234,
                "capacity": 2345,
                "key": "Total Tickets"
              }
            ]
          }
        }
      ]
    }

A brief description of the data is in order. The data object begins with 
typical initial information such as version, time of latest update, and 
other descriptors. For complete descriptions, see the the following 
Schema Object description, [Topology Object](Topology.html).

{% if site.github.pages_hostname == "github.io" %}
[Topology Object](Topology.html)
<a href="{{ site.github.baseurl }}{{ 'page/Topology.html' | relative_url }}">Topology Object</a>
{% else %}
<a href="{{ 'page/Topology.html' | absolute_url }}">Topology Object</a>
{% endif %}


{% if site.github.pages_hostname == "github.io" %}
<a href="{{ site.github.baseurl }}{{ 'page/Topology.html' | relative_url }}">Topology Object</a>
{% else %}
<a href="{{ 'page/Topology.html' | absolute_url }}">Topology Object</a>
{% endif %}


