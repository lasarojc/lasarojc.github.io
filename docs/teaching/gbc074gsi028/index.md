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
* **S** quer dizer **atividade síncrona**, feita em uma reunião no MS-Teams, gravada e disponibilizada para revisão posterior, e 
* **A** quer dizer **atividade assíncrono**, a ser realizado pelo discente antes da próxima atividade.





## Semana 1

* S
   * Apresentação
   * Plano do curso
      * Controle de Frequência

        O **controle de frequência** nas atividades será pelo relatório produzido pelo MS Teams.

      * Avaliação

        Ver plano de trabalho.

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

        * Os alunos desenvolverão um projeto seguindo uma especificação intencionalmente vaga para exercitar sua capacidade de resolução de problemas usando os conceitos apresentados na disciplina.
        * Questionamentos podem e devem ser feitos para refinar a especificação.

        * A especificação será disponibilizada [aqui](https://lasarojc.github.io/ds_notes/projeto/)
        * Grupos dos trabalhos serão compostos por no mínimo 4 e no máximo 6 alunos.
            * Não, não pode ter menos de 4 ou mais de 6.
            * Grupos podem ter membros das duas turmas.


   * Introdução
      * NA: [Introdução](https://lasarojc.github.io/ds_notes/intro/)

* A
    * NA: [Prefácio](https://lasarojc.github.io/ds_notes/)
    * LT: Sistemas Distribuídos: Princípios e Paradigmas. Capitulo 1.
    * [Difference Between Centralized, Decentralized & Distributed Systems Oversimplified](https://www.8bitmen.com/difference-between-centralized-decentralized-distributed-systems-explained/)
    * [Transparência - Parte 1](https://dev.to/vaidehijoshi/transparency-illusions-of-a-single-system-part-1-17ao)
    * [Transparência - Parte 2](https://dev.to/vaidehijoshi/transparency-illusions-of-a-single-system-part-2-lbb)












<!--

aula 1
* Área competitiva
* Computação distribuída é uma pedra fundamental
* Definição de Sistema Distribuído
* Tipos de Sistemas Distribuídos



## Aula 2: Fundamentos - Comunicação

Nesta aula nós relembraremos os fundamentos de redes de computadores e do protocolo IP, o substrato no qual sistemas distribuídos fracamente acoplados executam.

### Pontos Principais
* Modelos de Computação Distribuída
* Canais e protocolos de comunicação
* Sockets


### Leituras
* [Fundamentos](https://lasarojc.github.io/ds_notes/basics/)
* [Beej's Guide to Network Programming - Using Internet Sockets](https://beej.us/guide/bgnet/)
* Sistemas Distribuídos: Princípios e Paradigmas. Seção 4.1



## Aula 3: Laboratório de Sockets

Resolvamos os seguintes exercícios.

* Múltiplos Pacotes
* Ping-pong
* Ping-pong UDP
* IP-multicast

### Leituras
* [Fundamentos](https://lasarojc.github.io/ds_notes/basics/)
* [Beej's Guide to Network Programming - Using Internet Sockets](https://beej.us/guide/bgnet/)


## Aula 4: Fundamentos - Processos
Nesta aula discutiremos o papel da concorrência no desenvolvimento dos SD.


### Leituras
* [Fundamentos](https://lasarojc.github.io/ds_notes/basics/)
* Sistemas Distribuídos: Princípios e Paradigmas. Capítulo 3.



## Aula 5: Laboratório de *Multithreading*
Nesta aula discutiremos o papel dos processos no desenvolvimento de Sistemas distribuídos.

### Leituras
* Vídeo: Containers docker no desenvolvimento de aplicações distribuídas


## Aula 6: Arquiteturas
* Notas de aula: [Arquiteturas](https://lasarojc.github.io/ds_notes/intro/#arquiteturas)
* [Muitos nós, um sistema distribuído](https://dev.to/vaidehijoshi/many-nodes-one-distributed-system-kl9)
* [Diferenças entre sistemas centralizados, decentralizados e distribuídos](https://www.8bitmen.com/)
* Sistemas Distribuídos: Princípios e Paradigmas. Capítulo 2


## Aula 7: Arquiteturas - P2P
* Notas de aula: [Arquiteturas P2P](https://lasarojc.github.io/ds_notes/arch/#par-a-par-peer-to-peer-p2p)
* Sistemas Distribuídos: Princípios e Paradigmas. Capítulo 2


## Aula 8: Comunicação
* Middleware
* Transparência
* RPC

## Aula 9: Laboratório de RPC

## Aula 10: Comunicação orientada a mensagens
* MPI
* Filas de mensagens
* Publish Subscribe
    * MQTTP e Moquitto
* Protocolos epidêmicos

## Aula 11 - Coordenação: Exclusão mútua

## Aula 12 - Coordenação: Eleição de líderes

## Aula 13 e 14  - Atividade Assíncrona: computação em nuvem

Usando seu email institucional, inscreva-se no Coursera, no Curso "Cloud Computing Concepts, Part 1",  que faz parte da especialização "Cloud Computing".
Neste curso, você deverá fazer as 2 primeiras semanas, o que corresponde a 9 horas de trabalho.

## Aula 15 - Tempo físico e sincronização de relógios

* Tempo
* Relógios de Quartzo
* Relógios Atômicos
* Algoritmos de Sincronização
* NTP

## Aula 16 - Tempo lógico
* Relógios Lógicos
* Relógio de Lamport
* Relógio vetorial
* Ordenação total e causal

## Aula 17 - Tolerância a falhas
## Aula 18 - Tolerância a falhas
## Aula 19 - Tolerância a falhas
## Aula 20 - Tolerância a falhas
## Aula 21 - 
## Aula 22 - 
## Aula 23 - Bancos de dados
## Aula 24 - Bancos de dados
## Aula 25 - Sistemas de arquivos
## Aula 26 - Sistemas de arquivos
## Aula 27 - Tópicos avançados
## Aula 28 - Tópicos avançados
## Aula 29 - Seminários
## Aula 30 - Seminários

-->