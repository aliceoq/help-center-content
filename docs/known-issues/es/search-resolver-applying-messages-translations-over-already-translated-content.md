---
title: 'Search Resolver aplicando traducciones de Mensajes sobre contenido ya traducido'
id: 7OIKmmhO3Pa2z0pIU33kY
status: PUBLISHED
createdAt: 2023-07-20T15:28:57.078Z
updatedAt: 2024-02-05T21:20:29.986Z
publishedAt: 2024-02-05T21:20:29.986Z
firstPublishedAt: 2023-07-20T15:28:57.934Z
contentType: knownIssue
productTeam: Intelligent Search
author: 2mXZkbi0oi061KicTExNjo
tag: Intelligent Search
slug: search-resolver-aplicando-traducciones-de-mensajes-sobre-contenido-ya-traducido
locale: es
kiStatus: Backlog
internalReference: 865918
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


El Search Resolver (capa GraphQL para la Búsqueda Inteligente) está solicitando traducciones al servicio de Mensajes para contenidos ya traducidos.

En la práctica, estas traducciones se realizan sobre los mismos idiomas "de" y "a", pero si la tienda tiene activada la función de traducción automática, la cadena puede cambiar a algo inesperado.

Esto afecta especialmente a las cadenas con varias palabras que pueden considerarse de idiomas diferentes, como palabras en inglés en el nombre de un producto que está mayoritariamente en francés.


##

## Simulación



- Traduzca cualquier contenido del catálogo de la tienda a un idioma diferente del predeterminado;
- Asegúrese de que todavía hay al menos una palabra en un idioma diferente al traducido;
- Compruebe el escaparate; no coincidirá con la traducción.



## Workaround



- Desactiva la traducción automática;
- Cree traducciones para estos contenidos utilizando el mismo idioma que "de" y "a", por ejemplo, traduciéndolo de "fr-FR" a "fr-FR".



