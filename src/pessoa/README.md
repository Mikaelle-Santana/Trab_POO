# Módulo de Pessoas 👥

Este pacote gerencia as entidades humanas que interagem com o Ryusei Cafe, estabelecendo as relações e os dados fundamentais para o funcionamento do negócio.

## Classes Principais

*   **`Pessoa`**: É a classe base (superclasse) que abstrai os dados comuns de todos os indivíduos do sistema. Armazena informações essenciais como:
    *   Nome
    *   CPF
    *   Telefone
    *   Email
*   **`Usuario`**: Classe que representa um cliente do café. Estende de `Pessoa` e introduz conceitos de negócio voltados aos consumidores, como o tipo de **assinatura**. No contexto do mangá café, a assinatura pode garantir benefícios e ditar as regras de aluguel ou tempo de permanência.
*   **`Funcionario`**: Outra ramificação da classe `Pessoa`, responsável por gerenciar quem trabalha no local. Contém dados trabalhistas como **cargo** (ex: Atendente, Gerente) e **salário**.

## Papel no Sistema
A organização em herança destas classes permite polimorfismo em partes do sistema (como ao buscar qualquer "Pessoa" pelo CPF) e centraliza os dados sensíveis da aplicação de forma bem estruturada, facilitando a exportação e o carregamento a partir de arquivos `.csv`.
