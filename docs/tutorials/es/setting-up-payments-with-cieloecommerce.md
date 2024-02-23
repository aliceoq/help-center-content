---
title: 'Configurar pago con CieloEcommerce'
id: 6zuELBqEo0QzApbU4l7L4
status: PUBLISHED
createdAt: 2023-09-18T14:07:22.540Z
updatedAt: 2024-01-23T18:19:25.965Z
publishedAt: 2024-01-23T18:19:25.965Z
firstPublishedAt: 2023-09-18T15:29:57.321Z
contentType: tutorial
productTeam: Financial
author: 6DODK49lJPk3yvcoe6GB6g
slug: configurar-pago-con-cieloecommerce
locale: es
legacySlug: configurar-pago-con-cieloecommerce
subcategory: 3tDGibM2tqMyqIyukqmmMw
---

En VTEX es posible la integración con el CieloEcommerce. Con esta integración, su tienda puede rrealizar ventas a través de tarjetas de credito, debito, private y cobranded labels, boletos, PIX, entre otros. Para configurar CieloEcommerce, siga los siguientes pasos:

1. En el Admin VTEX, accede a __Configuración de la tienda > Pago > Proveedores__, o escribe __Proveedores__ en la barra de búsqueda en la parte superior de la página.
2. En la pantalla de proveedores, haga clic en el botón `Nuevo proveedor`.
3. Escriba el nombre __CieloEcommerce__ en la barra de búsqueda y haga clic en el nombre del proveedor.
4. Rellene los campos de registro __Application Key__ y __Application Token__ con los datos proporcionados por CieloEcommerce.
5. En __Integration__, seleccione si el conector se utilizará como __Adquirencia__ o __Gateway__.
6. En __Provider__, seleccione el adquiriente que se utilizará con el conector CieloEcommerce.
7. En __IsSplit__, elija si la opción de split estará disponible.
8. En __UseMpi__, elija si autenticarán las transacciones. Si selecciona “Sí”, vaya al Paso 9. Si selecciona “No”, vaya al Paso 10.
9. Rellene los campos __MpiClientId__, __MpiClientSecret__, __MpiMerchantName__, __MpiMCC__ y __MpiEstablishmentCode__ con tus datos de acceso a Mpi.
10. En __SoftDescriptor__, indicar la información que se mostrará para identificar la transacción realizada en su tienda.
11. Em __Captura__, seleccione el período en el que se debe solicitar la captura de pago. El horario estándar se realizará cuatro días después de la autorización.
12. En __Activar split y enviar receptores?__, seleccione si los pagos divididos estarán disponibles para el marketplace y los vendedores.
13. Haga clic en `Guardar`.

Para configurar los métodos de pago a procesar por CieloEcommerce, acceda al [Configurar Condiciones de Pago](https://help.vtex.com/es/tutorial/condiciones-de-pago--tutorials_455#).

Para establecer condiciones especiales en los métodos de pago, acceda al [Configurar condiciones especiales de Pago](https://help.vtex.com/es/tutorial/condiciones-especiales--tutorials_456#).

Después de seguir los pasos indicados, CieloEcommerce puede tardar hasta 10 minutos en aparecer en el checkout de tu tienda como una opción de pago.
