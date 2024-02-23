---
title: '¿Cómo funciona VTEX Intelligent Search?'
id: 23mytRDsEduqLO0Lo7yufy
status: PUBLISHED
createdAt: 2020-03-05T14:57:22.014Z
updatedAt: 2024-02-07T13:18:52.194Z
publishedAt: 2024-02-07T13:18:52.194Z
firstPublishedAt: 2020-03-05T19:54:00.932Z
contentType: trackArticle
productTeam: Marketing & Merchandising
slug: como-funciona-vtex-intelligent-search
locale: es
trackId: 19wrbB7nEQcmwzDPl1l4Cb
trackSlugES: vtex-intelligent-search
---

El motor de búsqueda es el centro de la inteligencia de VTEX Intelligent Search. Interpreta el término buscado y muestra la lista de productos filtrada y ordenada. Esta herramienta permite una búsqueda más objetiva, a través de la indexación y el tratamiento de los datos del catálogo.

Esta es una funcionalidad predeterminada de VTEX Intelligent Search y cubre a la mayoría de los escenarios. Sin embargo, el motor de búsqueda también presenta algunos ajustes para perfeccionar el resultado de la búsqueda. En esta guía describimos:

* [Configuración del comportamiento de la búsqueda](#configuracion-del-comportamiento-de-la-busqueda)
* [Formas de búsqueda alternativas](#formas-de-busqueda-alternativas)
* [Indexación](#indexacion)

## Configuración del comportamiento de búsqueda

Hay un conjunto de ajustes que alteran la lista y el orden de los productos mostrados en el resultado de la búsqueda. En las siguientes secciones se presentan las principales definiciones que afectan el comportamiento de la búsqueda.

### Definición de los campos de búsqueda

Determina la información de producto que se puede buscar. A partir de la configuración, toda búsqueda realizada en la barra de búsqueda verifica el contenido de este campo para generar resultados de búsqueda. Consulta la tabla a continuación para saber qué información permite la realización de búsquedas de forma predeterminada y ver las otras opciones de configuración:

| Información | Configuración |
| - | - |
| Nombre del producto, marca, ID de producto (`ProductID`), código de referencia del producto (`ProductRefID`), ID del SKU (`SKUID`), código de referencia del SKU (`SKURefID`) y EAN | Se pueden realizar búsquedas en estos datos de forma predeterminada en VTEX Intelligent Search. Para remover alguno de ellos, ponte en contacto con nuestro [Soporte](https://help.vtex.com/es/support). |
| Especificaciones de producto y SKU | Ponte en contacto con nuestro [Soporte](https://help.vtex.com/es/support) para incluir las especificaciones deseadas como campos de búsqueda.<br /><br /> Por ejemplo, si una camisa no tiene el color en el nombre del producto o del SKU, de forma predeterminada, Intelligent Search no identifica ese atributo cuando se busque “camisa azul” y devolverá como resultado camisas de diferentes colores. Sin embargo, si la especificación de color se configura de manera que se pueden realizar búsquedas sobre la especificación de color, la búsqueda podrá devolver camisas azules en las primeras posiciones.<br /><br /> Puedes ver más información sobre especificaciones en [Especificaciones de producto y SKU](https://help.vtex.com/es/tracks/catalogo-101--5AF0XfnjfWeopIFBgs3LIQ/2NQoBv8m4Yz3oQaLgDRagP). |
| Código del fabricante (`ManufactureID`) | Ponte en contacto con nuestro [Soporte](https://help.vtex.com/es/support) para configurar la realización de búsquedas en este campo. |

*Ejemplo*: se configuró que la especificación “color” se puede buscar y el producto está registrado con el nombre “Zapatilla Nike Total 90” y con el color “negro”. Si un cliente busca “Zapatilla Negra”, la herramienta devolverá productos que tengan el término “zapatilla” y el color “negra” en la parte superior del resultado de búsqueda.

Se puede encontrar un producto realizando una búsqueda por caracteres especiales (`-` y `/`).

<div class="alert alert-warning">
	<p>La selección de los campos de búsqueda afecta las posibilidades de las <a href="https://help.vtex.com/es/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/5tBSYXb9EIdePa0MWTnFd0">reglas de merchandising</a>, ya que solo se pueden utilizar los campos que permiten búsquedas para configurar reglas. Por ejemplo, al definir solo el campo <code>SKUID</code> para búsquedas, no se podrá promover un <code>ProductID</code> o un <code>ProductRefID</code> utilizando reglas de merchandising.</p>
</div>

### Definición y orden de los campos de filtro

En todos los resultados de búsqueda se muestran filtros que el usuario puede seleccionar. De forma predeterminada, algunos filtros ya están predefinidos, pero es posible crearlos según la necesidad de la tienda. Otro aspecto personalizable es el orden de visualización. Ejemplo: en una lista de resultados de búsqueda pueden haber los filtros Precio, Categorías y Marca.

### Configuración de autocorrección

El usuario puede cometer errores ortográficos al realizar una búsqueda. Es función de la herramienta interpretar estos errores y devolver como resultados los productos que se parezcan a la búsqueda realizada.

Para esto, el motor de búsqueda intenta corregir lo que el usuario escribió de acuerdo con los ítems registrados en el catálogo. Para cada término de búsqueda, se permite un número específico de caracteres incorrectos. Esta cantidad de errores aceptados se denomina *fuzzy*.

El *fuzzy* varía dependiendo del tamaño del término de búsqueda. De forma predeterminada, si el término tiene de 3 a 5 caracteres, el *fuzzy* aplicado es 1, es decir, 1 carácter puede estar equivocado. Para términos de 6 caracteres o más, el *fuzzy* aplicado es 2.

Los errores previstos considerando *fuzzy* = 1 son:

* Introducir 1 carácter extra.
* Eliminar 1 carácter.
* Intercambiar 1 carácter.
* Intercambiar 2 caracteres que estén uno al lado del otro.

Ejemplo: Supongamos que un cliente quiere buscar el término `bola`. Siguiendo la configuración predeterminada (*fuzzy* = 1 para términos de 3 a 5 caracteres), el motor de búsqueda mostrará el resultado `bola` para cualquier búsqueda que contenga los errores aceptados, como:

* `bolla` (introducir 1 carácter extra)
* `boa` (eliminar 1 carácter)
* `bora` (cambiar 1 carácter)
* `obla` (intercambiar 2 caracteres que están uno al lado del otro entre ellos)

<div class="alert alert-info">
	<p>Los espacios en blanco no se consideran en el <em>fuzzy</em>, por lo que <code>base ball</code> no se corregirá a <code>baseball</code>. Recomendamos utilizar <a href="https://help.vtex.com/es/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/1pxAWPEglBey1UFdvcetZV">sinónimos</a> para estos casos.</p>
</div>

### Configuración de relevancia

La relevancia es la funcionalidad que define el orden de los productos en el resultado de búsqueda. Esta configuración permite asignar pesos y priorizar determinados criterios utilizados por el motor de búsqueda, como popularidad, fecha de lanzamiento del producto y participación en promociones. La relevancia de un producto está compuesta por la combinación de los pesos y prioridades definidos por cada administrador de la tienda.

Ejemplo: un administrador de la tienda configuró que el criterio “promoción” tiene una mayor relevancia que otros criterios. Así, cuando un cliente busca “camiseta” en la búsqueda interna de la tienda, las camisetas incluidas en las promociones tienden a aparecer en primer lugar en los resultados, dependiendo del peso asignado a los demás criterios.

Para obtener más información sobre cómo personalizar el orden de los resultados de acuerdo con las necesidades de tu tienda, consulta el artículo [Configuración de relevancia](https://help.vtex.com/es/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/1qlObWIib6KqgrfX1FCOXS).

<div class="alert alert-info">
	<p>Al utilizar Intelligent Search, hay dos opciones que definirán el orden de tus colecciones. Si utilizas el comando <code>map=productClusterIds</code>, estás definiendo que el orden de tus colecciones será el predefinido por el administrador de la tienda, con su propio criterio de relevancia. Si eliges utilizar <code>productClusterNames</code>, estás definiendo que quieres que tus colecciones sigan los estándares de relevancia de Intelligent Search.</p>
</div>

### Configuración de resultado mínimo

El motor de búsqueda permite configurar la cantidad mínima de productos para la consulta de múltiples términos. Si no se alcanza este número, la búsqueda presenta resultados más amplios, que respetan solo uno de los términos buscados.

Ejemplo: se configuró que el resultado mínimo para consultas con múltiples términos es **tres**. El usuario realizó la búsqueda de “zapatilla nike”, pero el catálogo solo tiene **cuatro** productos con ese nombre. La plataforma presentará primero productos que tengan el término “zapatilla nike”, luego productos con el término “zapatilla” y, por último, aquellos que tengan el término “nike”.

### Límite de páginas

VTEX Intelligent Search limita el resultado de la búsqueda a 50 páginas. Este límite fomenta el uso de filtros, lo que permite una navegación más relevante y centrada para el usuario.

## Formas alternativas de búsqueda

Es posible buscar el ID de uno o varios artículos en la barra de búsqueda o añadiendo parámetros de consulta (*query*) a la URL de la tienda.

### Coincidencia parcial

Al ingresar únicamente los primeros dígitos exactos del ID del producto (`ProductID`), código de referencia del producto (`ProductRefID`), ID del SKU (`SKUID`), código de referencia del SKU (`SKURefID`) o EAN en la barra de búsqueda, Intelligent Search hará un match parcial con productos y SKU activos en la tienda, incluyéndolos en los resultados de la búsqueda.

Por ejemplo, si el ID del producto es `123456789` y la búsqueda realizada es `123`, ese producto se mostrará entre los resultados; sin embargo, si la búsqueda es `234`, sin alguno de los primeros dígitos del ID, este producto no se mostrará.

### URL

Para buscar desde la URL de su tienda, añada parámetros de búsqueda (*query*) al final de la URL de la tienda, respetando una de las siguientes estructuras:

- Ejemplo de búsqueda de un ítem: `[dirección de la cuenta]/[tipo de id]:[id_1]?q=[tipo de id]&map=ft`
- Ejemplo de búsqueda de lista: `[dirección de la cuenta]/[tipo de id]:[id_1];[id_2];[id_3]?q=[tipo de id]:[id_1];[id_2];[id_3]&map=ft`

Los posibles tipos de valores para el campo “tipo de ID” son `product.id`, `sku.id`, `sku.ean`, `sku.reference` o `id` (ProductID, ProductRefID, SKUID, SKURefID y EAN). Cabe resaltar que todos los ID deben ser del mismo tipo.

* **Búsqueda por ID de SKU:** `?q=sku.id:<id>` o `?q=sku:<id>`
* **Búsqueda por EAN:** `?q=sku.ean:<id>`
* **Búsqueda por ID de referencia:** `?q=sku.reference:<id>`
* **Búsqueda por slug:** `?q=product.link:<link>`
* **Búsqueda por ID de producto:** `?q=product:<id>` o `?q=product.id:<id>`

## Indexación

La indexación es un proceso de sincronía entre los catálogos de la tienda y la búsqueda. Esta funcionalidad permite una actualización continua del índice de productos. Además, ejecuta un tratamiento de datos para utilizarlos en la búsqueda.

Inicialmente, se realiza una sincronización con todos los productos del catálogo VTEX del cliente. Después, el indexador de búsqueda recibirá en tiempo real las futuras actualizaciones de datos, como el nombre y el status del producto.

En este proceso de sincronía, el sistema forma una fila con la información que se ha actualizado para indexarlas en el catálogo de búsqueda. Una vez que se hayan indexado todos los cambios, estarán disponibles en el sitio web.

El proceso de indexación es seguro y cuenta con reglas de recuperación: si un ítem no se indexa en el primer intento, el sistema realiza más intentos. La indexación también es muy importante para analizar, tratar y organizar los datos de la mejor manera para que se muestren en los resultados.

Consulta [Historial de indexación](https://help.vtex.com/es/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/4flMwTaQL8FRKl1YT58ezH) para ver más información sobre cómo monitorear el proceso de indexación.
