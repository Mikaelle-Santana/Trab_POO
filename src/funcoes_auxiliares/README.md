# Funções Auxiliares e Regras de Negócio ⚙️

O pacote `funcoes_auxiliares` atua como o motor do sistema Ryusei Cafe. Ele agrupa a lógica principal de vendas, gerenciamento de estoque, modelos de itens e serviços, assim como a busca de dados.

## Principais Componentes

*   **`SistemaDeBusca`**: O "coração" operacional da aplicação. Gerencia as listas globais de usuários, funcionários, mangás, pagamentos e o menu. É responsável pelas funções C.R.U.D e pela conversão de todos os dados do programa em persistência física (lendo e escrevendo os arquivos `.csv`).
*   **`Vendivel`**: Uma estrutura polimórfica crucial no sistema, criada para unificar diferentes tipos de mercadorias em transações.
*   **`Manga`**: Representa os livros do acervo do café. Armazena dados complexos como os autores, gêneros, série, número do volume e a sua localização na estante, além das informações de custo.
*   **`Item_menu`**: Representa pratos, lanches ou bebidas oferecidos. Mantém a relação de ingredientes, preços e estoque.
*   **`Carrinho_de_compras`**: Modela a sessão de consumo de um cliente. Permite adicionar instâncias de `Vendivel` (seja um mangá ou um café), calcular o valor total em tempo real e atualizar os estoques no banco de dados, caso a venda seja concretizada.
*   **`Pagamento`**: Registra cada transação, associando o método de pagamento (Cartão, Pix, Dinheiro), o valor final, a data, o status e o cliente envolvido (via CPF).

Este módulo assegura que tanto a Interface Gráfica (`gui`) quanto a Linha de Comando (`cli`) consigam consumir regras de negócios perfeitamente encapsuladas sem a necessidade de duplicar lógicas ou manipular as classes de forma indevida.
