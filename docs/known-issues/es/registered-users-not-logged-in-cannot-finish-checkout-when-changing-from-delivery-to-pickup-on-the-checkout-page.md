---
title: 'Los usuarios registrados (que no han iniciado sesión) no pueden finalizar el proceso de pago cuando cambian de entrega a recogida en la página de pago.'
id: hmQ2riW1Ptjxyhk6gcWxN
status: PUBLISHED
createdAt: 2023-07-28T19:49:16.993Z
updatedAt: 2023-07-31T21:10:42.505Z
publishedAt: 2023-07-31T21:10:42.505Z
firstPublishedAt: 2023-07-28T19:49:17.732Z
contentType: knownIssue
productTeam: Checkout
author: 2mXZkbi0oi061KicTExNjo
tag: Checkout
slug: los-usuarios-registrados-que-no-han-iniciado-sesion-no-pueden-finalizar-el-proceso-de-pago-cuando-cambian-de-entrega-a-recogida-en-la-pagina-de-pago
locale: es
kiStatus: Backlog
internalReference: 870845
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Cuando un usuario registrado (no logueado) inicia el checkout con Delivery como opción de envío, y posteriormente cambia a pickup, al intentar finalizar el checkout aparece el mensaje de error "_O campo Número nos dados de entrega é inválido_" y no permite realizar el pedido.


##

## Simulación



1. Ir a la caja y añadir un nuevo artículo
2. Introduzca un código postal para calcular el envío y mantenga **Entrega** seleccionado
3. Cuando se le pida que introduzca una dirección de correo electrónico, utilice la de un usuario registrado.
4. En la caja aparecerá un mensaje emergente informando de que sus datos personales han sido recuperados de compras anteriores
5. 5. Cambie de Entrega a Recogida e intente completar el pedido (aparecerá el mensaje de error)




## Workaround


N/A





