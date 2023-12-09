---
title: 'Error en operaciones de reembolso y captura con Payout Split - "Valor en destinatarios * es diferente al valor de la operación *."'
id: 3Wo9ltN7Ju0ZqVLAQZcd7m
status: PUBLISHED
createdAt: 2023-08-23T13:57:20.424Z
updatedAt: 2023-08-23T13:57:21.389Z
publishedAt: 2023-08-23T13:57:21.389Z
firstPublishedAt: 2023-08-23T13:57:21.389Z
contentType: knownIssue
productTeam: Payments
author: 2mXZkbi0oi061KicTExNjo
tag: Payments
slug: error-en-operaciones-de-reembolso-y-captura-con-payout-split-valor-en-destinatarios-es-diferente-al-valor-de-la-operacion
locale: es
kiStatus: Backlog
internalReference: 698005
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Debido a problemas de redondeo al recalcular los destinatarios de una transacción con Payout Split, ya sea en la captura o en el reembolso, recibimos la siguiente excepción de la pasarela, ya que la suma del valor del destinatario difiere del valor de la transacción.


    Vtex.Practices.ExceptionHandling.ValidationException: El valor de los destinatarios (xx.98999999999999999999999999988) es distinto del valor de la operación (xx.99). at Vtex.PaymentGateway.PaymentSplit.RecipientsBuilder.ValidateRecipientsValue(List`1 destinatarios, Decimal valor)...



##

## Simulación


No se puede simular



## Workaround


No hay solución

