---
layout: notes
title: "Aula 3 - Logística e Introdução"
part: 1 Introdução
---

# Projetos

A ideia do estudo orientado a projetos é sedimentar os conceitos vistos em aula teórica pela prática.
Cada grupo de alunos definirá o seu próprio projeto, dentro de certos de limites e de forma a exercitar os conceitos aprendidos.
Todo requisito do trabalho deve ser demonstrado na apresentação, feita diretamente a mim.

* Projeto: 
  * Entregas por repositório **Github público** até 23:59 da data da entrega.
  * A cada dia de atraso, o valor total do trabalho sofrerá 3% de desconto.
  * Após uma semana, o trabalho não pode ser mais entregue.
  * Todos os membros do grupo deverão estar aptos a apresentar o trabalho.
  * A qualidade do código será julgada.
  * Qualquer linguagem suportada por gRPC pode ser utilizada.
  * Relatório indicando todos os passos para se clonar o código, compilá-lo, executá-lo e testá-lo.
  * Todas as dependências devem ser baixadas automaticamente durante a compilação (sugestão, usar maven).
  * Entrega 0
    * Formalização do projeto
      * Descrição suscinta do serviço a ser implementado para a primeira entrega, incluindo os componentes que você jé vê como os grandes blocos da sua arquitetura (client, applicativo, servidor...).
    * Individual - Alguns destes projetos serão descartados para a segunda entrega.
    * Lista de testes a serem implementados. Algumas sugestões são: 
      * teste de concorrência: demonstrando que múltiplos clientes podem acessar o serviço ao mesmo tempo, sem comportamentos estranhos.
      * teste de recuperação de falhas: quando um componente falha e volta a executar, ele não leva o sistema a nenhum estado inesperado.
      * demonstração de funcionalidades: mostre que as funcionalidades estão implementadas, por exemplo, se seu sistema é um banco de dados, demonstre CRUD dos dados..
  * Entrega 1
    * Seu projeto foi combinado com o professor e ajustes foram feitos. Você deverá agora implementá-lo.
    * Trabalho em grupos de 4 alunos.
    * Escolham um dos trabalhos da entrega 0 dos membros do grupo para construir o trabalho 1.
    * Elementos mínimos de todos os projetos:
      * Cliente TCP/IP ou UDP/IP: executa operações interativamente e sem erros; não recria sockets desnecessariamente.
      * Cliente TCP/IP ou UDP/IP para testes automatizados: executa baterias de testes; reporta testes falhos e bem sucedidos; simula múltiplos clientes concorrentes.
      * Servidor TCP/IP ou UPD: serve requisições concorrentes de múltiplos clientes;
        * O servidor deve manter alguma forma de estado acessado concorrentemente pelos clientes.
        * Controle de concorrência nos clientes deverá ser implementado.
        * Em caso de reinicializações, recupera o estado anterior;
      * Execução em mais de uma máquina.
      * Codificação de dados deve usar constantes pré-definidas e com mnemônicos, isto é, nada de mandar 1 para Criar e 2 para Apagar, mas CRIAR e APAGAR.
  * Entrega 2
    * Toda a comunicação deverá ser substituída por gRPC;
    * Toda operação a ser executada no servidor deve ser definida pela função, não por parâmetro (por exemplo, use funções "somar" e "subtrair", não uma única função "calcular" com parâmetro indicando se é para somar ou subtrair);
    * O estado armazenado no servidor deve ser composto por log + snapshots dos dados, como visto na aula [sobre estruturas de dados para sistemas distribuídos](https://lasarojc.github.io/ds_notes/notes/p2p/2_ed_sd.html);
      * Assuma que todos os dados cabem em memória e portanto em uma única sstable, isto é, sstables são snapshots da memória;
      * Não é necessário implementar compactação;
      * Escreva um texto de até uma página explicando como e porquê *Log Structured Merge Trees* seriam usadas no projeto;
    * Outros elements dependerão de cada trabalho, com duas opções:
      * O serviço será particionado usando *consistent hashing*;
        * O roteamento entre pares é feito via *finger table*;
          * Qualquer nó pode receber requisições dos clientes e é capaz de encaminhá-las para o nó correto;
          * Pode assumir que o conjunto de nós é conhecido e estático;
          * Todos os processos que param de funcionar voltam ao normal depois de um tempo;
          * Não há pontos únicos de falha no sistema (processos que se falharem paralisam todo o sistema);
        * Os dados são particionados usando alguma chave que os identifique;
          * A chave externa depende da aplicação;
          * A chave interna tem um espaço significativo, por exemplo, $2^160$ possíveis valores;
          * A distribuição de carga entre os nós é uniforme;
        * No caso de reinicialização de algum servidor, sua recuperação é baseada nos snapshots e logs;
      * O serviço será particionado usando microsserviços;
        * Vários microsserviços são usados para decompor funcionalmente o sistema;
        * Os dados são roteados segundo alguma tabela pré-configurada associando função a microsserviço;
  * Entrega 3
    * Trabalho em grupos de 4 alunos; o mesmo do trabalho anterior.
    * O serviço será replicado e a comunicação poderá ser substituída por um método adequado.
    * Será usada um implementação do Raft, do Paxos, ou do barramento Kafka para dar confiabilidade à comunicação.
    * Outros detalhes serão definidos em tempo.


Laboratórios serão usados para exemplificar o uso de tecnologias. *A priori*, executar o laboratório não vale nota, mas a quizes e exercícios poderão ser atribuídos nota de participação. Além disso, são uma "mão na roda" para ajudar a fazer os trabalhos.

Os alunos também farão seminários sobre tópicos "quentes" na computação distribuída.
* 6 Seminários
* Grupos de 1/6 da turma
* Conteúdo:
  * Histórico/Motivação da tecnologia.
  * Como funciona?
  * Tutorial/Exemplo em vídeo ou laboratório prático
  * Questionário com 3 perguntas de múltiplas alternativas, impressas, e entregues para os alunos responderem.
    * Nada de NDA ou todas as anteriores, ou V/F.
  * 50 Minutos no total
* Exemplos
  * Kafka
  * Kubernetes
  * AWS Cloudformation
  * O uso de RUST para programação distribuída.
  * ...

# Notas

Os projetos equivalerão a 70% da nota, sendo
* Entrega 0: 5%
* Entrega 1: 15
* Entrega 2: 20
* Entrega 3: 30

Seminários equivalerão a 20% da nota.

Finalmente, a quizes, dinâmicas e testes surpresa, serão atribuídos até 20% da nota.

# Atendimento

* Piazza: \url{piazza.com/ufu.br/semester22019/gbc074gsi028}
* TODA COMUNICAÇÃO deve ser iniciada via Piazza.
* Atendimento presencial
  * Agendado via Piazza
  * Sala 1b149
  * Seg. 10:30 e 19:00


# Visão geral dos sistemas distribuídos

Voltemos à nossa visão geral de Sistemas Distribuídos, para entendermos o que é um sistema distribuído e quais dificuldades encontraremos ([O quê?](https://lasarojc.github.io/ds_notes/notes/intro/2_oque.html). 


