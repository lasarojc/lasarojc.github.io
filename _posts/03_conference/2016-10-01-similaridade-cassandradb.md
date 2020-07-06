---
layout: post
categories:
 - Publications

title: Busca por Similaridade no CassandraDB
author: Antonio Mourão, Rafael Pasquini, Rodolfo Villaça, Lásaro Camargos
venue: 31st Brazilian Symposium on Databases
paper: https://www.researchgate.net/publication/309121006_Busca_por_Similaridade_no_CassandraDB 
type: Peer-reviewed Conference


---
Abstract: The need for scalability in the Big Data era has lead to flourishing of distributed NOSQL systems. However, none of the widely used solutions available support similarity searches, another important feature in such scenarios. Here we propose to overcome this limitation by extending Cassandra with similarity search capabilities. Our approach is based on using locality sensitive hashing to spread data to nodes, to target nodes for queries, and for efficiently recovering similar data from stable storage at the nodes. We overview how to implement the approach, our test plan, and initial results. Resumo. A necessidade de escalabilidade em cenários de Big Data levou à prosperação dos NOSQL distribuídos. Contudo, as soluções mais amplamente usadas não suportam uma outra característica desejável, busca por similari-dade. Neste artigo propomos contornar tal limitação estendendo o Cassandra com suporte a buscas por dados similares. Nossa abordagem usa hashing sensí-vel à localidade para distribuir dados entre nós, direcionar buscas, e recuperar dados em armazenamento estável de forma eficiente. Descrevemos aqui como implementar esta abordagem, nosso plano de testes e resultados iniciais. 1. Introdução Cassandra [Lakshman and Malik 2010] é um banco de dados NOSQL (Not Only SQL) amplamente utilizado em cenários BigData devido à sua escalabilidade horizontal. Como em outros NOSQL [Decandia et al. 2007, Chang et al. 2008], essa característica vem do consistent hashing, particionamento aleatório dos dados entre os nós do sistema que dis-tribui a carga uniformemente entre os mesmos e facilita sua entrada e saída do sistema [Stoica et al. 2001]. Apesar das vantagens, essa distribuição dificulta a busca por dados similares, outra característica desejável em BigData. Dois objetos de um mesmo domínio são similares se seus atributos possuem um grau de semelhança elevado; caso contrário são dissimilares. A busca por similaridade consiste em recuperar objetos que sejam similares aos parâmetros da consulta. Alguns exemplos incluem a identificação de perfis de clientes com hábitos de consumo parecidos e de imagens com o mesmo tema. Dentre alguns esforços para se melhorar a busca por similaridade nestes sistemas, destacamos a HammingDHT [Villaca et al. 2013]. Na HammingDHT, a chave de cada objeto é construída por uma função de espa-lhamento sensível a localidade (LSH), que gera chaves similares para dados similares e * Agradecimentos à CAPES, CNPq, FAPEMIG e FAPES pelo apoio à realização deste trabalho.


 
