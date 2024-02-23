---
title: 'Possíveis erros na notificação de ordens de alteração na interface do usuário, na API e no gateway.'
id: 1UeG6MyFYIUVCnH8kPwNIJ
status: PUBLISHED
createdAt: 2023-12-19T19:37:47.313Z
updatedAt: 2023-12-19T19:37:47.950Z
publishedAt: 2023-12-19T19:37:47.950Z
firstPublishedAt: 2023-12-19T19:37:47.950Z
contentType: knownIssue
productTeam: Order Management
author: 2mXZkbi0oi061KicTExNjo
tag: Order Management
slug: possiveis-erros-na-notificacao-de-ordens-de-alteracao-na-interface-do-usuario-na-api-e-no-gateway
locale: pt
kiStatus: Backlog
internalReference: 955489
---

## Sumário

<div class="alert alert-info">
  <p>Este problema conhecido foi traduzido automaticamente do inglês.</p>
</div>


Alguns problemas foram identificados na arquitetura Change Orders V1, onde alguns casos não eram notificados na interação do pedido na UI, não eram notificados na API Get Orders, porém, havia um desconto ou aumento no valor. Também vimos cenários em que a notificação ocorre na UI e na API, mas o desconto ou aumento não é feito no gateway.

## Simulação


Não é possível realizar uma simulação, pois os cenários são esporádicos e geralmente ocorrem devido a um erro de tempo limite, para o qual já aumentamos o cronômetro.



## Workaround


Inicialmente não temos uma solução alternativa, no entanto, vale mencionar que alguns cenários poderemos ajustar manualmente, como, por exemplo, se o registro de pedidos de alteração ocorrer no gateway e não ocorrer no Marketplace ou na interação do pedido de atendimento e também na API.





