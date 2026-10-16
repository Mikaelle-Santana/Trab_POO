# Ryusei Cafe ☕

Este repositório contém o sistema de um mangá café desenvolvido em Java para a disciplina de Programação Orientada a Objetos.

O projeto foi organizado de forma modular, dividindo as responsabilidades entre diferentes "trabalhos" (pacotes). Abaixo você encontra uma visão geral de cada módulo que compõe o sistema:

## 📁 Estrutura do Projeto

O código-fonte está localizado na pasta `src/`, organizada nos seguintes módulos:

*   [**`gui/` (Interface Gráfica)**](./src/gui/README.md): Contém a aplicação principal desenvolvida utilizando a biblioteca Swing. Fornece uma interface rica e intuitiva para gerenciar vendas, estoque, clientes e funcionários.
*   [**`cli/` (Linha de Comando)**](./src/cli/README.md): Contém uma versão do sistema baseada em terminal (CLI), oferecendo os mesmos recursos através de menus de texto interativos.
*   [**`pessoa/` (Gestão de Pessoas)**](./src/pessoa/README.md): Módulo que define as entidades de usuários e funcionários do café.
*   [**`funcoes_auxiliares/` (Lógica de Negócios e Utilitários)**](./src/funcoes_auxiliares/README.md): Núcleo do sistema, contendo o gerenciamento de carrinho de compras, pagamentos, itens do menu, mangás e o sistema de busca.

## 🚀 Como Executar

Você pode escolher entre rodar a versão com interface gráfica ou a versão via terminal.

### Pré-requisitos
*   Java Development Kit (JDK) instalado.

### Compilando o projeto

Para compilar todo o projeto de uma vez, execute o seguinte comando na raiz do repositório:
```bash
javac -d bin src/**/*.java
```
Isso criará os arquivos compilados (`.class`) dentro da pasta `bin/`.

### Rodando a versão GUI
```bash
java -cp bin gui.RyuseiCafeGUI
```

### Rodando a versão CLI (Terminal)
```bash
java -cp bin cli.ryusei_cafe
```