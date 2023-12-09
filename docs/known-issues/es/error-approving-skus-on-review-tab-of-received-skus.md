---
title: 'Error al aprobar skus en la pestaña de revisión de skus recibidos'
id: 7fRMTxq7CFRkyZeK08AGIg
status: PUBLISHED
createdAt: 2023-11-23T13:46:30.453Z
updatedAt: 2023-11-23T13:46:31.370Z
publishedAt: 2023-11-23T13:46:31.370Z
firstPublishedAt: 2023-11-23T13:46:31.370Z
contentType: knownIssue
productTeam: Marketplace
author: 2mXZkbi0oi061KicTExNjo
tag: Marketplace
slug: error-al-aprobar-skus-en-la-pestana-de-revision-de-skus-recibidos
locale: es
kiStatus: Backlog
internalReference: 940998
---

## Sumario

<div class="alert alert-info">
  <p>Este problema conocido ha sido traducido automáticamente del inglés.</p>
</div>


Cuando un sku falla las reglas opcionales de Calidad de Oferta creadas por el Marketplace, va directamente a la "Pestaña de Revisión" de Skus Recibidos.

Sin embargo, al intentar aprobar el sku, se devuelve un mensaje de error: "Lo sentimos, algo ha ido mal en el Catálogo. Por favor, inténtelo de nuevo o póngase en contacto con VTEX si el problema persiste".

Esto ocurre porque el módulo Matcher no ha podido rellenar la información del producto y del sku después de enviar el sku a la pestaña Review (puedes comprobarlo usando las APIs):
 ![](https://vtexhelp.zendesk.com/attachments/token/0Dti3ak7twOpuVzvzntmPCGit/?name=image.png)


##

## Simulación



1. Cree una regla opcional sobre Calidad de la oferta;
2. Espere a que un sku falle la regla y vaya a la pestaña Revisar;
3. Intente aprobar el sku y obtenga un mensaje de error;
4. 4. Comprobar a través de la API si el objeto de coincidencias se rellena como en la imagen anterior.



## Workaround


Aprobar el sku a través de la API pasando la información correcta del producto y del sku manualmente.





