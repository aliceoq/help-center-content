---
title: 'No es posible crear una ruta utilizando el tipo de contenido a través de UI'
id: 3jVjkZYCATrnDNhR0IKSEA
status: PUBLISHED
createdAt: 2023-10-23T13:19:09.970Z
updatedAt: 2023-10-23T13:19:10.738Z
publishedAt: 2023-10-23T13:19:10.738Z
firstPublishedAt: 2023-10-23T13:19:10.738Z
contentType: knownIssue
productTeam: CMS
author: 2mXZkbi0oi061KicTExNjo
tag: CMS
slug: no-es-posible-crear-una-ruta-utilizando-el-tipo-de-contenido-a-traves-de-ui
locale: es
kiStatus: Backlog
internalReference: 923619
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Si intentamos crear una ruta usando tipos de contenido a través de la UI la página no funcionará. Sólo funciona si la creamos a través del tema.


##

## Simulación



- Crea una ruta utilizando un tipo de contenido en el módulo Pages, por ejemplo, `storeTest/:test_id`.
- Guárdala
- Intenta acceder a ella desde el front
- No funcionará



## Workaround


Si añadimos la ruta usando el tipo de contenido a través del tema, la página aparecerá en la UI y funcionará





