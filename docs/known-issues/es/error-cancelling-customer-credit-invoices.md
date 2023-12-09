---
title: 'Error al anular facturas de crédito de clientes'
id: 75nZNOHGYGBlAoTOjG6gs
status: PUBLISHED
createdAt: 2023-10-26T21:09:54.255Z
updatedAt: 2023-10-26T21:09:54.992Z
publishedAt: 2023-10-26T21:09:54.992Z
firstPublishedAt: 2023-10-26T21:09:54.992Z
contentType: knownIssue
productTeam: Payments
author: 2mXZkbi0oi061KicTExNjo
tag: Payments
slug: error-al-anular-facturas-de-credito-de-clientes
locale: es
kiStatus: Backlog
internalReference: 926563
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Hemos encontrado casos en los que no se puede cancelar una factura, al ejecutar la API DEL obtenemos un error 500 con la siguiente respuesta:

`"mensaje": "Se ha producido un error."`


##

## Simulación


No hemos podido replicar este error, parece relacionado con facturas antiguas (con fecha anterior a 2023)



## Workaround


NA




