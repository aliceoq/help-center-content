---
title: 'La capacidad de entrega no se respeta si hay espacio en el Id de la política de envío'
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
slug: la-capacidad-de-entrega-no-se-respeta-si-hay-espacio-en-el-id-de-la-politica-de-envio
locale: es
kiStatus: Backlog
internalReference: 862830
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Si se está utilizando la función de orden de entrega y la capacidad de entrega está activada, si hay un espacio en el Id de la política de envío en cuestión, la ventana estará siempre visible y no se respetará la cantidad configurada para la capacidad de entrega.


##

## Simulación


Cree una política de envío y en su Id inserte un espacio, configure la entrega programada así como la capacidad de entrega.
Realice pedidos seleccionando la ventana registrada, verifique que será posible crear más pedidos que el máximo configurado en la capacidad de entrega.
En el checkout una vez alcanzado el límite configurado la ventana no debería estar disponible, sin embargo permanece visible y posible de ser seleccionada.



## Workaround


No registre ningún Id con espacio en la política de envíos.





