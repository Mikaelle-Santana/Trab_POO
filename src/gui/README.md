# Módulo GUI (Interface Gráfica) 🎨

Este módulo provê a interface visual do sistema **Ryusei Cafe**, construída utilizando a biblioteca **Java Swing**.

A classe `RyuseiCafeGUI.java` é o ponto de entrada deste módulo. Em vez de menus de texto, o usuário interage com janelas, botões, tabelas de dados e painéis estruturados de forma clara e moderna.

## Estrutura da Interface

A interface é dividida em diferentes telas ("cards"), facilmente navegáveis por um menu lateral:

*   **Módulo de Vendas**: Tela que concentra o atendimento aos clientes. É possível buscar um cliente por CPF, ver os detalhes de sua assinatura, adicionar itens ao carrinho através de um campo de busca inteligente e finalizar pagamentos com diferentes métodos.
*   **Módulo de Estoque**: Painel completo para gerenciamento do inventário do café. Apresenta uma tabela unificada com mangás e itens do menu. Além de permitir atualizar rapidamente o estoque de itens já cadastrados, possui formulários detalhados para o cadastro de novos mangás (volume, série, localização, autores) e novos itens de cardápio (preço, ingredientes).
*   **Módulo de Pessoas (Clientes e Funcionários)**: Interfaces focadas no cadastro e visualização tabular de todos os usuários do café, bem como a equipe de funcionários, seus cargos e salários.
*   **Módulo de Pagamentos**: Permite visualizar de forma clara o histórico de transações e vendas já efetuadas.

## Detalhes de Implementação

O uso de componentes Swing como `CardLayout`, `GridBagLayout` e `JTable` garantiu que o sistema apresentasse informações complexas de forma organizada e escalável. Mensagens de erro e confirmação são feitas de forma amigável através de `JOptionPane`.
