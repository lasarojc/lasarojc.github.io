# Sistemas Distribuídos

Bem vindos ao curso de Sistemas Distribuídos. Este material é comum para as duas disciplinas, isto é, GBC 074 (BCC) e GSI 028 (BSI).
Esta página é o ponto de partida para acesso a todo o material que estudaremos.



A seguir, veja o plano de como nossa interação acontecerá. Para deixar bem claro,  isto é um plano, e planos ~~podem ser~~ serão alterados:

![Plano](images/plano.jpg)



Para comunicação, usaremos o MS-Teams. 
Para entrar no time do curso, logue-se com seu email institucional usando este [apontador](https://teams.microsoft.com/l/team/19%3aENVynv2QRS0qTMt3LYXi14qmLrtNsHD4KFUIKQARFb01%40thread.tacv2/conversations?groupId=be53d70a-3131-4c1e-9fb2-f38bcb4bad21&tenantId=cd5e6d23-cb99-4189-88ab-1a9021a0c451) e use o código **zn6p1cp** para entrar no time.


As atividades da semana serão postadas abaixo, semana a semana.
Na descrição das atividades,

* **NA** quer dizer Notas de Aula, acessíveis em https://lasarojc.github.io/ds_notes/, 
* **S** quer dizer **atividade síncrona** na data em postada, feita em uma reunião no MS-Teams, gravada e disponibilizada para revisão posterior e como atividade assíncrona pela outra turma, e 
* **A** quer dizer **atividade assíncrono**, a ser realizado pelo discente antes da próxima atividade.





## Semana 1

* S - 12/07/2021: 8:50 e 20:50
      * Apresentação
          * (NA) [Prefácio](https://lasarojc.github.io/ds_notes/preface/)

      * Plano do curso: ver aba arquivos no MS Teams
      * Seminários

          * O **objetivo** dos seminários é apresentar tópicos modernos relacionados à computação distribuída.

          ![Know your buzzwords](images/dilbert.jpeg)

          * Os alunos deverão gravar seminários, em grupos de 2 alunos, para seus colegas.
          * Cada seminário terá duração de 40 minutos.
          * Cada seminário será acompanhado por um questionário desenvolvido pelos apresentadores a ser respondido ***offline***.
          * Sua apresentação será avaliada nos seguintes pontos:
             * Duração
             * Conteúdo: 
                * Contextualização
                * Importância para o profissional da área
                * Referencial teórico
                * Algo mais: discussão, vídeo, lab
             * Qualidade dos slides
             * Qualidade do questionário
                * Não faça questões triviais.
                * Coloque 5 alternativas que façam sentido, mas só uma correta.
                * Não use "todas as alternativas" ou "nenhuma das alternativa" ou coisas do gênero.
             * Proposta de temas
                * Arquiteturas distribuídas reativas usando Kafka
                * [Pravega.io](https://pravega.io)
                * Event Sourcing 
                * [O protocolo PBFT](https://medium.com/thundercore/consensus-series-pbft-3e011e7f3691)
                * [Algorand](https://algorand.foundation/)
                * [Dapr](https://docs.dapr.io)
                * Kubernetes
                * [Cache distribuído Redis](https://redislabs.com/solutions/use-cases/caching/)
                * [New Directions in Cloud Programming](http://cidrdb.org/cidr2021/papers/cidr2021_paper16.pdf)
                * O protocolo [Hermes](https://hermes-protocol.com/)
                * Se precisar de um tema, entre em contato. 

      * Projeto

        * Os alunos desenvolverão um projeto seguindo uma **especificação intencionalmente vaga** para exercitar sua capacidade de resolução de problemas usando os conceitos apresentados na disciplina.
        * Questionamentos podem e devem ser feitos para refinar a especificação.

        * A especificação será disponibilizada [aqui](https://lasarojc.github.io/ds_notes/projeto/)
        * Grupos dos trabalhos serão compostos por no mínimo 4 e no máximo 6 alunos.
            * Não, não pode ter menos de 4 ou mais de 6.
            * Grupos podem ter membros das duas turmas.


   * Introdução
      * (NA) [O quê são Sistemas Distribuídos?](https://lasarojc.github.io/ds_notes/intro/#tipos-de-sistemas-distribuidos)
      * (NA) [Por quê desenvolvemos sistemas distribuídos?](https://lasarojc.github.io/ds_notes/intro/#por-que-desenvolvemos-sistemas-distribuidos)

* S: 14/07/2021: 10:40
   * Introdução
      * (NA) [Tipos de Sistemas Distribuídos](https://lasarojc.github.io/ds_notes/intro/#tipos-de-sistemas-distribuidos)


* A
    * (LT) Sistemas Distribuídos: Princípios e Paradigmas. Capitulo 1.
    * [Difference Between Centralized, Decentralized & Distributed Systems Oversimplified](https://www.8bitmen.com/difference-between-centralized-decentralized-distributed-systems-explained/)
    * [Transparência - Parte 1](https://dev.to/vaidehijoshi/transparency-illusions-of-a-single-system-part-1-17ao)
    * [Transparência - Parte 2](https://dev.to/vaidehijoshi/transparency-illusions-of-a-single-system-part-2-lbb)



## Semana 2
* S: 19/07/2021: 20:50
   * Comunicação
      * (NA) [Introdução](https://lasarojc.github.io/ds_notes/comm/)-[Sockets](https://lasarojc.github.io/ds_notes/comm/sockets/)

* S: 21/07/2021: 10:40
   * Comunicação
      * (NA) [Sockets](https://lasarojc.github.io/ds_notes/comm/sockets/)
      * (NA) [Representação de dados](https://lasarojc.github.io/ds_notes/comm/datarep/)

* A: 
    * (LT) Sistemas Distribuídos: Princípios e Paradigmas. Comunicação - Seção 4.1
    * [Understanding IP Multicast](http://www.dasblinkenlichten.com/understanding-ip-multicast/)
    * [Beej's Guide to Network Programming - Using Internet Sockets](https://beej.us/guide/bgnet/)
    * Exercícios


## Semana 3
* S: 26/07/2021: 20:50
   * Comunicação
      * (NA) [Middlewares](https://lasarojc.github.io/ds_notes/comm/middleware)

* S: 28/07/2021: 10:40
   * Comunicação
      * (NA) [RPC](https://lasarojc.github.io/ds_notes/comm/rpc/)
      * (NA) [Estudo de caso gRPC](https://lasarojc.github.io/ds_notes/cases/grpc/)

* A
   * (LT) 2.3 Middleware Organization
   * (LT) 4.2 Remote Procedure Call



## Semana 4
* S: 02/08/2021: 20:50
   * Comunicação
      * (NA) [MOM](https://lasarojc.github.io/ds_notes/comm/mom)
      * (NA) [Estudo de caso Mosquito](https://lasarojc.github.io/ds_notes/cases/mosquito/)

* S: 04/08/2021: 10:40
   * Comunicação
      * (NA) [Protocolos Epidêmicos](https://lasarojc.github.io/ds_notes/comm/epidemics/)
   * Especificação da primeira etapa do projeto

* A:
   * (LT) 4.3 Message-Oriented Communication
   * (LT) 4.4 Multicast Communication


## Semana 5
* S: 09/08/2021: 20:50
    * Arquiteturas
        * (NA) [Introdução](https://lasarojc.github.io/ds_notes/arch/)

* S: 11/08/2021: 10:40
    * Arquiteturas
        * (NA) [Peer-2-Peer](https://lasarojc.github.io/ds_notes/p2p/)
        * (NA) Estudo de caso [P2P: Chord](https://lasarojc.github.io/ds_notes/cases/chord/)
    * Discussão sobre a primeira entrega do projeto

* A:
    * (NA) [Peer-2-Peer](https://lasarojc.github.io/ds_notes/p2p/)
    * (NA) Estudo de caso [P2P: Chord](https://lasarojc.github.io/ds_notes/cases/chord/)
    * Exercícios


## Semana 6
* S: 16/08/2021: 20:50
    * (NA) [Modelos computacionais](https://lasarojc.github.io/ds_notes/fundamentals/)

* S: 18/08/2021: 10:40
    * (NA) [Concorrência](https://lasarojc.github.io/ds_notes/coord/concurrency)

* A:
    * (NA) [Microsserviços](https://lasarojc.github.io/ds_notes/arch/microservices/)
    * (NA) [Multithread na Prática](https://lasarojc.github.io/ds_notes/coord/concurrency/#multithread-na-pratica)
    * Exercícios de *multithread*


## Semana 7
* S: 23/08/2021: 20:50
    * (NA) [Exclusão mútua](https://lasarojc.github.io/ds_notes/coord/coord/#exclusao-mutua) 

* S: 15/08/2021: 10:40
    * (NA) [Eleição de líderes](https://lasarojc.github.io/ds_notes/coord/coord/#eleicao-de-lideres) 

* A: desenvolvimento do projeto

## Semana 8
* S: 30/08/2021: 20:50
    * (NA) [Tempo e Relógios Físicos](https://lasarojc.github.io/ds_notes/time/physical/) 

* S: 01/09/2021: 10:40
    * (NA) [Relógios Lógicos](https://lasarojc.github.io/ds_notes/time/logical/) 

* A: Desenvolvimento do projeto

## Semana 9
* S: 06/09/2021 - Recesso
* S: 08/09/2021 - Não há aula - Reposição de terça-feira
* A: Desenvolvimento do projeto

## Semana 10
* S: 13/09/2021: 20:50
     * (NA) [Tolerância a falhas](https://lasarojc.github.io/ds_notes/fault/)

* S: 15/09/2021: 10:40
     * (NA) [Replicação](https://lasarojc.github.io/ds_notes/fault/replication/)
     * (NA) [Detectores de Falhas](https://lasarojc.github.io/ds_notes/fault/failuredetector/)

## Semana 11
* S: 20/09/2021: 20:50
     * (NA) [Acordo](https://lasarojc.github.io/ds_notes/fault/agreement)

* S: 21/09/2021: 10:40
     * (NA) [Estudo de Caso: Ratis](https://lasarojc.github.io/ds_notes/cases/ratis/)


## Semana 12
* S: 27/09/2021: 20:50
     * (NA) [Estudo de Caso: Zookeeper](https://lasarojc.github.io/ds_notes/cases/zookeeper/)

* S: 29/09/2021: 10:40
     * (NA) 

## Semana 13
* S: 04/10/2021: 20:50
     * (NA) [Modelos de Consistência](https://lasarojc.github.io/ds_notes/consistency/consistency_models/)
     * (NA) [Modelos de Consistência centrados nos dados](https://lasarojc.github.io/ds_notes/consistency/data_centric/)

* S: 06/10/2021: 10:40
     * (NA) [Modelos de Consistência centrados nos dados](https://lasarojc.github.io/ds_notes/consistency/data_centric/)
     * (NA) [Modelos de Consistência centrados no cliente](https://lasarojc.github.io/ds_notes/consistency/client_centric/)

## Semana 14
* S: 11/10/2021: 20:50 (NA) Gerenciamento de réplicas e checkpointing
* S: 13/10/2021: 10:40 (NA) Consistência em bancos de dados transacionais

## Semana 15
* S: 18/10/2021: 20:50 (NA) Transações distribuídas. 1PC, 2PC, 3PC, Paxos Commit
* S: 20/10/2021: 10:40 (NA) Árvores de merge de logs (Log structured merge trees). Filtros de Bloom.

## Semana 16
* S: 25/10/2021: 20:50
    * (NA) [Log Structured merge trees]
* S: 27/10/2021: 10:40
    * (NA) [BlockChain]()

## Semana 17
* A: 03/11/2021: 
    * Seminários
    * (NA) [Sistemas de Arquivos]()

