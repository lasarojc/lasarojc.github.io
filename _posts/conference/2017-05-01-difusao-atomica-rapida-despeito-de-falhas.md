---
layout: post
categories:
 - Publications

title: Algoritmo de Difusao Atomica Rapido a Despeito de Colisoes Tolerante a Falhas Bizantinas
author: Rodrigo Saramago, Eduardo Adílio Pelinson Alchieri, Tuanir França Rezende, Lásaro Camargos
venue: XXXV Simpósio Brasileiro de Redes de Computadores e Sistemas Distribuídos (SBRC), Belem, PA, Brazil
paper: https://www.researchgate.net/publication/316911325_Algoritmo_de_Difusao_Atomica_Rapido_a_Despeito_de_Colisoes_Tolerante_a_Falhas_Bizantinas 
type: Peer-reviewed Conference


---
Abstract: The inefficiency of Consensus-based Atomic Broadcast protocols inthe presence of collisions (concurrent proposals) harms their adoption in theimplementation of State Machine Replication.  Proposals that are not decidedin some instance of Consensus (commands not delivered) must be reproposed ina new instance, delaying their execution.  The CFABCast algorithm (Collision-Fast Atomic Broadcast) uses M-Consensus, a Consensus variant, to decide anddeliver multiple values in the same instance.   However,  CFABCast is not By-zantine fault tolerant, a requirement for many systems.  Our first contributionis a variation CFABCast that handles Byzantine failures. Unfortunately, the re-sulting protocol is not collison-fast due to the possibility of Byzantine failures.In fact, our second contribution is the conjecture that there are no Byzantinecollision-fast algorithm in the asynchronous model.  Finally, our third contri-bution is a Byzantine collision-fast algorithm that bypasses our impossibilityconjecture by using the USIG (Unique Sequential Identifier Generator) trustedcomponent. 
