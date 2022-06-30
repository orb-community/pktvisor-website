---
hide:
- navigation
- toc
- tags
---

<h1></h1>
<img src="img/pktvisor-header.png" alt="pktvisor" width="400"/>
![pktvisor Overview](img/pktvisor-diagram.png){ align=right width="500" }

# Open source, network observability agent for analysis at the edge

[Get Started with pktvisor](install/){ .md-button .md-button--primary }


***

## What is pktvisor?
**pktvisor** (pronounced "packet visor") is an **observability agent** for analyzing high volume, information dense network data streams and extracting actionable insights **directly from the edge**.

## How is pktvisor different?
It is a resource-efficient agent built from the ground up to be **modular**, **dynamically controlled in real time** and produce **"small data"** metric and log output. 

## Why pktvisor?
Metric output can be visualized and actioned **on-node** as well as **centrally collected** into modern observability stacks.

## What questions does pktvisor answer?
pktvisor uses <a href="https://en.wikipedia.org/wiki/Streaming_algorithm">streaming algorithms</a> to **analyze in real time**, providing metrics which let you answer questions such as:

 * What are the rates and frequent items across common network traffic dimensions?
 * How many unique IP addresses (cardinality) have we seen in the last minute?
 * What are the percentiles of DNS transaction times? 
 * What is the histogram of response payload sizes?
 * What is still querying that DNS record that was deleted?
 * From what ASN and Geo regions is traffic coming?
 * Is this traffic spike malicious or legitimate? Is this a random label attack? Is it widely distributed? IPv4? UDP? 

## How can I centrally control and collect pktvisor metrics?
Although pktvisor can be used stand-alone, it is designed to be run at scale as part of the <a href="https://orb.community"><img src="img/ORB-logo-black@3x.png" alt="pktvisor" width="100"/></a>
<a href="https://orb.community">Observability Platform</a>.
***

# Backed by NS1
**pktvisor** was born at [NS1 Labs](https://ns1.com/labs), where we're
committed to making [open source, dynamic edge observability a reality](https://ns1.com/blog/orb-a-new-paradigm-for-dynamic-edge-observability).

