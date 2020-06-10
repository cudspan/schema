---
layout: default
title: Hello World
---

This tutorial walks your through a Hello World project. This is the 
simplese project you can deploy to show end-to-end functioning of 
the Data Ingestion Framework (DIF). 

The DIF is the pairing of a specific data format with a 
{{ site.data.vars.Product_Short }} probe. 
This probe can get the data and use it to add entities or metric values to the 
{{ site.data.vars.Product_Short }} supply chain. In this tutorial you will:

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
* Validate your data against the JSON schema
* Deploy your data to the DIF data server
* Configure your DIF data server as a target in {{ site.data.vars.Product_Short }}

# Step 1: Deploy a DIF Data Server

A DIF data server is simply an HTTP or HTTPS server that can return a JSON string on 
request.  The request must be a static URL that {{ site.data.vars.Product_Short }} 
can use to GET this data at regular intervals. Just make sure the URL endpoint 
returns your JSON data.

For this tutorial, the JSON data is static, so you can serve it up from any web server 
that you {{ site.data.vars.Product_Short }} can access. For example, assume you have 
a web server at `MyDomain.com`. If you deploy your DIF data to `dif/myTopology.json`, 
the the URL `http"//www.MyDomain.com/dif/myTopology.json` should return your JSON string.

Note that the DIF data server domain should be a static address. In a real-world 
deployment, the static address ensures the same data server is available 
for the long term.

# Step 2: Create the JSON Data

For this tutorial you will create a single Business Application entity. This 
entity 

    {
      "version": "v1",
      "updateTime": 123,
      "scope": "",
      "source": "",
      "topology" : [
        {
          "uniqueId": "Hello_World",
          "type": "businessApplication",
          "name": "Tutorial",
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


