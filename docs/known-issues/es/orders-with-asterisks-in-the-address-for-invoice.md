---
title: 'Pedidos con asteriscos en la dirección de facturación'
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
slug: pedidos-con-asteriscos-en-la-direccion-de-facturacion
locale: es
kiStatus: Backlog
internalReference: 360783
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Hay pedidos en los que la `invoiceAddress` o `shippingAddress` se está enviando como `enmascarada` en lugar de la dirección real. Este comportamiento ocurre cuando un usuario completa la compra con un formulario de pedido que contiene datos enmascarados que son 'stringified'. Como se trata de campos de cadena, los datos del pedido se rellenan con la máscara "***".

Así pues, el fallo radica en que nuestra API para realizar pedidos permite objetos con caracteres especiales en estos campos.


##

## Simulación



1. Añade algunos productos a tu cesta;
2. Durante el proceso de pago, introduzca una dirección de facturación válida e inicie sesión en su cuenta;
3. Abandonar el carrito o salir del sitio web sin completar la compra;
4. Utilizar nuestra API para insertar un archivo adjunto y poner una dirección con "***" en algunos campos, como el del barrio;
5. Realizar un pedido utilizando este mismo carrito;
6. Tenga en cuenta que el pedido tendrá los datos de envío con estos caracteres especiales.


##

## Workaround


N/A





