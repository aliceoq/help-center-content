---
title: 'El sitemap no se genera/actualiza'
id: 1tJ4XHtbnFsfS30JWXwxb0
status: PUBLISHED
createdAt: 2023-05-17T13:58:46.443Z
updatedAt: 2023-12-05T16:45:03.711Z
publishedAt: 2023-12-05T16:45:03.711Z
firstPublishedAt: 2023-05-17T13:58:47.102Z
contentType: knownIssue
productTeam: Store Framework
author: 2mXZkbi0oi061KicTExNjo
tag: Store Framework
slug: el-sitemap-no-se-generaactualiza
locale: es
kiStatus: Backlog
internalReference: 827104
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Hay tres escenarios en los que el mapa del sitio no está siendo generado/actualizado:

1. Cuando tenemos un producto no encontrado o con algún tipo de problema en el catálogo no se genera el mapa del sitio. Puede buscar los logs en OpenSearch, en este caso, para comprobar qué producto tiene un problema;

2. Cuando la cuenta tiene la app `search.resolver@1.x` el sitemap puede tener errores cuando:

      - una categoría tiene su primer producto procedente de una categoría similar (las reglas de comercio pueden tener un impacto en este caso dependiendo del producto que estés promocionando);

      - la página de búsqueda/marca/categoría no tiene productos, en este caso, la página no se indexa en el sitemap, y su generación se bloquea

3. Los productos que no tienen la política comercial establecida en el catálogo no serán recibidos por el sitemap



##

## Simulación


Trate de generar el mapa del sitio para una cuenta que tiene uno de los escenarios descritos anteriormente y se bloqueará



## Workaround


- Crear un nuevo espacio de trabajo
- Instale el `search-resolver@0.x`
- Generar el nuevo mapa del sitio
- Promoverlo a maestro

Pero eventualmente, necesitarás arreglar el escenario que impide que el mapa del sitio sea generado




