# Módulo CLI (Linha de Comando) 💻

Este módulo é responsável por prover uma interface interativa de terminal para o sistema do **Ryusei Cafe**. 

A classe `ryusei_cafe.java` funciona como o ponto de entrada (método `main`) para os usuários que preferem ou necessitam utilizar o sistema via console.

## Funcionalidades
Ao rodar a aplicação, o sistema exibe um menu em texto com as seguintes opções de gerenciamento:

*   **Gestão de Pessoas**: Adicionar ou buscar clientes e funcionários no sistema.
*   **Gestão de Mangás**: Consultar mangás disponíveis no acervo e atualizar a quantidade de estoque.
*   **Gestão do Menu**: Consultar pratos e bebidas, adicionar novos itens ou renovar o estoque.
*   **Módulo de Compras**: Um fluxo passo-a-passo no terminal para identificar o cliente por CPF, adicionar mangás e itens de menu ao carrinho e, por fim, efetuar o pagamento.
*   **Persistência**: O sistema cuida de ler os dados de arquivos `.csv` na inicialização e salvá-los corretamente antes de ser encerrado.

## Como utilizar

Toda a interação é feita através da entrada padrão (`Scanner`). Basta ler as opções na tela e digitar o número correspondente à ação desejada. O programa informará caso haja erros de validação (como buscar um mangá que não existe ou tentar realizar o pagamento com o carrinho vazio).
