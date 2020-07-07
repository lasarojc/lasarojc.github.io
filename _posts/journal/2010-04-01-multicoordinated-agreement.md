---
layout: post
categories:
 - Publications

title: Multicoordinated agreement for groups of agents
author: Lasaro Camargos, Rodrigo Schmidt, Edmundo R. M. Madeira, Fernando Pedone
venue: Journal of the Brazilian Computer Society
paper: https://journal-bcs.springeropen.com/articles/10.1007/s13173-010-0001-7
type: Journal


---
Abstract: Agents in agreement protocols play well distinct roles. Proposers propose values to the acceptors, which will accept proposals and inform the learners so they detect that an agreement has been reached. A fourth role is that of the coordinator, who filters the proposals from proposers to acceptors. While proposers, learners, and coordinators are easily replaced, substituting an acceptor is prohibitive. Protocols that do not employ a coordinator are less resilient to acceptor failures. Protocols that use one coordinator are more resilient to acceptor failures, at the expense of one extra communication step even in the absence of failures. Moreover, they require replacing the coordinator as soon as it fails, a reconfiguration that, although relatively inexpensive, diminishes the protocol availability. Hence, either option, i.e, one or zero coordinator, has its drawbacks. In previous works, we have presented an alternative: multicoordinated agreement protocols. Such protocols are as resilient as single-coordinated protocols but require less reconfiguration to cope with coordinator failures. In fact, most reconfiguration can be done in parallel to the execution of the protocol's normal steps. Multicoordination can be applied to several problems. In this paper we exemplify its use in solving consensus and then introduce a fast multicoordinated agreement protocol for agents organized in groups, an abstraction for fast local area networks interconnected by slower links.
