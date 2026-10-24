# WordCount CLI - Contagem de Palavras em PDF

[![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)](https://www.rust-lang.org/) [![Cargo](https://img.shields.io/badge/Cargo-f5F5F5?style=for-the-badge&logo=cargo&logoColor=black)](https://crates.io/) [![clap](https://img.shields.io/crates/v/clap?style=for-the-badge)](https://crates.io/crates/clap) [![pdf_extract](https://img.shields.io/crates/v/pdf_extract?style=for-the-badge)](https://crates.io/crates/pdf_extract) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

Seja bem-vindo! Este repositório contém o **WordCount CLI**, uma ferramenta de linha de comando desenvolvida em **Rust** para extrair texto de arquivos PDF e exibir as palavras mais frequentes de maneira rápida e eficiente.

---

## 📌 Visão Geral

O **WordCount CLI** permite:

- Verificar se o arquivo PDF informado existe.
- Extrair texto do PDF utilizando a crate `pdf_extract`.
- Limpar o texto (converter para minúsculas e remover caracteres não alfabéticos).
- Contar a frequência de cada palavra.
- Exibir as **10** palavras mais frequentes por padrão.

---

## 🛠️ Tecnologias Utilizadas

- **Rust**
- **clap** para parsing de argumentos de linha de comando
- **pdf_extract** para extração de texto de arquivos PDF
- **std** (`std::path`, `std::collections::HashMap`, entre outros)

---

## 🚀 Funcionalidades

- Checagem de existência do arquivo PDF.
- Tratamento de erros com mensagens claras.
- Extração e limpeza de texto para análise precisa.
- Contagem e ordenação das palavras mais frequentes.
- Saída no terminal com formato legível.

---

## 📦 Como Compilar e Executar

### Pré-requisitos

- [Rust e Cargo](https://www.rust-lang.org/tools/install) instalados em sua máquina.

### Compilando

No diretório raiz do projeto, execute:

```bash
cargo build --release
```

O binário compilado ficará disponível em `target/release/wordcount`.

### Instalando via Cargo

Para instalar globalmente:

```bash
cargo install --path .
```

### Executando

```bash
wordcount --file path/para/seu_arquivo.pdf
```

Você verá no terminal algo como:

```
Processing file: seu_arquivo.pdf
Top 10 most frequent words:
exemplo - 42x
rust - 37x
...
```


