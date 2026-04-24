# 🔒 How Crypto Hashing Works to Ensure Immutability

*Entendendo hashing e seus mecanismos para garantir confiabilidade e imutabilidade de dados em Blockchain*

O processo de hashing converte uma informação ("Plain Text") através de um algoritmo seguro (como o `SHA-256`, uma função de hashing popular em tecnologia blockchain) para produzir um "Hash" exclusivo. 

```text
Plain Text ("Hello world") -> [ SHA-256 ] -> "07e42324292ec3bfc15095890983459647898784768yec394885839475837485..."
```

## O Processo de Hash na Blockchain (Blockchain Hash Process)

Cada bloco de dados encadeado possui a seguinte estrutura de integridade:
* **Header** (Cabeçalho)
* **Previous Hash** (Hash do bloco anterior, garantindo a ligação)
* **Meta-Data** (Metadados do bloco)
* **TX Data Hash** (Hash representando os dados da transação atual)
* **Transaction Data** (Os dados das transações validadas)

Qualquer alteração minúscula em *Transaction Data* alteraria o *TX Data Hash*, que consequentemente alteraria o *Hash* do bloco inteiro, quebrando a corrente de *Previous Hash* dos blocos subsequentes e tornando a adulteração imediatamente detectável.
