---
title: 'Los mensajes traducen automáticamente el contenido para el mismo idioma (cuando "de" es igual a "a")'
id: 7OIKmmhO3Pa2z0pIU33kY
status: PUBLISHED
createdAt: 2023-07-20T15:28:57.078Z
updatedAt: 2023-07-20T15:28:57.934Z
publishedAt: 2023-07-20T15:28:57.934Z
firstPublishedAt: 2023-07-20T15:28:57.934Z
contentType: knownIssue
productTeam: Store Framework
author: 2mXZkbi0oi061KicTExNjo
tag: Store Framework
slug: los-mensajes-traducen-automaticamente-el-contenido-para-el-mismo-idioma-cuando-de-es-igual-a-a
locale: es
kiStatus: Backlog
internalReference: 865918
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


La aplicación Mensajes traduce automáticamente el contenido cuando el idioma "de" es igual a "a".

Cuando se implementan tiendas multilingües y el contenido tiene una palabra en un idioma extranjero, por ejemplo, si el nombre de un producto se traduce del inglés al español pero sigue teniendo palabras en inglés, mostrará una traducción no deseada.


##

## Simulación



- Traduzca cualquier contenido de la tienda a cualquier otro idioma diferente del predeterminado;
- Asegúrese de que todavía hay al menos una palabra en un idioma diferente al traducido;
- Compruebe el escaparate; no coincidirá con la traducción.



## Workaround



- Desactive la traducción automática;
- Traducir el contenido donde el idioma 'de' es igual a 'a', por ejemplo, de 'es-ES' a 'es-ES'.



