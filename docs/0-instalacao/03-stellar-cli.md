# 🚀 Instalando a Stellar CLI

A **Stellar CLI** é o seu canivete suíço. Ela pode executar comandos, gerenciar identidades, formatar redes e compilar/executar contratos inteligentes na rede *futurenet*, *testnet*, *mainnet* e também em um *sandbox* local para testes.

*Repositório Oficial:* [stellar-cli](https://github.com/stellar/stellar-cli)
*Documentação Oficial:* [Stellar Docs](https://developers.stellar.org/docs/build/smart-contracts/getting-started/setup)

## Instalação Rápida (macOS e Linux/WSL)

A versão estável recomendada é a **v26.0.0**.

**Opção 1: Via Script Direto**
```bash
curl -fsSL https://github.com/stellar/stellar-cli/raw/main/install.sh | sh
```

**Opção 2: Via Homebrew (macOS/Linux)**
```bash
brew install stellar-cli
```

**Opção 3: Compilando via Cargo (Do código fonte)**
Se preferir, ou se estiver utilizando Windows sem WSL, você pode instalar através do gerenciador de pacotes do próprio Rust:
```bash
cargo install --locked stellar-cli@26.0.0
```

---

## ⚡ Habilitando Autocompletar (O Superpoder)

Você pode usar o recurso de `completion` da Stellar CLI para ter sugestões diretamente no seu terminal quando pressionar `TAB`. Isso acelera imensamente a velocidade do seu desenvolvimento.

Para habilitar na sessão atual do seu terminal (Bash):
```bash
source <(stellar completion --shell bash)
```

Para habilitar permanentemente no **Bash** (para Linux/WSL), rode o comando abaixo e reinicie seu terminal:
```bash
echo "source <(stellar completion --shell bash)" >> ~/.bashrc
```

*(Se utilizar `ZSH`, substitua `bash` por `zsh` e `~/.bashrc` por `~/.zshrc`)*
