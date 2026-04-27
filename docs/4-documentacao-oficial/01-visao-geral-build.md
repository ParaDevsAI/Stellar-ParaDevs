# 🏗️ Construindo na Stellar: Visão Geral

Seja muito bem-vindo ao arsenal de construção da Stellar! O ecossistema oficial da Stellar é dividido em três grandes pilares quando o assunto é o "Build" (construção). Entender essas três frentes é o primeiro passo para arquitetar sistemas imbatíveis.

## 1. Smart Contracts (Soroban)
Os contratos inteligentes na Stellar utilizam a plataforma **Soroban**. Eles são programas auto-executáveis com regras enraizadas direto no código.
* **Características:** São escritos na linguagem **Rust** e compilados em **WebAssembly (Wasm)** antes de irem para a blockchain.
* **Foco:** Esta é a lógica de backend. Aqui você lida com as regras de negócio implacáveis, controle de acesso e segurança para evitar vulnerabilidades.

## 2. Applications (Aplicações)
As aplicações são a ponte entre o usuário final e a blockchain. Elas fornecem a interface de usuário (UI) e a gestão das interações.
* **O que fazem:** Elas se conectam aos seus Smart Contracts (ou diretamente à Stellar) para submeter transações, gerenciar chaves (wallets) e orquestrar a UX.
* **Detalhe tático:** Você pode construir aplicações poderosas na Stellar *mesmo sem* usar um Smart Contract (como plataformas de pagamento direto via SDK).

## 3. How-To Guides (Guias Práticos)
Quando você precisa implementar algo muito específico, os Guias Práticos da documentação oficial salvam a sua vida. Eles cobrem:
* Controle e Autorização de Contratos
* Gestão de Contas (Contract Accounts)
* Armazenamento (Storage) nativo
* Taxas e Metrificações (Fees & Metering)

> ⚠️ **Tática de Guerra:** Não tente reinventar a roda. Antes de construir um sistema complexo de armazenamento no seu contrato, verifique as *Security Best Practices* e os *How-To Guides* oficiais da Stellar. A segurança do seu projeto agradece.

---
**Próximo Passo no Roadmap:** Mova-se para a [Visão Geral dos Smart Contracts](02-smart-contracts-overview.md) e entenda as regras do jogo no ambiente do Rust.
