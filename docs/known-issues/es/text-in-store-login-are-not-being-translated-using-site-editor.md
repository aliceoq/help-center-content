---
title: 'El texto de inicio de sesión en la tienda no se traduce con el editor del sitio.'
id: 6DptiKTxtOcYIJEgJlZCmo
status: PUBLISHED
createdAt: 2023-11-08T13:33:41.296Z
updatedAt: 2023-11-08T13:33:41.967Z
publishedAt: 2023-11-08T13:33:41.967Z
firstPublishedAt: 2023-11-08T13:33:41.967Z
contentType: knownIssue
productTeam: CMS
author: 2mXZkbi0oi061KicTExNjo
tag: CMS
slug: el-texto-de-inicio-de-sesion-en-la-tienda-no-se-traduce-con-el-editor-del-sitio
locale: es
kiStatus: Backlog
internalReference: 911757
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Al tratar de traducir un texto utilizando el editor de sitio para el inicio de sesión de la tienda, los cambios no se aplicarán en el frente de la tienda.


##

## Simulación



1. Abrir el editor del sitio
2. Seleccione el bloque Store Login
3. Cambia la etiqueta de texto del inicio de sesión por la que desees
4. Guardar cambios
5. Visualice la página y el texto será el mismo independientemente de la configuración regional seleccionada.




## Workaround


Asegúrese de que iconLabel está vacío tanto en el código de la tienda como en el editor del sitio.
Si no está seguro de que esté vacío en el editor del sitio, puede restablecer el contenido pasando por la versión del editor del sitio > restablecer.
 ![](https://vtexhelp.zendesk.com/attachments/token/PXovY6zVHdqqhxjodbtMqdXAa/?name=image.png)

Siga la documentación aquí y los contextos aquí para establecer la etiqueta como desee en su lugar.





