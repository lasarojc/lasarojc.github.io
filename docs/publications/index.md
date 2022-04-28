I am a computer scientist working on the design and implementation of large scale distributed systems including, but not limited to, P2P systems, Network Protocols, and Agreement Problems.
I enjoy reasoning about concurrency in large scale systems and the challenges it brings to achieving consistency.

The following is an incomplete list of my publications. 
As time allows I will complete it and add details. 
In the mean time, if you need more information, please visit [Research Gate](http://www.google.com/url?q=http%3A%2F%2Fwww.researchgate.net%2Fprofile%2FLasaro_Camargos&sa=D&sntz=1&usg=AFQjCNF3tgNGeYe1XaW89jbOEm9fBRY-0g), your favorite academic search engine, or contact me directly.

## Patents

1. **Decommissioning, re-commissioning, and commissioning new metadata nodes in a working distributed data storage system**    
    Lasaro Camargos, Deepak Jain, Avinash Lakshman, and Bharat Pundalik Naik
    Publication number: 20220100710. Publication date: March 31, 2022      
    United States Patent and Trademark Office.
    
    ??? "Abstract"
        In a running distributed data storage system that actively processes I/Os, metadata nodes are commissioned and decommissioned without taking down the storage system and without introducing interruptions to metadata or payload data I/O. The inflow of reads and writes continues without interruption even while new metadata nodes are in the process of being added and/or removed and the strong consistency of the system is guaranteed. Commissioning and decommissioning nodes within the running system enables streamlined replacement of permanently failed nodes and advantageously enables the system to adapt elastically to workload changes. An illustrative distributed barrier logic (the “view change barrier”) controls a multi-state process that controls a coordinated step-wise progression of the metadata nodes from an old view to a new normal. Rules for I/O handling govern each state until the state machine loop has been traversed and the system reaches its new normal.

1. **Commissioning and decommissioning metadata nodes in a running distributed data storage system**   
    Lasaro Camargos, Deepak Jain, Bharat Naik, and Avinash Lakshman    
    Publication number: 20220103622. Publication date: March 31, 2022      
    United States Patent and Trademark Office.   
    
    ??? "Abstract"
         In a running distributed data storage system that actively processes I/Os, metadata nodes are commissioned and decommissioned without taking down the storage system and without introducing interruptions to metadata or payload data I/O. The inflow of reads and writes continues without interruption even while new metadata nodes are in the process of being added and/or removed and the strong consistency of the system is guaranteed. Commissioning and decommissioning nodes within the running system enables streamlined replacement of permanently failed nodes and advantageously enables the system to adapt elastically to workload changes. An illustrative distributed barrier logic (the “view change barrier”) controls a multi-state process that controls a coordinated step-wise progression of the metadata nodes from an old view to a new normal. Rules for I/O handling govern each state until the state machine loop has been traversed and the system reaches its new normal.

1. **Anti-entropy based metadata recovery in a strongly consistent distributed data storage system**     
    Deepak Jain, Lasaro Camargos, Srinivas Lakshman, and Avinash Lakshman    
    Publication number: 20220100618. Publication date: March 31, 2022      
    United States Patent and Trademark Office.   
    
    ??? "Abstract" 
        A strongly consistent distributed data storage system comprises an enhanced metadata service that is capable of fully recovering all metadata that goes missing when a metadata-carrying disk, disks, and/or partition fail. An illustrative recovery service runs automatically or on demand to bring the metadata node back into full service. Advantages of the recovery service include guaranteed full recovery of all missing metadata, including metadata still residing in commit logs, without impacting strong consistency guarantees of the metadata. The recovery service is network-traffic efficient. In preferred embodiments, the recovery service avoids metadata service downtime at the metadata node, thereby reducing the impact of metadata disk failure on the availability of the system. The disclosed metadata recovery techniques are said to be “self-healing” as they do not need manual intervention and instead automatically detect failures and automatically recover from the failures in a non-disruptive manner.

1. **Container Data mover for Migrating Data Between Distributed Data Storage Systems Integrated with Application Orchestrators**    
    Srividhya Kavaipatti Anantharamakrishnan, Lásaro Camargos, Abhijith Shenoy, Xiangyu Wang, Avinash Lakshman, Srinivas Lakshman     
    Publication number: 20220092024 Publication date: March 24, 2022.   
    United States Patent and Trademark Office.    
    
    ??? "Abstract" 
        A distributed data storage system comprises features for integration with application orchestrators such as Kubernetes, and includes a proprietary Container Storage Interface (CSI) driver. Features include setting snapshot scheduling and retention policies, and a “container data mover” that replicates data from a source to a distinct destination distributed data storage system. The migration may be configured one-to-one, one-to-many, unidirectional, and/or bi-directional. Metadata-based snapshots and metadata-based changed block tracking identify payload data to move from source to destination within application orchestrator frameworks at both ends. Payload data is migrated from source to destination using different techniques than those used for migrating metadata, e.g., kernel-to-kernel for copying payload data versus ordinary metadata writes. An illustrative barrier logic ensures that the migration follows a controlled progression of operations.

1. **Synchronization of Metadata in a Distributed Storage System**
    Avinash Lakshman, Lasaro Camargos and Deepak Jain            
    Publication Number: 20200334207.    Publication Date: Oct. 22, 2020.    
    United States Patent and Trademark Office.    
    
    ??? "Abstract" 
        A client machine writes to and reads from a virtual disk on a remote storage platform. Metadata is generated and stored in replicas on different metadata nodes of the storage platform. A modified log-structured merge tree is used to store and compact string-sorted tables of metadata. During file storage and compaction, a consistent file identification scheme is used across all metadata nodes. A fingerprint file is calculated for each SST (metadata) file on disk that includes hash values corresponding to regions of the SST file. To synchronize, the fingerprint files of two SST files are compared, and if any hash values are missing from a fingerprint file then the key-value-timestamp triples corresponding to these missing hash values are sent to the SST file that is missing them. The SST file is compacted with the missing triples to create a new version of the SST file. The synchronization is bi-directional.
    
1. **Storage and Synchronization of Metadata in a Distributed Storage System**     
    Avinash Lakshman, Lasaro Camargos and Deepak Jain    
    Publication Number: 20200334206.    Publication Date: Oct. 22, 2020.    
    United States Patent and Trademark Office.
    
    ??? "Abstract" 
        A client machine writes to and reads from a virtual disk on a remote storage platform. Metadata is generated and stored in replicas on different metadata nodes of the storage platform. A modified log-structured merge tree is used to store and compact string-sorted tables of metadata. During file storage and compaction, a consistent file identification scheme is used across all metadata nodes. A fingerprint file is calculated for each SST (metadata) file on disk that includes hash values corresponding to regions of the SST file. To synchronize, the fingerprint files of two SST files are compared, and if any hash values are missing from a fingerprint file then the key-value-timestamp triplets corresponding to these missing hash values are sent to the SST file that is missing them. The SST file is compacted with the missing triplets to create a new version of the SST file. The synchronization is bi-directional.
        
1. **Synchronizing Metadata in a Data Storage Platform Comprising Multiple Computer Nodes**    
    Avinash Lakshman, Lasaro Camargos and Deepak Jain    
    Publication Number: 20200334205.    Publication Date: October 22, 2020.    
    United States Patent and Trademark Office.    
    
    ??? "Abstract" 
        A client machine writes to a virtual disk on a remote storage platform. Metadata is generated and stored in replicas on different nodes of the storage platform. A modified log-structured merge tree is used to store and compact string-sorted tables of metadata. During file storage and compaction, a consistent file identification scheme is used across all metadata nodes. A fingerprint file is calculated for each SST (metadata) file on disk that includes hash values corresponding to regions of the SST file. To synchronize, the fingerprint files of two SST files are compared, and if any hash values are missing from a fingerprint file then the key-value-timestamp triplets corresponding to these missing hash values are sent to the SST file that is missing them. The SST file is compacted with the missing triplets to create a new version of the SST file. The synchronization is bi-directional as between distinct computer nodes.
        
1. **Synchronization of Metadata in a Distributed Storage System**    
    Avinash Lakshman, Lasaro Camargos, Deepak Jain 
    Patent Number: US 10740300.    Patent Date: August 11, 2020.    
    United States Patent and Trademark Office.    
    
    ??? "Abstract" 
        A client machine writes to and reads from a virtual disk on a remote storage platform using a storage protocol. Metadata is generated and is stored in replicas on different metadata nodes of the storage platform. A modified log-structured merge tree is used to store and compact string-sorted tables of metadata. During file storage and compaction, a consistent file identification scheme is used across all metadata nodes. A fingerprint file is calculated for each SST file on disk that includes hash values corresponding to regions of the SST file. To synchronize, the fingerprint files of two SST files are compared, and if any hash values are missing from a fingerprint file then the key-value-timestamp triples corresponding to these missing hash values are sent to the SST file that is missing them in the SST file is compacted with the missing triples to create a new version of the SST file. The other fingerprint file is then analyzed the same way.
## Journals

1. **Analysis of Monitoring and Multipath Support on top of OpenFlow Specification**   
    Pedro Rezende, Paulo R. S. L. Coelho, Luiz F. Faina, Lasaro Camargos, Rafael Pasquini  
    International Journal of Network Management   
    [PDF](https://onlinelibrary.wiley.com/doi/abs/10.1002/nem.2017)   

    ??? "Abstract"
        In general, traffic is pushed through a single path despite the existence of alternative paths in networks. For example, routing solutions based on spanning tree prune the topology to prevent loops, consequently preventing also the use of alternative paths. Research on quality of service frequently advocates that the use of alternative paths is interesting for enforcing Service Level Agreements (SLAs), bypassing bottlenecks created by shortest paths. In this paper, we are interested in analyzing the support for monitoring network traffic and for provisioning of multipaths in software‐defined networking (SDN), given the strong platform it provides for experimentation of new networked solutions. Our approach firstly enriches the topology view at the control plane with data gathered through fine grain data plane monitoring. On the basis of such enriched view, our system determines the path, or multipaths, necessary to enforce the specified SLA. We propose 2 extension modules to an OpenFlow controller: SDNMon, which monitors the data plane to enrich the topology information at the control plane, and MP‐Routing, which determines a set of paths, in the absence of a single path capable of enforcing the SLA. Both modules are extensively evaluated, and the results not only demonstrate what can be achieved in terms of accuracy in SDNMon and in terms of quality of service benefits in MP‐Routing but also highlight some limitations of OpenFlow specification. On the basis of our findings, we propose a set of new counters to Per Port and Per Flow granularity levels of OpenFlow specification.


1. **A game theoretical approach to model the channel selection dynamics in non-coordinated IEEE 802.11 networks**   
    Sérgio L. D. L. Gramacho, Gustavo B. Figueiredo, Lasaro Camargos   
    Wireless Networks   
    [PDF](https://link.springer.com/article/10.1007%2Fs11276-018-1751-y)   
    
    ??? "Abstract"
        The massive deployment of Wireless Local Area Networks has made interference mitigation between neighboring networks a challenging issue. These uncoordinated access networks aim at improving their operation by choosing the best wireless channel available, characterizing a competition over the restricted set of possible channels. This work analyses this competition using Game Theory and Markov Chains models, showing that such competitive behavior can lead to Nash Equilibria and that outcomes mostly will not be maximal. Additionally, partially and fully cooperative models are proposed and evaluated, allowing (a) individual players to increase global results using arbitrarily computed and non-rational moves, and (b) achieving maximal outcomes when considering the cooperation of up to all players.


1.  **Multicoordinated agreement for groups of agents**   
    Lasaro Camargos, Rodrigo Schmidt, Edmundo R. M. Madeira, Fernando Pedone     
    Journal of the Brazilian Computer Society   
    [PDF](https://journal-bcs.springeropen.com/articles/10.1007/s13173-010-0001-7)    

    ??? "Abstract"
        Agents in agreement protocols play well distinct roles. Proposers propose values to the acceptors, which will accept proposals and inform the learners so they detect that an agreement has been reached. A fourth role is that of the coordinator, who filters the proposals from proposers to acceptors. While proposers, learners, and coordinators are easily replaced, substituting an acceptor is prohibitive. Protocols that do not employ a coordinator are less resilient to acceptor failures. Protocols that use one coordinator are more resilient to acceptor failures, at the expense of one extra communication step even in the absence of failures. Moreover, they require replacing the coordinator as soon as it fails, a reconfiguration that, although relatively inexpensive, diminishes the protocol availability. Hence, either option, i.e, one or zero coordinator, has its drawbacks. In previous works, we have presented an alternative: multicoordinated agreement protocols. Such protocols are as resilient as single-coordinated protocols but require less reconfiguration to cope with coordinator failures. In fact, most reconfiguration can be done in parallel to the execution of the protocol's normal steps. Multicoordination can be applied to several problems. In this paper we exemplify its use in solving consensus and then introduce a fast multicoordinated agreement protocol for agents organized in groups, an abstraction for fast local area networks interconnected by slower links.


## Book Chapters

1. **Byzantine Collision-Fast Consensus Protocols**   
    Rodrigo Saramago, Eduardo Alchieri, Tuanir Rezende, Lasaro Camargos  
    Transactions on Computational Collective Intelligence XXXIII   
    [PDF](https://link.springer.com/chapter/10.1007%2F978-3-662-59540-4_6)   

    ??? "Abstract"
        Atomic broadcast protocols are fundamental building blocks used in the construction of many reliable distributed systems. Atomic broadcast and consensus are equivalent problems, but the inefficiency of consensus-based atomic broadcast protocols in the presence of collisions (concurrent proposals) harms their adoption in the implementation of reliable systems, as the ones based on state machine replication. In the traditional consensus protocols, proposals that are not decided in some instance of consensus (commands not delivered) must be re-proposed in a new instance, delaying their execution. Moreover, whether different values (commands) are proposed in the same instance (leading to a collision), some of its phases must be restarted, also delaying the execution of these commands involved in the collision. The CFABCast (Collision-Fast Atomic Broadcast) algorithm uses m-consensus to decide and deliver multiple values in the same instance. However, CFABCast is not byzantine fault-tolerant, a requirement for many systems. Our first contribution is a modified version of CFABCast to handle byzantine failures. Unfortunately, the resulting protocol is not collision-fast due to the possibility of malicious failures. In fact, our second contribution is to prove that there are no byzantine collision-fast algorithms in an asynchronous model as traditionally extended to solve consensus. Finally, our third contribution is a byzantine collision-fast algorithm that bypasses the stated impossibility by means of a USIG (Unique Sequential Identifier Generator) trusted component.

## Peer-reviewed Conferences


1. **Intrusion Detection over Network Packets using Data Stream Classification Algorithms**   
    G. Olímpio Jr., P. Franklin, R. Miani, L. Camargos and E.Faria   
    The 33rd IEEE International Conference on Tools with Artificial Intelligence (ICTAI) Virtually
    [PDF]

    ??? "Abstract"
        Intrusion Detection Systems (IDS) are a popular solution against cyber-attacks. IDS collect network traffic in- formation and identify attack attempts by inspecting packets individually or in the context of flows. In this work, we consider the intrusion detection process a classification task over a stream of continuously generated packets with a non-stationary data distribution. To cope with this task, we advocate using state- of-the-art Stream Mining algorithms that constantly learn what normal traffic is and what could be an attack. We determined that inspecting packets individually renders similar performance to examining flows in several situations and that only a subset of the packets’ headers is sufficient for the classification. These re- sults are shown through experimentation using the CICIDS2017 dataset and through multiple measures.


1. **Bandwidth throttling in a P4 switch**    
    Lucas Borges Fernandes and Lasaro Camargos    
    IEEE Conference on Network Function Virtualization and Software Defined Networks (IEEE NFV-SDN 2020), Virtual Conference
    [PDF]

    ??? "Abstract"
         Quality of service (QoS) provisioning is an important subject for the computer networks community and, as many other problems, has been revisited under the light of Software Defined Networks (SDN), which promise flexibility and simplification of network protocols.
         We follow such trend in this paper, proposing a bandwidth throttling solution using the P4 framework and contrasting it with the state of the art.
         Our proposal showcases the simplicity and adaptability of P4-programmable switches.

1. **On the Impossibility of Byzantine Collision-Fast Atomic Broadcast**   
    Rodrigo Saramago, Tuanir França Rezende, Eduardo Adílio Pelinson Alchieri, Lasaro Camargos   
    The 32nd IEEE International Conference on Advanced Information Networking and Applications (IEEE AINA-2018), Krakow, Poland     
    [PDF](https://www.researchgate.net/publication/325264988_On_the_Impossibility_of_Byzantine_Collision-Fast_Atomic_Broadcast)   

    ??? "Abstract"
        The inefficiency of Consensus-based Atomic Broadcast protocols in the presence of collisions (concurrent proposals) harms their adoption in the implementation of State Machine Replication. Proposals that are not decided in some instance of Consensus (commands not delivered) must be re-proposed in a new instance, delaying their execution. The CFABCast (Collision-Fast Atomic Broadcast) algorithm uses M-Consensus to decide and deliver multiple values in the same instance. However, CFABCast is not Byzantine fault-tolerant, a requirement for many systems. Our first contribution is a modified version of CFABCast to handle Byzantine failures. Unfortunately, the resulting protocol is not collision-fast due to the possibility of malicious failures. In fact, our second contribution is to prove that there are no Byzantine collision-fast algorithms in an asynchronous model as traditionally extended to solve Consensus. Finally, our third contribution is a Byzantine collision-fast algorithm that bypasses the stated impossibility by means of a USIG (Unique Sequential Identifier Generator) trusted component.

1. **Algoritmo de Difusao Atomica Rapido a Despeito de Colisoes Tolerante a Falhas Bizantinas**   
    Rodrigo Saramago, Eduardo Adílio Pelinson Alchieri, Tuanir França Rezende, Lásaro Camargos   
    XXXV Simpósio Brasileiro de Redes de Computadores e Sistemas Distribuídos (SBRC, 2017), Belem, PA, Brazil   
    [PDF](https://www.researchgate.net/publication/316911325_Algoritmo_de_Difusao_Atomica_Rapido_a_Despeito_de_Colisoes_Tolerante_a_Falhas_Bizantinas)   

    ??? "Abstract"
        The inefficiency of Consensus-based Atomic Broadcast protocols inthe presence of collisions (concurrent proposals) harms their adoption in theimplementation of State Machine Replication.  Proposals that are not decidedin some instance of Consensus (commands not delivered) must be reproposed ina new instance, delaying their execution.  The CFABCast algorithm (Collision-Fast Atomic Broadcast) uses M-Consensus, a Consensus variant, to decide anddeliver multiple values in the same instance.   However,  CFABCast is not By-zantine fault tolerant, a requirement for many systems.  Our first contributionis a variation CFABCast that handles Byzantine failures. Unfortunately, the re-sulting protocol is not collison-fast due to the possibility of Byzantine failures.In fact, our second contribution is the conjecture that there are no Byzantinecollision-fast algorithm in the asynchronous model.  Finally, our third contri-bution is a Byzantine collision-fast algorithm that bypasses our impossibilityconjecture by using the USIG (Unique Sequential Identifier Generator) trustedcomponent. 

1. **On Making Generalized Paxos Practical**   
    Tuanir França Rezende, Pierre Sutra, Rodrigo Saramago, Lásaro Camargos   
    The 31st IEEE International Conference on Advanced Information Networking and Applications (IEEE AINA-2017)   
    [PDF](https://www.researchgate.net/publication/313550141_On_Making_Generalized_Paxos_Practical)   

    ??? "Abstract"
        Generalized Paxos, GPaxos, is a recent solution to Generalized Consensus, a distributed problem to which several key agreement problems reduce. We envision that GPaxos may unify within a single and novel Agreement-as-a-Service infrastructure multiple distributed protocols. To date this potential is however not fully unleashed, due to the steep learning curve of the protocol and the high complexity of its implementation.Moreover, before GPaxos reaches a real world usage, several computationally expensive operations have to be optimized and simplified. This paper aims at closing this gap between theory and practice. To this end, we first provide a concise tour of Generalized Paxos, hardly found elsewhere. Then, we assess the versatility of the Generalized Consensus problem by presenting a variation of GPaxos that solves the lease coordination problem. Our last contribution consists in three optimizations that apply to the critical phases of the algorithm: i) a method to quickly start a new round, ii) a novel approach to execute a checkpoint, and iii) a data structure that speeds-up the detection of an agreement.


1. **Priority-Based State Machine Replication with PRaxos**   
    Paulo R. Pinho Filho, Luciana De Oliveira Rech, Lau Cheuk Lung, Miguel Correia, Lásaro Camargos   
    2016 IEEE 30th International Conference on Advanced Information Networking and Applications (AINA)    
    [PDF](https://ieeexplore.ieee.org/document/7474136)   

    ??? "Abstract"
         State machine replication is a form of active replication commonly used to create fault-tolerant distributed services. In a nutshell, the approach consists in ensuring that a set of replicas receive and execute the same sequence of deterministic requests, returning the same results. This approach handles all requests evenly, but for some services it is important to consider that some requests have priority over others, i.e., that whenever two or more requests are ready to be executed, the one with higher priority is executed first. Paxos is perhaps the best known protocol to order requests in asynchronous environments, but Paxos has no notion of priority. In this paper we introduce the notion of priority-based state machine replication and modify Paxos to take request priorities into account. The proposed algorithm, PRaxos, works in three steps and satisfies Paxos' safety properties in asynchronous systems, while enforcing priorities when the system behaves synchronously. 

1. **An Architecture for Monitoring and Improving Public Transportation Systems**   
    Pedro H. S. Duarte, Luis F. Faina, Lásaro Camargos, Luciano B. de Paula, Rafael Pasquini  
    2016 IEEE 30th International Conference on Advanced Information Networking and Applications (AINA), Crans-Montana, Switzerland   
    [PDF](https://ieeexplore.ieee.org/document/7474181)    

    ??? "Abstract"
        Brazilian public transportation systems are facing a significant demand reduction, mainly due to the poor quality of the offered services, lack of information regarding lines and timetables, high cost and lack of investment from the government. Even though it is not trivial to improve financial aspects related to the public transportation system, this work claims that the overall system quality can be improved through ubiquitous data collection according to a proposed ontology, which is the basis for knowledge extraction to support the required quality of experience improvements. The proposed architecture relies on standard technologies available nowadays, providing a low cost solution for the required data collection and analysis. This paper presents the proposed inter-networking architecture and ontology, then evaluates the system performance using a prototype developed with standard solutions.

1. **An Architecture for Traffic Sign Management in Smart Cities**   
    Everton Lira, Enrique Fynn, Paulo R. S. L. Coelho, Luis F Faina, Lasaro Camargos, Rodolfo S. Villaca, Rafael Pasquini   
    2016 IEEE 30th International Conference on Advanced Information Networking and Applications (AINA), Crans-Montana, Switzerland   
    [PDF](https://ieeexplore.ieee.org/document/7474141)      

    ??? "Abstract"
        This  paper  introduces  and  evaluates  a  Traffic  SignManagement Architecture (TSMA), which represents a paradigmshift  for  the  deployment  of  traffic  sign  infrastructure  in  thecontext of Intelligent Transport Systems, Vehicular Networks andSmart  Cities.  The  proposal  addresses  limitations  of  the  currenttraffic control model by enabling remote updates of traffic signsand  displaying  them  on  the  vehicular  navigation  system  displayto  improve  their  legibility.  TSMA  is  an  architecture  developedto  provide  V2I  interaction  using  a  commodity  technology,  Wi-Fi,  through  the  beacon-stuffing  technique.  The  initial  design  ofTSMA’s  security  mechanisms  is  also  presented  in  this  paper.Evaluations   were   performed   on   a   developed   prototype   andsimulation  environments. 

1. **AR2C2 - Actively Replicated Controllers for SDN resilient Control Planes**   
    Eros S. Spalla, Diego Rossi Mafioletti, Alextian Bartolomeu Liberato, Gilberto Ewald, Christian Esteve Rothenberg, Lásaro Camargos, Rodolfo Villaca, Magnos Martinello   
    2016 IEEE/IFIP Network Operations and Management Symposium (NOMS 2016)
    [PDF](https://doi.org/10.1109/NOMS.2016.7502812)

    ??? "Abstract"
        Software Defined Networking (SDN) is a promisingarchitectural  approach  based  on  a  programmatic  separation  ofthe  control  and  data  planes.  For  high  availability  purposes,logically  centralized  SDN  controllers  follow  a  distributed  im-plementation.  While  controller  role  features  in  the  OpenFlowprotocol allow switches to communicate with multiple controllers,these mechanisms alone are not sufficient to guarantee a resilientcontrol  plane,  leaving  the  actual  implementation  an  open  chal-lenge for SDN designers. This paper explores OpenFlow roles forthe  design  of  resilient  SDN  control  plane  and  proposes  AR2C2as  an  actively  replicated  multi-controller  strategy.  As  proof  ofconcept,  AR2C2  is  implemented  based  on  the  Ryu  controllerand  relying  on  OpenReplica  to  ensure  consistent  state  amongthe   distributed   controllers.   Our   prototype   is   experimentallyevaluated  using  real  commodity  switches  and  Mininet  emulatedenvironment.  Results  of  the  measured  times  to  recover  fromfailures for different workloads shed some light on the practicaltrade-offs on replication overhead and latency as a step forwardtowards  SDN  resiliency. 

1. **Roteamento Multicaminhos em Redes Definidas por Software**   
    Pedro Rezende, Luis Fernando Faina, Lásaro Camargos, Rafael Pasquini   
    XXXIV Simpósio Brasileiro de Redes de Computadores e Sistemas Distribuídos (SBRC 2016), Salvador, Brazil   
    [PDF](https://www.researchgate.net/publication/304183929_Roteamento_Multicaminhos_em_Redes_Definidas_por_Software)   

1. **Replicação de Máquina de Estado Baseada em Prioridade com PRaft**   
    Paulo R. Pinho Filho, Luciana Rech, Lau Cheuk Lung, Miguel Correia, Lásaro Camargos   
    XXXIV Simpósio Brasileiro de Redes de Computadores e Sistemas Distribuídos (SBRC 2016), Salvador, Brazil   
    [PDF](https://www.researchgate.net/publication/304183954_Replicacao_de_Maquina_de_Estado_Baseada_em_Prioridade_com_PRaft)   

    ??? "Abstract"
        State machine replication is an approach to create fault tolerant dis-tributed systems.  The system remains corret while tolerating faults from someof its replicas.  These replicas must execute the same sequence of requests, aproblem that is solved by total order algorithsm like Raft.  some services mayneed that requests have different priority levels, such that some be executed be-fore others.  In this work, we propose an algorithm, PRaft, that introduces theidea of priority based state machine replication to Raft, modifying it to deal withrequest priority. 

1. **Busca por Similaridade no CassandraDB (Short Paper)**
    Antonio Mourão, Rafael Pasquini, Rodolfo Villaça, Lásaro Camargos   
    2016 31st Brazilian Symposium on Databases   
    [PDF](https://www.researchgate.net/publication/309121006_Busca_por_Similaridade_no_CassandraDB )   

    ??? "Abstract"
        The need for scalability in the Big Data era has lead to flourishing of distributed NOSQL systems. However, none of the widely used solutions available support similarity searches, another important feature in such scenarios. Here we propose to overcome this limitation by extending Cassandra with similarity search capabilities. Our approach is based on using locality sensitive hashing to spread data to nodes, to target nodes for queries, and for efficiently recovering similar data from stable storage at the nodes. We overview how to implement the approach, our test plan, and initial results. Resumo. A necessidade de escalabilidade em cenários de Big Data levou à prosperação dos NOSQL distribuídos. Contudo, as soluções mais amplamente usadas não suportam uma outra característica desejável, busca por similari-dade. Neste artigo propomos contornar tal limitação estendendo o Cassandra com suporte a buscas por dados similares. Nossa abordagem usa hashing sensí-vel à localidade para distribuir dados entre nós, direcionar buscas, e recuperar dados em armazenamento estável de forma eficiente. Descrevemos aqui como implementar esta abordagem, nosso plano de testes e resultados iniciais. Introdução Cassandra [Lakshman and Malik 2010] é um banco de dados NOSQL (Not Only SQL) amplamente utilizado em cenários BigData devido à sua escalabilidade horizontal. Como em outros NOSQL [Decandia et al. 2007, Chang et al. 2008], essa característica vem do consistent hashing, particionamento aleatório dos dados entre os nós do sistema que dis-tribui a carga uniformemente entre os mesmos e facilita sua entrada e saída do sistema [Stoica et al. 2001]. Apesar das vantagens, essa distribuição dificulta a busca por dados similares, outra característica desejável em BigData. Dois objetos de um mesmo domínio são similares se seus atributos possuem um grau de semelhança elevado; caso contrário são dissimilares. A busca por similaridade consiste em recuperar objetos que sejam similares aos parâmetros da consulta. Alguns exemplos incluem a identificação de perfis de clientes com hábitos de consumo parecidos e de imagens com o mesmo tema. Dentre alguns esforços para se melhorar a busca por similaridade nestes sistemas, destacamos a HammingDHT [Villaca et al. 2013]. Na HammingDHT, a chave de cada objeto é construída por uma função de espa-lhamento sensível a localidade (LSH), que gera chaves similares para dados similares e ???++ " Agradecimentos à CAPES, CNPq, FAPEMIG e FAPES pelo apoio à realização deste trabalho.



 
## Peer-reviewed Workshop 

1. **Comutador P4 com Suporte a Roteamento Multicaminhos**   
    Lucas Borges Fernandes, Pedro Henrique Ribeiro, Leonardo Martins, Rafael Pasquini, Luis F. Faina, Lasaro Camargos   
    IX Workshop de Pesquisa Experimental da Internet do Futuro (WPEIF 2018)    
    [PDF](https://www.researchgate.net/publication/325265001_Comutador_P4_com_Suporte_a_Roteamento_Multicaminhos)    
    
    ??? "Abstract"
        In this paper we describe a network switch with multi-path routing capabilities. The switch is implemented using P4, easily extensible and available as a free software project. The switch supports different routing policies, which adhere to different levels of QoS, making the network use very flexible. 

1. **Mechanism Reduction via Adjacency Matrix Power**   
    Lásaro Camargos, João Marcelo Vedovoto, Ricardo Serfaty, Aristeu da Silveira Neto    
    5th International Workshop on Model Reduction in Reacting Flows (IWMRRF 2015), Spreewald, Germany    
    [PDF](https://www.researchgate.net/publication/280157089_Mechanism_Reduction_via_Adjacency_Matrix_Power)

    ??? "Abstract"
        Mechanism reduction is badly needed in large scale chemical simulations. Most graph based approaches, such as Directed Relation Graphs, derive the dependency of a species on all the others using single paths between them, which is not optimal. But since calculating the optimal solution has prohibitive costs, in this paper we propose the use of all the paths of a given large size to approximate the dependency. 



## Thesis

1. **PhD Dissertation - Multicoordinated agreement protocols and the log service**   
    Lasaro Camargos   
    Università della Svizzera Italiana and State university of Campinas   
    [PDF]( https://www.researchgate.net/publication/40754605_Multicoordinated_agreement_protocols_and_the_log_service)    
    
    ??? "Abstract"
        Agreement problems are a common abstraction in distributed systems. They appear when the components of the system must concur on reconfigurations, changes of state, or in lines of action in general. Examples of agreement problems are Consensus, Atomic Commitment, and Atomic Broadcast. In this thesis we investigate these abstractions in the context of the environment in which they will run and the applications that they will serve; in general, we consider the asynchronous crash-recovery model. The goal is to devise protocols that explore the contextual information to deliver improved availability. The correctness of our protocols holds even when the extra assumptions do not. In the first part of this thesis we explore the following property: messages broadcast in small networks tend to be delivered in order and reliably. We make three contributions in this part. The first contribution is to turn known Consensus algorithms that harness this ordering property to reach agreement in the crash-stop model into practical protocols. That is, protocols that tolerate message losses and recovery after crashes, efficiently. Our protocols ensure progress even in the presence of failures, if spontaneous ordering holds frequently. In the absence of spontaneous ordering, some other assumption is required to cope with failures. The second contribution of this thesis is to generalize one of our crash-recovery consensus protocols as a ``multicoordinated'' mode of a hybrid Consensus protocol, that may use spontaneous ordering or failure detection to progress. Compared to other protocols, ours provide improved availability with no price in resilience. The third contribution is to employ this new mode to solve Generalized Consensus, a problem that generalizes a series of other agreement problems and, hence, is of much practical interest. Moreover, we considered several aspects of solving this problem in practice, which had not been considered before. As a result, our Generalized Consensus protocol features graceful degradation, load balancing, and is parsimonious in accessing stable storage. In the second part of this thesis we have considered agreement problems in wide area networks organized hierarchically. More specifically, we considered a topology that is commonplace in the data centers of large corporations: groups of nodes, with large-bandwidth low-latency links connecting the nodes in the same group, and slow and limited links connecting nodes in different groups. In such environments, latency is clearly a major concern and reconfiguration procedures that render the agreement protocol momentarily unavailable must be avoided as much as possible. Our contribution here is in avoiding reconfigurations and improving the availability of a collision fast agreement protocol. That is, a protocol that can reach agreement in two intergroup communication steps, irrespectively to concurrent proposals. Besides the use of a multicoordinated approach, we employed multicast primitives and consensus to restrict some reconfigurations to within groups, where they are less expensive. In the last part of this thesis we study the problem of terminating distributed transactions. The problem consists of enforcing agreement among the parties on whether to commit or rollback the transaction and ensuring the durability of committed transactions. Our contribution in this topic is an abstract log service that detaches the termination problem from the processes actually performing the transactions. The service works as a black box and abstracts its implementation details from the application utilizing it. Moreover, it allows slow and failed resource managers be re-started on different hosts without relying on the stable storage of the previous host. We provide two implementations of the service, which we evaluated experimentally.


1. **MSc Thesis - DisCusS desenvolvendo um Serviço de Consenso genérico, simples e modular**   
    Lasaro Camargos   
    State university of Campinas   
    [PDF](https://www.researchgate.net/publication/264399325_DisCusS_desenvolvendo_um_Servico_de_Consenso_generico_simples_e_modular)    
    
    ??? "Abstract"
        Esta dissertação trata do processo de engenharia de um serviço de detecção de falhas compatível com FT-CORBA, a especificação para tolerância a falhas em CORBA, e de um serviçco de consenso distribuído. Os serviçoos são independentes e fornecem diferentes propriedades para a aplicação cliente, dependendo dos módulos, com implementações de algoritmos diferentes, selecionados para uma instanciação destes serviços. A arquitetura dos serviços é tal que a aplicação cliente não toma conhecimento dos algoritmos de detecção e consenso sendo executados, acessando-os por uma interface genérica. Com o intuito de facilitar a escolha dos módulos dos serviços, apresentamos um pequeno estudo comparativo da influência de detectores de falhas adaptativos, aqueles que se adaptam para prover melhor qualidade de serviço na detecção, e não adaptativos sobre o desempenho dos algoritmos de consenso distribuído.
