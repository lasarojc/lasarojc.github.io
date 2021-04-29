# Sistemas Distribuídos


## Logística
Este material é comum para as duas disciplinas, isto é, GBC 074 (BCC) e GSI 028 (BSI) e este sítio é primeira fonte de informação sobre estas disciplinas.
A seguir, veja o plano de como nossa interação acontecerá. Para deixar bem claro,  isto é um plano, e planos podem ser alterados:


![Plano](images/plano.jpg)

### Aulas

Usaremos a ferramenta MS Teams (tm) para nossos encontros síncronos, atendimento a alunos e para comunicação em geral.
Após criar sua conta **usando o email da UFU**, cadastre-se na disciplina [aqui](https://teams.microsoft.com/l/team/19%3aaa949b16dda54fc8b612566bb652f888%40thread.tacv2/conversations?groupId=a430897a-9525-41ab-a06d-72e1137b3cde&tenantId=cd5e6d23-cb99-4189-88ab-1a9021a0c451). O código para aceite automático deve ter sido enviado para o seu email cadastrado no sistema da UFU.

#### Controle de Frequência

O **controle de frequência**  nas atividades será feito por chamadas usando questionários em momentos aleatórios da aula.
Isto é, apenas **estar logado não é garantia de que receberá presença**.

#### Programa

A disciplina abordará os tópicos definidos na ficha da disciplina, disponível no sítio do curso.
O plano da disciplina, aula-a-aula estará disponível na aba **Arquivos** no Teams.

#### Avaliação
Vocês serão avaliados de acordo com os critérios também disponíveis no plano.


### Seminários

Os alunos deverão apresentar seminários, desenvolvidos em grupos de $X$ alunos para seus colegas, onde $X$ será definido baseado na quantidade de matriculados.
O **objetivo** dos seminários é apresentar tópicos modernos relacionados à computação distribuída.

![Know your buzzwords](images/dilbert.jpeg)

A duração dos seminários será em torno de 40 minutos **de apresentação**.
Cada seminário será seguido por uma seção de perguntas e respostas de 10 minutos e de questionário **offline** desenvolvido pelos apresentadores.
Respeito ao tempo, tanto para mais quanto para menos, e qualidade do questionário são **critérios de avaliação**. Sua apresentação será avaliada nos seguintes pontos:

* Conteúdo: 
    * Contextualização
    * Importância para o profissional da área
    * Referencial teórico
    * Algo mais: discussão, vídeo, lab
* Postar vídeo da apresentação até a terça feira da última semana de aula. 
* Qualidade dos slides

Como sugestão inicial de temas, temos a seguinte lista, que pode ser expandida por sugestão dos alunos:

* Arquiteturas distribuídas reativas usando Kafka
   * Thiago Muniz
* Framework SpringBoot para Microsserviços
* [ELK - Elastic Search, Logstash, Kibana](https://www.elastic.co/what-is/elk-stack)
* Event Sourcing
* [O protocolo PBFT](https://medium.com/thundercore/consensus-series-pbft-3e011e7f3691)
* [Algorand](https://algorand.foundation/)
* [Dapr](https://docs.dapr.io)
* Kubernetes
* [Cache distribuído Redis](https://redislabs.com/solutions/use-cases/caching/)
* [Zipkin](https://zipkin.io/)
* [New Directions in Cloud Programming](http://cidrdb.org/cidr2021/papers/cidr2021_paper16.pdf)
* O protocolo [Hermes](https://hermes-protocol.com/)
* Se precisar de um tema, entre em contato. 

### Projeto

Os alunos desenvolverão um projeto seguindo uma intencionalmente vaga para exercitar sua capacidade de resolução de problemas usando os conceitos apresentados na disciplina.

* [Especificação](https://lasarojc.github.io/ds_notes/intro/#projeto/)
* Grupos dos trabalhos serão compostos por 6 alunos.
   * Não, não pode ter mais de 6.
   * Pode ter menos, mas não recomendo, pois o trabalho dá trabalho.
   * Podem misturar BCC e BSI se facilitar.
   * Quem ficar sem grupo, forme um grupo. Podem usar este chat aqui para se encontrarem.






## Aula 1: Apresentação e Introdução
Nesta aula apresentarei uma visão geral e rápida dos sistemas distribuídos e espero que os motive ao estudo dos mesmos.

### Pontos principais
* Área competitiva
* Computação distribuída é uma pedra fundamental
* Definição de Sistema Distribuído
* Tipos de Sistemas Distribuídos


### Leituras
* Notas de aula: [Prefácio](https://lasarojc.github.io/ds_notes/)
* Notas de aula: [Introdução](https://lasarojc.github.io/ds_notes/intro/)
* Sistemas Distribuídos: Princípios e Paradigmas. Capitulo 1.
* [Difference Between Centralized, Decentralized & Distributed Systems Oversimplified](https://www.8bitmen.com/difference-between-centralized-decentralized-distributed-systems-explained/)
* [Transparência - Parte 1](https://dev.to/vaidehijoshi/transparency-illusions-of-a-single-system-part-1-17ao)
* [Transparência - Parte 2](https://dev.to/vaidehijoshi/transparency-illusions-of-a-single-system-part-2-lbb)


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

