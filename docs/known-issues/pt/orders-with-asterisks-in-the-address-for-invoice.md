---
title: 'Pedidos com asteriscos no endereço da fatura'
id: 6AaZ4p042LZwvfeKIqavjw
status: PUBLISHED
createdAt: 2023-08-25T17:03:49.755Z
updatedAt: 2023-11-10T20:11:14.163Z
publishedAt: 2023-11-10T20:11:14.163Z
firstPublishedAt: 2023-08-25T17:03:50.594Z
contentType: knownIssue
productTeam: Checkout
author: 2mXZkbi0oi061KicTExNjo
tag: Checkout
slug: pedidos-com-asteriscos-no-endereco-da-fatura
locale: pt
kiStatus: Backlog
internalReference: 360783
---

## Sumário

<div class="alert alert-info">
  <p>Este problema conhecido foi traduzido automaticamente do inglês.</p>
</div>


Há pedidos em que o `invoiceAddress` ou `shippingAddress` está sendo enviado como "mascarado" em vez do endereço real. Esse comportamento ocorre quando um usuário conclui a compra com um formulário de pedido que contém dados mascarados que são "stringificados". Como esses campos são do tipo string, os dados do pedido são preenchidos com a máscara '***'.

Portanto, o erro está no fato de que nossa API para fazer pedidos permite objetos com caracteres especiais nesses campos.

## Simulação



1. Adicione alguns produtos ao seu carrinho;
2. Durante o processo de checkout, insira um endereço de cobrança válido e faça login em sua conta;
3. Abandonar o carrinho ou sair do site sem concluir a compra;
4. Usar nossa API para inserir um anexo e colocar um endereço com "***" em alguns campos, como o do bairro;
5. Fazer um pedido usando esse mesmo carrinho;
6. Observe que o pedido terá os dados de envio com esses caracteres especiais

## Workaround


N/A





