# Grande Banco - Sistema de Operações Financeiras (v1)
Este projeto consiste na implementação de um sistema básico de operações bancárias (depósito, saque e extrato) utilizando a linguagem Python. O desafio foi proposto com o objetivo de simular um cenário real de desenvolvimento para um banco que busca modernizar suas plataformas, oferecendo uma solução simples e eficiente para a gestão de transações financeiras.

## Objetivo
O objetivo principal foi desenvolver uma aplicação console em Python capaz de gerenciar três operações fundamentais em uma conta bancária: depósito, saque e extrato. A meta era criar uma interface intuitiva para o usuário, ao mesmo tempo em que se aplicavam regras de negócio específicas para garantir a segurança e a consistência das transações.

## Regras a Serem Seguidas
O sistema foi desenvolvido seguindo um conjunto de regras predefinidas para cada operação:

- Depósito: Apenas valores positivos são aceitos. O valor depositado é adicionado ao saldo da conta.

- Saque: Foram estabelecidas três restrições principais:
  - O valor do saque não pode exceder o saldo disponível.
  - O valor máximo por saque é de R$ 500,00.
  - O limite diário é de 3 saques.

- Extrato: O extrato apresenta um histórico de todas as operações realizadas (saque e depósito), além de exibir o saldo atual da conta e o resumo das transações (quantidade de saques/depósitos e seus respectivos totais).

## Metodologia
A implementação foi realizada em Python, utilizando uma abordagem procedural para a lógica do programa. O desenvolvimento seguiu os seguintes passos:

- Estrutura de Dados: Utilização de variáveis para armazenar o saldo e o histórico de transações, como saques, depositos e a quantidade de saques e depósitos realizados. Um dicionário (extrato_historico) foi empregado para registrar cada operação, permitindo o armazenamento de pares chave:valor (ex: Operação 1: ['Saque', 100]), facilitando a exibição detalhada no extrato.

- Interface com o Usuário: O sistema interage com o usuário por meio do terminal, utilizando a função input() para capturar a escolha da operação e os valores das transações. A interface foi projetada para ser clara e informativa, com mensagens de feedback para cada ação.

- Lógica de Controle: Um laço de repetição while foi implementado para manter o programa em execução, permitindo que o usuário realize múltiplas operações sequencialmente. Estruturas condicionais (if/elif/else) foram utilizadas para verificar as regras de negócio, como a validade do valor do depósito ou as restrições do saque, garantindo que as transações só fossem realizadas se todas as condições fossem atendidas.

- Encerramento: O programa oferece uma opção para o usuário encerrar a sessão, saindo do loop principal e exibindo uma mensagem de agradecimento.

## Resultados Alcançados
O projeto foi concluído com sucesso, resultando em um sistema funcional que atende a todos os requisitos do desafio. As principais conquistas foram:

- Validação de Regras: O código valida efetivamente os limites de saque (quantidade e valor), bem como a validade do valor do depósito, prevenindo transações inválidas.

- Controle de Fluxo: A utilização de while e if/else demonstrou habilidade na construção de fluxos de controle lógicos e interativos.

- Histórico de Transações: A implementação de um extrato detalhado com o histórico completo das movimentações prova a capacidade de armazenar e manipular dados de forma estruturada.

- Prática de Python: O projeto consolidou o conhecimento em conceitos fundamentais da linguagem, como manipulação de variáveis, estruturas de dados (dicionário), laços de repetição e condicionais, além de formatar saídas para o usuário (uso de f-strings).
