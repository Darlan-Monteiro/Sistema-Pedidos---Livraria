# Sistema-Pedidos---Livraria
Este projeto é um sistema de gerenciamento de pedidos para uma livraria, implementado em SQL. O sistema permite o registro e gerenciamento de clientes, editoras, livros, pedidos e itens de pedidos. O objetivo é fornecer uma solução para controlar o estoque e processar pedidos de forma eficiente.


Estrutura do Banco de Dados
O banco de dados é composto pelas seguintes tabelas:

Cliente

idCliente: Identificador único do cliente.
nome: Nome do cliente.
telefone: Número de telefone do cliente.
email: Endereço de e-mail do cliente.
endereco: Endereço completo do cliente.
Editora

idEditora: Identificador único da editora.
nome: Nome da editora.
telefone: Número de telefone da editora.
email: Endereço de e-mail da editora.
endereco: Endereço completo da editora.
Livro

idLivro: Identificador único do livro.
titulo: Título do livro.
autor: Autor do livro.
ano: Ano de publicação do livro.
ISBN: Número ISBN do livro.
preco: Preço do livro.
idEditora: Identificador da editora responsável pela publicação.
Pedido

idPedido: Identificador único do pedido.
idCliente: Identificador do cliente que fez o pedido.
dataPedido: Data do pedido.
valorPedido: Valor total do pedido.
ItemPedido

idPedido: Identificador do pedido.
idLivro: Identificador do livro.
quantidade: Quantidade do livro no pedido.
valorItemPedido: Valor total do item no pedido.
Estoque

idLivro: Identificador do livro.
quantidade: Quantidade disponível do livro no estoque.
