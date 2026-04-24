# 🦀 Instalação do Rust

Os *smart contracts* da rede Stellar são pequenos programas escritos na linguagem de programação **Rust**. 
Para construir e desenvolver esses contratos, precisamos do compilador Rust atualizado.

## Instalando o Rustup (macOS / Linux / WSL)

A maneira mais simples de instalar a toolchain do Rust é via `rustup`. Rode o comando abaixo em seu terminal:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Após a instalação, **reinicie o seu terminal** ou rode `source ~/.cargo/env`.

> [!IMPORTANT]
> Os contratos inteligentes da Stellar exigem a versão **v1.84.0 ou superior** do Rust, pois o target que utilizaremos (`wasm32v1-none`) só está disponível nas versões recentes.

Para verificar a versão instalada:
```bash
rustc --version
```

Caso precise atualizar uma instalação existente:
```bash
rustup update stable
```

## Instalando o Target WebAssembly (Wasm)

Você precisará instalar um "target" (alvo de compilação) específico para que seu contrato inteligente seja compilado corretamente para a infraestrutura da Stellar. 

Instale o target `wasm32v1-none`:
```bash
rustup target add wasm32v1-none
```

> [!NOTE]
> Quando você instala o Rust, os targets do WebAssembly são instalados por *toolchain*. Isso significa que se você atualizar a sua versão do Rust no futuro, precisará rodar este comando novamente para instalar o target na nova versão.
