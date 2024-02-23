---
title: 'O=OrderByPriceASC (o OrderByPriceDESC) podría dar lugar a un pedido erróneo'
id: 2XCplZQutilKeD2bNnjYDx
status: PUBLISHED
createdAt: 2022-05-20T15:48:15.215Z
updatedAt: 2024-01-11T22:09:50.045Z
publishedAt: 2024-01-11T22:09:50.045Z
firstPublishedAt: 2022-05-20T15:48:16.089Z
contentType: knownIssue
productTeam: Portal
author: 2mXZkbi0oi061KicTExNjo
tag: Portal
slug: oorderbypriceasc-o-orderbypricedesc-podria-dar-lugar-a-un-pedido-erroneo
locale: es
kiStatus: Backlog
internalReference: 582861
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


O=OrderByPriceASC (o OrderByPriceDESC) puede utilizar una política incorrecta para ordenar los precios

Además, los precios de los vendedores no regionalizados no se tienen en cuenta en la ordenación. En consecuencia, las tiendas regionalizadas del Portal no pueden utilizar el parámetro OrderByPrice.


##

## Simulación



- Introducir más de un precio en el producto. Ej: dos precios de lista diferentes en vendedores diferentes.
- Poner ordenación de la página por precio (ej: O=OrderByPriceASC)
- Ver que la clasificación no está en el orden de los precios que se muestran



## Workaround


Ninguna en el Portal. Sin embargo, la cuenta puede cambiar a Búsqueda Inteligente.





