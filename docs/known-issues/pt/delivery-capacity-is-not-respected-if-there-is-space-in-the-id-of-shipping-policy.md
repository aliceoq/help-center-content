---
title: 'A capacidade de entrega não é respeitada se houver espaço no Id da Política de Remessa'
id: 1OyY54G05o15EI2zAmW4Vq
status: PUBLISHED
createdAt: 2023-07-14T21:25:50.522Z
updatedAt: 2023-07-28T21:37:08.673Z
publishedAt: 2023-07-28T21:37:08.673Z
firstPublishedAt: 2023-07-14T21:25:51.117Z
contentType: knownIssue
productTeam: Logistics
author: 2mXZkbi0oi061KicTExNjo
tag: Logistics
slug: a-capacidade-de-entrega-nao-e-respeitada-se-houver-espaco-no-id-da-politica-de-remessa
locale: pt
kiStatus: Backlog
internalReference: 862830
---

## Sumário

<div class="alert alert-info">
  <p>Este problema conhecido foi traduzido automaticamente do inglês.</p>
</div>


Se o recurso de programação de entrega estiver em uso e a capacidade de entrega estiver ativada, se houver um espaço no Id da política de remessa em questão, a janela sempre estará visível e a quantidade configurada para a capacidade de entrega não será respeitada.

## Simulação


Crie uma política de remessa e, em seu Id, insira um espaço, configure a entrega programada e a capacidade de entrega.
Faça os pedidos selecionando a janela registrada, verifique se será possível criar mais pedidos do que o máximo configurado na capacidade de entrega.
No checkout, quando o limite configurado for atingido, a janela não deverá ficar indisponível, mas permanecerá visível e poderá ser selecionada

## Workaround


Não registre nenhum Id com espaço na política de envio.





