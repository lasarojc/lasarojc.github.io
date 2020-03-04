---
layout: post
categories:
 - Publications

title: Analysis of Monitoring and Multipath Support on top of OpenFlow Specification 
author: Pedro Rezende, Paulo R. S. L. Coelho, Luiz F. Faina, Lasaro Camargos, Rafael Pasquini
venue: International Journal of Network Management
paper: https://onlinelibrary.wiley.com/doi/abs/10.1002/nem.2017
type: journal


---
Abstract: In general, traffic is pushed through a single path despite the existence of alternative paths in networks. For example, routing solutions based on spanning tree prune the topology to prevent loops, consequently preventing also the use of alternative paths. Research on quality of service frequently advocates that the use of alternative paths is interesting for enforcing Service Level Agreements (SLAs), bypassing bottlenecks created by shortest paths. In this paper, we are interested in analyzing the support for monitoring network traffic and for provisioning of multipaths in software‐defined networking (SDN), given the strong platform it provides for experimentation of new networked solutions. Our approach firstly enriches the topology view at the control plane with data gathered through fine grain data plane monitoring. On the basis of such enriched view, our system determines the path, or multipaths, necessary to enforce the specified SLA. We propose 2 extension modules to an OpenFlow controller: SDNMon, which monitors the data plane to enrich the topology information at the control plane, and MP‐Routing, which determines a set of paths, in the absence of a single path capable of enforcing the SLA. Both modules are extensively evaluated, and the results not only demonstrate what can be achieved in terms of accuracy in SDNMon and in terms of quality of service benefits in MP‐Routing but also highlight some limitations of OpenFlow specification. On the basis of our findings, we propose a set of new counters to Per Port and Per Flow granularity levels of OpenFlow specification.

