---
title: 'La integración de MercadoPagoV1 y V2 no funciona con la función de guardar tarjeta'
id: 2V8kdA60OTl7VQoUUNgBci
status: PUBLISHED
createdAt: 2022-05-03T15:45:09.856Z
updatedAt: 2023-08-23T14:49:25.228Z
publishedAt: 2023-08-23T14:49:25.228Z
firstPublishedAt: 2022-05-03T15:45:10.554Z
contentType: knownIssue
productTeam: Payments
author: 2mXZkbi0oi061KicTExNjo
tag: Payments
slug: la-integracion-de-mercadopagov1-y-v2-no-funciona-con-la-funcion-de-guardar-tarjeta
locale: es
kiStatus: No Fix
internalReference: 283727
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


La integración de MercadoPagoV1 y MercadoPagoV2 no funciona con la funcionalidad de guardar tarjeta en la sección Mi cuenta.

Este error se produce porque Mis tarjetas esperan una respuesta sincrónica de las entidades adquirentes de tarjetas de crédito y MercadoPagoV1 no devuelve una respuesta inmediata.


##

## Simulación



1. 1. Vaya a VTEX **Admin.**
2. Configurar el adquirente MercadoPagoV1 o MercadoPagoV2.
3. Configura un método de pago con tarjeta de crédito -como Mastercard, Visa, American Express, etc.- para que sea procesado por la entidad adquirente.
4. Vaya a la página de inicio de su tienda.
5. Inicie sesión introduciendo su dirección de correo electrónico y contraseña.
6. Haz clic en **Mi cuenta**.
7. Vaya a la sección **Tarjetas de crédito**.
8. Haga clic en **Añadir nueva tarjeta**.
9. Rellena todos los campos y pulsa en **Guardar nueva tarjeta**.
10. Este proceso devolverá _se ha producido un error al intentar registrar la tarjeta_.



## Workaround


N/A

