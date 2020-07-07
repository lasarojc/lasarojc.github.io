---
layout: post
categories:
 - Publications

title: On the Impossibility of Byzantine Collision-Fast Atomic Broadcast
author: Rodrigo Saramago, Tuanir França Rezende, Eduardo Adílio Pelinson Alchieri, Lasaro Camargos
venue: The 32nd IEEE International Conference on Advanced Information Networking and Applications (IEEE AINA-2018), Krakow, Poland 
paper: https://www.researchgate.net/publication/325264988_On_the_Impossibility_of_Byzantine_Collision-Fast_Atomic_Broadcast
type: Peer-reviewed Conference


---

Abstract: The inefficiency of Consensus-based Atomic Broadcast protocols in the presence of collisions (concurrent proposals) harms their adoption in the implementation of State Machine Replication. Proposals that are not decided in some instance of Consensus (commands not delivered) must be re-proposed in a new instance, delaying their execution. The CFABCast (Collision-Fast Atomic Broadcast) algorithm uses M-Consensus to decide and deliver multiple values in the same instance. However, CFABCast is not Byzantine fault-tolerant, a requirement for many systems. Our first contribution is a modified version of CFABCast to handle Byzantine failures. Unfortunately, the resulting protocol is not collision-fast due to the possibility of malicious failures. In fact, our second contribution is to prove that there are no Byzantine collision-fast algorithms in an asynchronous model as traditionally extended to solve Consensus. Finally, our third contribution is a Byzantine collision-fast algorithm that bypasses the stated impossibility by means of a USIG (Unique Sequential Identifier Generator) trusted component.
 
