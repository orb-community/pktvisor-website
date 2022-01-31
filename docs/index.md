---
hide:
- navigation
- toc
- tags
---

<h1></h1>
<img src="img/pktvisor-header.png" alt="Orb" width="400"/>
<img src="img/pktvisor-diagram.png" alt="Orb" width="500"/>

# Open-source observability agent

[Get Started with pktvisor](install/)

***

## What is pktvisor?



**pktvisor** (pronounced "packet visor") is an **observability agent** for _summarizing_ high volume, information-dense data streams down to lightweight, immediately actionable observability data directly at the edge. Its goal is to extract the signal from the noise, separating the needles from the haystacks as close to the source as possible.

It is a resource-efficient, side-car style agent built from the ground up to be modular and dynamically controlled in real time via API. Input and processor modules may be dynamically loaded at runtime. Metric output can be visualized both on-node via command-line UI (for a localized, hyper real-time view) as well as centrally collected into industry standard observability stacks like Prometheus and Grafana.

The [input stream system](src/inputs) is designed to _tap into_ data streams—currently on [packet capture](https://en.wikipedia.org/wiki/Packet_analyzer) and [dnstap](https://dnstap.info/) with forthcoming support for [sFlow](https://en.wikipedia.org/wiki/SFlow) / [Netflow](https://en.wikipedia.org/wiki/NetFlow), [envoy taps](https://www.envoyproxy.io/docs/envoy/latest/operations/traffic_tapping), and [eBPF](https://ebpf.io/).

The [stream processor system](src/handlers) includes full application-level analysis and [efficiently](https://en.wikipedia.org/wiki/Streaming_algorithm) summarizes to one-minute buckets of:

* Counters
* Histograms and Quantiles
* Timers and Rates
* Heavy Hitters/Frequent Items/Top N
* Set Cardinality
* GeoIP

These screenshots display both the [command line](golang/) and [centralized views](centralized_collection/) of
the [Network](src/handlers/net) and [DNS](src/handlers/dns) stream processors, and the types of summary information provided:

![Image 1 of Grafana Dash](https://raw.githubusercontent.com/ns1labs/pktvisor/develop/docs/images/pktvisor-grafana-screenshot1.png)
![Image of CLI UI](https://raw.githubusercontent.com/ns1labs/pktvisor/develop/docs/images/pktvisor3-cli-ui-screenshot.png)
![Image 2 of Grafana Dash](https://raw.githubusercontent.com/ns1labs/pktvisor/develop/docs/images/pktvisor-grafana-screenshot2.png)
