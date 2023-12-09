---
title: 'Pérdida intermitente de contenido del Editor de Sitios'
id: 3a5MlAoD2Z7Gu6HDS8wihD
status: PUBLISHED
createdAt: 2022-07-05T17:07:24.733Z
updatedAt: 2023-11-01T14:19:36.358Z
publishedAt: 2023-11-01T14:19:36.358Z
firstPublishedAt: 2022-07-05T17:07:25.091Z
contentType: knownIssue
productTeam: CMS
author: 2mXZkbi0oi061KicTExNjo
tag: CMS
slug: perdida-intermitente-de-contenido-del-editor-de-sitios
locale: es
kiStatus: Backlog
internalReference: 610533
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Cada cambio de contenido en el Editor de Sitios inserta cambios en el archivo content.json, que se almacena en un bucket en AWS S3. Algunos clientes han informado de la pérdida de contenido del Editor de Sitios tras algunos procedimientos habituales de actualización de temas.


##

## Simulación


El escenario es intermitente, sin embargo, se ha reportado en dos escenarios diferentes:

**1. Al promover un espacio de trabajo de producción a maestro:**
Los clientes informaron de que al promover un espacio de trabajo de producción, que contenía cambios en los componentes, al entorno maestro, se producía una pérdida de contenido en otros espacios de trabajo.

**2. Al instalar una nueva versión en un espacio de trabajo de prueba:**
Los clientes informaron de que, al instalar una nueva versión del tema en un espacio de trabajo de prueba, se eliminaba el contenido de las páginas de categorías.



## Workaround


N/A





