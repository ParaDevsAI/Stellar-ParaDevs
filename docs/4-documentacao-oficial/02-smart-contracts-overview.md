# 🧠 Smart Contracts: A Máquina por Trás do Soroban

Entrar no Soroban é como pilotar um jato militar: você tem muita potência, mas o painel de controle tem regras estritas para que você não caia. Soroban **não é** uma nova blockchain, mas sim uma plataforma de smart contracts perfeitamente acoplada à blockchain Stellar que você já conhece.

## O Dialeto Rust (Rust Dialect)

Se você já conhece Rust, ótimo. Mas atenção: **Smart Contracts na Stellar não usam o pacote completo do Rust.**

* O ambiente tem restrições pesadas de limites de recursos e segurança.
* A **Standard Library (std)** do Rust tradicional e a maioria das *crates* (bibliotecas de terceiros) **não** estão disponíveis direto da prateleira.
* **A Arma Secreta:** O **Soroban Rust SDK**. Ele atua como o substituto da standard library, dando acesso a hashes criptográficos, verificação de assinaturas, storage persistente e invocação de outros contratos.

## O Host Environment (A Arena de Batalha)

O seu código compilado em Wasm não roda no vácuo. Ele é executado pelo **Host Environment**, que vive dentro do `stellar-core`.
O Host gerencia:
* As funções e objetos do ambiente
* O armazenamento on-chain (acessos de leitura e escrita)
* A contabilidade pesada: quem paga quanto de taxa (fees)

## FAQs Táticas - Respostas Diretas

1. **Como invoco um contrato?**
   Você não manda um email. Você envia uma transação comum da Stellar contendo a operação `InvokeHostFunctionOp`.
   
2. **Posso usar minhas contas antigas da Stellar?**
   **SIM**. Contas da Stellar (aquelas com chave G...) são 100% integradas. Os contratos conseguem ler as assinaturas e a origem de quem invocou a transação.

3. **E os tokens clássicos da Stellar?**
   A integração é nativa. O Soroban possui um **Stellar Asset Contract** embutido. Se você enviar um ativo clássico para um contrato, o emissor original *mantém* as configurações de autorização (como Clawback, se configurado).

4. **Taxas e Reservas Base?**
   Smart contracts usam uma estrutura de taxas separada e possuem um sistema de "metering" (medição de uso de cpu/memória). A reserva base da Stellar (base reserve) clássica não se aplica à alocação de armazenamento dos contratos.

---
**Próximo Passo no Roadmap:** Você conhece o motor. Agora é hora de ver como os [Exemplos de Contratos](03-example-contracts.md) são montados na prática.
