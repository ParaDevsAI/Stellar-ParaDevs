# 🌟 Learning The Consensus Mechanism: SCP & PoA

*O Protocolo de Consenso Estelar (SCP) fornece uma maneira de chegar a um consenso sem depender de um sistema fechado para registrar com precisão as transações financeiras.*

## Prova de Acordo (PoA - Proof of Agreement)

A **Prova de Acordo (PoA)** descreve o mecanismo de consenso **SCP (Stellar Consensus Protocol)** usado pela rede Stellar. 
O PoA é uma alternativa muito mais eficiente para blockchains mais antigos que exigem soluções de força bruta para problemas de matemática difíceis e a energia para executar e resfriar pilhas maciças de hardware (PoW). 

Em vez disso, o PoA permite blockchains não baseados em mineração, que alcançam consenso por meio de uma série muito rápida de mensagens entre os participantes para confirmar as transações e finalizá-las no livro-razão.

## A Rede Stellar

A rede Stellar é uma blockchain pública de código aberto alimentada pelo protocolo SCP. Graças ao PoA, a rede Stellar é mais rápida, mais barata e muito mais eficiente em termos energéticos do que muitas outras blockchains. 
As transações são finalizadas e adicionadas à blockchain uma vez que são acordadas por computadores chamados "nós" (nodes).

* Qualquer pessoa pode configurar um nó Stellar e participar, fornecendo suas informações de identificação no registro público. 
* Dessa forma, outros nós podem decidir em quem incluir (ou excluir) de seu grupo de confiança. 
* SCP ganha Prova de Acordo sobre quais transações são adicionadas através de um processo de votação por esses nós mutuamente confiáveis. 
* Quando nós suficientes em seus grupos de sobreposição confiáveis (chamados de **quórum**) concordam que um conjunto de transações e os ativos nele são válidos, ele será permanentemente adicionado. Todo esse processo geralmente leva cerca de **5 segundos**.

## Como funciona o Consenso Stellar (SCP)?

O sistema de confiança opera baseado em **Quorum Sets** e **Quorum Slices**.

Exemplo: Se um "Estudante A" tem três outros alunos (1, 2, 3) em seu *Quorum Set* e a sua regra de validação requer que pelo menos 2 deles concordem para considerar uma transação como verdadeira, o "Estudante A" tem 3 *Quorum Slices* resultantes (combinações de confiança suficientes para formar um quórum localizado). 
