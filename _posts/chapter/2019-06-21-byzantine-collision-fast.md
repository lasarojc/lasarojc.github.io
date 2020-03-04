---
layout: post
categories:
 - Publications

title: Byzantine Collision-Fast Consensus Protocols 
author: Rodrigo Saramago, Eduardo Alchieri, Tuanir Rezende, Lasaro Camargos
venue: Transactions on Computational Collective Intelligence XXXIII
paper: https://link.springer.com/chapter/10.1007%2F978-3-662-59540-4_6
type: chapter


---
Abstract: Atomic broadcast protocols are fundamental building blocks used in the construction of many reliable distributed systems. Atomic broadcast and consensus are equivalent problems, but the inefficiency of consensus-based atomic broadcast protocols in the presence of collisions (concurrent proposals) harms their adoption in the implementation of reliable systems, as the ones based on state machine replication. In the traditional consensus protocols, proposals that are not decided in some instance of consensus (commands not delivered) must be re-proposed in a new instance, delaying their execution. Moreover, whether different values (commands) are proposed in the same instance (leading to a collision), some of its phases must be restarted, also delaying the execution of these commands involved in the collision. The CFABCast (Collision-Fast Atomic Broadcast) algorithm uses m-consensus to decide and deliver multiple values in the same instance. However, CFABCast is not byzantine fault-tolerant, a requirement for many systems. Our first contribution is a modified version of CFABCast to handle byzantine failures. Unfortunately, the resulting protocol is not collision-fast due to the possibility of malicious failures. In fact, our second contribution is to prove that there are no byzantine collision-fast algorithms in an asynchronous model as traditionally extended to solve consensus. Finally, our third contribution is a byzantine collision-fast algorithm that bypasses the stated impossibility by means of a USIG (Unique Sequential Identifier Generator) trusted component.
