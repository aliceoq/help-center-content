---
title: 'Cómo funciona Suscripciones '
id: frequentlyAskedQuestions_4453
status: PUBLISHED
createdAt: 2019-01-24T20:46:00.886Z
updatedAt: 2023-12-21T14:13:17.283Z
publishedAt: 2023-12-21T14:13:17.283Z
firstPublishedAt: 2019-01-24T22:14:56.290Z
contentType: tutorial
productTeam: Post-purchase
author: 0QBQws7rk0t5Mnu8fgfUv
slug: como-funciona-suscripciones
locale: es
legacySlug: como-funciona-suscripciones
subcategory: 1rA9wuuskW3PpjvMrhatAM
---

El **Sistema de Suscripciones** es una aplicación desarrollada por VTEX para facilitar las ventas recurrentes, que sustiye el módulo de *Recurrencia*. Funciona como un programador automático: realiza una recompra en la frecuencia solicitada por el cliente de la tienda. 

Su cliente indica con qué frecuencia desea repetir la compra de un determinado SKU y el sistema rehace el pedido de la compra automáticamente en cada periodo programado, con las mismas características configuradas en el pedido original. 

Una suscripción para VTEX consiste en una lista de SKUs vinculada a cierta configuración de compra. Todas las operaciones de gestión giran en torno a la entidad «Suscripción», que contiene toda la información necesaria para generar el pedido correspondiente. El diagrama a continuación presenta el concepto de suscripción:

![img8 subscriptions ES](//images.ctfassets.net/alneenqid6w5/1tNo9gQza7gWuDXZPRxQRO/0d226ff2f1bbcf31e803c7b9d297e35a/img8_subscriptions_ES_2.png)

La suscripción es una forma simple de ahorrarle tiempo a su cliente y traer un flujo programado de ventas adicional a su tienda. 

## Cómo el cliente de su tienda genera un pedido con Suscripciones 

Cuando termine la [configuración de la funcionalidad Suscripciones V2](https://help.vtex.com/es/tutorial/como-configurar-suscripciones-v2--1FA9dfE7vJqxBna9Nft5Sj), ya estará habilitada para que el cliente de su tienda genere un pedido con Suscripciones. Hay dos maneras en que su cliente puede crear una suscripción: 

### Añadir productos para suscripción durante el checkout

Al añadir un *producto habilitado para Suscripción*, durante el checkout, se mostrará un selector desplegable para cada producto con las opciones de suscripción asociadas a ese SKU. Su cliente deberá seleccionar la opción «Suscripción» y seleccionar la frecuencia de la suscripción. Tenga en cuenta que este flujo puede ser personalizado en algunos casos, dependiendo de la necesidad del negocio. 

Después de seleccionar los detalles de la suscripción, el cliente procederá con el flujo normal de compra. Deberá ingresar la dirección de entrega y utilizar uno de los [**métodos de pago habilitados para el Sistema de Suscripción**](https://help.vtex.com/es/tutorial/como-configurar-suscripciones-v2--1FA9dfE7vJqxBna9Nft5Sj). La suscripción se activará después de la aprobación del pago.

### Crear una nueva suscripción en la página «Mi cuenta»

El cliente de su tienda tiene acceso a la creación de suscripciones en la página **Mi cuenta**. Este espacio permite configurar una nueva suscripción sin tener que pasar por el checkout y completar un pedido.

Para ello, solo hay que entrar a la página **Mi cuenta** en el sitio web de su tienda, acceder a la sección **Suscripciones** y hacer clic en el botón **Nueva suscripción**. Una vez que se registren los métodos de pago y la dirección de entrega, solo hay que hacer clic en el botón **Suscribirse** para activar la suscripción de los productos seleccionados.

## Cómo el cliente de su tienda visualiza las Suscripciones

<div class = "alert alert-info">
En <a href="https://help.vtex.com/es/tutorial/how-my-account-works--2BQ3GiqhqGJTXsWVuio3Xh">Mi Cuenta</a>, los clientes solo pueden acceder a los pedidos de los últimos dos años.
</div>

Después de finalizar el pedido con Suscripción, su cliente visualiza en la página **Mi cuenta** la sección **Suscripciones**. En esta sección, el cliente también puede encontrar la lista de suscripciones realizadas con los detalles y el estado individual. Su cliente también recibirá por *email* una confirmación de la suscripción y del pedido generado.

La comunicación con su cliente acerca de la suscripción se llevará a cabo por el módulo **Centro de mensajes**. Consulte nuestro artículo [Correos Electrónicos Transaccionales para Pedidos de Suscripción](https://help.vtex.com/es/tutorial/e-mails-transacionais-para-pedidos-de-assinatura--2NYHqHMRqZ43Cn6s84ZCB5). 

## Detalles de suscripción

Nuestra página de detalles de suscripción ha sido remodelada para mejorar la experiencia del consumidor al reducir el tiempo que toma encontrar información y realizar tareas. Además, tenemos una nueva función para añadir ítems a una suscripción existente.

### Barra de acciones

Añadimos una barra de acciones para mejorar la comunicación con el usuario sobre lo que necesita hacer o informar sobre eventos importantes de la suscripción. En esta sección su cliente podrá:

- Editar la frecuencia de la suscripción.
- Cambiar el periodo de la suscripción.
- Editar el día de facturación.
- Editar la dirección registrada en la suscripción.
- Pausar la suscripción.
- Cancelar la suscripción.
- Cambiar el método de pago utilizado en el cobro recurrente de la suscripción.

## Añadir productos a su suscripción

Ahora es posible añadir un nuevo ítem a su suscripción a través de la búsqueda de los productos disponibles en la tienda.

## Preguntas frecuentes sobre Suscripciones 

1. **¿Puedo tener más de una suscripción en mi tienda?**
El número de suscripciones es ilimitado, tanto para su tienda como para su cliente. Esto significa que no hay un número máximo de suscripciones que puedan ser vendidas por su tienda o compradas por su cliente. Sin embargo, es importante conocer las condiciones que se aplican en las suscripciones.

2. **¿Puede mi cliente comprar por suscripción y retirar en las tiendas o en puntos de recogida?**
Sí, lea el artículo [Puntos de recogida para pedidos de suscripción (Beta)](https://help.vtex.com/es/tutorial/puntos-de-recogida-para-pedidos-de-suscripcion-beta--csIqB6iBh4QNIFdEj0nVv) para más información.

3. **¿Puede mi cliente registrar más de una dirección en su suscripción?**
No es posible registrar más de una dirección en la misma suscripción.

4. **¿Cuál es el plazo de entrega y la regla de flete?**
El plazo de entrega y la regla de flete se basan en las políticas de entrega vigentes en la tienda en el momento del ciclo del pedido.

5. **¿Puede mi cliente pagar en cuotas sus pedidos de suscripción?**
No es posible pagar en cuotas una suscripción. El pago en cuotas puede ocurrir apenas en el primer pedido; pero a partir del segundo, el valor se cobrará al contado.

6. **¿Qué pasa si la tarjeta de mi cliente es cancelada?**
La suscripción no se generará por falta de posibilidad de pago.

7. **¿Puede mi cliente solicitar una entrega programada para pedidos de Suscripción?**
Todavía no es posible solicitar entregas programadas para pedidos de Suscripción. Ese escenario no se atiende para que su cliente no se vea afectado negativamente si la configuración logística de su tienda cambia. Sin embargo, su cliente puede crear una nueva suscripción con la fecha futura de la primera entrega en el día que desee.   

8. **¿Cómo puedo cancelar, omitir o pausar un pedido de suscripción de mi cliente?**
Todavía no es posible hacer cambios en los pedidos de suscripción de sus clientes a través del Admin de VTEX. Solo es posible pausar, omitir o cancelar un pedido de suscripción por medio del acceso a Televentas, en el painel de subscripción de su cliente, o por medio de nuestras [APIs](https://developers.vtex.com/vtex-rest-api/reference/subscriptions-api-v3-overview).

9. **¿Es posible agregar ítems de Sellers o Marketplaces en un pedido de Suscripción?**
Suscripciones pueden ser creadas con ítems de la propia tienda, de sellers VTEX o de sellers white lable (cuenta franquicia).

10. **¿Si el administrador de la tienda crea una regla para un valor mínimo, ¿esta regla podrá afectar a las suscripciones?**
Sí, si el valor del pedido de suscripción es inferior al límite definido por la configuración _Valor mínimo total de la compra_. Tenga en cuenta que nuestro sistema de Suscripción no admite ciclos, o pedidos con un valor total de $0.

11. **¿Si el precio de un SKU cambia, ¿se verá afectada la suscripción de mi cliente?**
Sí, el precio que paga el cliente por la suscripción se basa en el precio registrado para cada SKU. La suscripción del cliente no acompaña las condiciones de precio del primer pedido realizado. El pedido se realiza con los mismos productos que el pedido original, pero el precio se calculará en función de lo que está configurado en el momento de la siguiente ciclo del pedido.

12. **¿A qué hora se crean pedidos de suscripción?**
La creación de pedidos de suscripción se realiza entre 6:00 y 7:00 de la mañana, con referencia a la zona de Brasil (GMT-3).
