# 💼 Contratos de Exemplo: A Engenharia Reversa (Roadmap)

A melhor forma de dominar a engenharia dos Smart Contracts é realizando **engenharia reversa** em códigos já testados em batalha. A equipe da Stellar reuniu um arsenal de contratos de exemplo (`soroban-examples`), e a ordem em que você os estuda importa.

Você não começa construindo um Liquidity Pool. Você começa armazenando um número. Siga este roteiro progressivo para treinar:

## Categoria 1: O Recruta (Fundamentos)
Aqui você aprende a respirar dentro do Soroban.
1. **Storage:** Armazenar dados permanentemente (ex: incrementar um contador).
2. **Events:** Como disparar eventos para que suas Aplicações (Frontends) saibam que algo aconteceu on-chain.
3. **Errors & Logging:** Emitir erros nativos do contrato e debugar através de logs.
4. **Custom Types:** Estruturar e organizar seus próprios tipos de dados customizados dentro do contrato.

## Categoria 2: O Operador Tático (Contas e Autenticação)
Sem segurança, seu contrato é um vazamento de fundos esperando para acontecer.
1. **Auth:** O básico da segurança. Como exigir que o usuário X aprove a transação antes que o contrato mova o fundo Y.
2. **Simple Account & Complex Account:** Contratos que agem como carteiras. Do básico com uma chave `ed25519` até multi-assinaturas e políticas avançadas de autorização.
3. **Cross Contract Calls:** Invocando as funções de *outro* contrato, direto do seu contrato.

## Categoria 3: O Engenheiro Financeiro (DeFi e Tokens)
Onde a revolução financeira acontece de verdade.
1. **Atomic Swap & Batched Swaps:** Trocas atômicas perfeitas entre usuários. Ou tudo acontece junto (a troca de tokens), ou nada acontece.
2. **Tokens (Fungible & NFT):** Contratos criados e auditados pela OpenZeppelin para criar tokens fungíveis e não fungíveis seguros e padronizados.
3. **Liquidity Pool:** A construção bruta de uma pool de liquidez baseada na matemática de produto constante (x * y = k).
4. **Upgradeable Contract:** A habilidade extrema de atualizar o *bytecode* (código compilado) de um contrato que já está implementado na rede principal.

> 🛠️ **Missão:** Não copie e cole às cegas. Abra a [documentação oficial de exemplos](https://developers.stellar.org/docs/build/smart-contracts/example-contracts), analise o repositório, faça um clone local, olhe os testes de cada contrato (eles possuem TDD embutido) e altere a lógica de armazenamento ou autorização para ver o que quebra.

*Esta é a reta final da Fase teórica pesada. Se você leu e testou os contratos acima, você está pronto para invadir o campo de batalha de cabeça.*
