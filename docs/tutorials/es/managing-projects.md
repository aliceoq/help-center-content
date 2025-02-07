---
title: 'Gestionar Proyectos'
id: 42IpDFqTVTESH8DCypJMPM
status: PUBLISHED
createdAt: 2023-11-01T13:45:57.091Z
updatedAt: 2023-11-16T14:44:11.820Z
publishedAt: 2023-11-16T14:44:11.820Z
firstPublishedAt: 2023-11-01T19:38:50.237Z
contentType: tutorial
productTeam: VTEX IO
author: 4oTZzwYoyhy1tDBwLuemdG
slug: gestionar-proyectos
locale: es
legacySlug: gestionar-proyectos
subcategory: 27t6x0lngvjI3bnUg5AgEO
---

Proyectos es una funcionalidad de VTEX Headless CMS que simplifica la gestión de varios proyectos de frontend, como aplicaciones móviles, páginas web y email marketing, desde un único dashboard.

![Projects pages](//images.ctfassets.net/alneenqid6w5/5sXlS9M78whzUVdSxJiKpX/28a48f587a491e87481d837595130e0d/projects-one-es.gif)

Cada proyecto cuenta con sus propios ajustes, contenido y marca, pudiendo personalizarse en función de públicos u objetivos específicos. 

En esta guía aprenderás a gestionar cada proyecto de frontend de tu tienda.

## Antes de empezar
Asegúrate de tener acceso a VTEX Headless CMS. Ponte en contacto con los administradores de la cuenta para comprobar si tu rol de usuario tiene permiso para gestionar contenido en VTEX Headless CMS en el Admin VTEX. Para saber más, consulta el artículo [Roles] (https://help.vtex.com/es/tutorial/roles--7HKK5Uau2H6wxE1rH5oRbc).

## Visión general
Para acceder a **Proyectos**, en el Admin VTEX ve a **Storefront > Headless CMS**.

![Projects overview](//images.ctfassets.net/alneenqid6w5/3RgVmOuLr7SJmEfots0KMZ/fa66fd00d9a29e3eeb835369c70277d7/projects-two-es-outro.png)

| Opciones     | Descripción     |
| ---------- | ---------- |
| Tarjeta del proyecto       | Abre el proyecto seleccionado, para que puedas crear y editar las páginas de su contenido.       |
| Configuración (⚙️)      | Abre una ventana que muestra los ajustes del proyecto organizados en dos pestañas: <ul><li>**General:** permite editar el ID del proyecto y la configuración de la API o archivar el proyecto.</li> <li>**Compilar:** permite conectar el proyecto CMS con tu código fuente a través de webhooks, configurando los tipos de contenido y las secciones. </li></ul>      |
| Crear nuevo | Abre una página para configurar un nuevo proyecto. |

## Crear un nuevo proyecto

Crea un nuevo proyecto para tu tienda configurando ajustes generales como **ID del proyecto** y **URL base de producción**. Para conectar eficazmente un proyecto Headless CMS con el código fuente de tu proyecto también será necesario configurar webhooks y ajustes de compilación, como *URL de compilación de webhook* y *URL de previsualización*. 

Un webhook es un endpoint HTTP que permite la comunicación automatizada entre VTEX Headless CMS y el código fuente del proyecto. Por ejemplo, permite que el CMS notifique a un proyecto FastStore sobre cambios de contenido u otros eventos, desencadenando acciones como la sincronización de contenido en tiempo real.

1. En la página **Proyectos**, haz clic en `Crear nuevo`.
2. En la página **Nuevo proyecto**, rellena los campos de la sección [Configuración del proyecto](#configuración del proyecto).
3. Después de definir cada campo de la página, haz clic en `Crear` y un mensaje de éxito se mostrará en la pantalla.

Tras crear un nuevo proyecto, puedes crear páginas para el mismo con todas las rutas URL y modelos de página compatibles con tu tienda, como páginas de inicio, de producto y de inicio de sesión. 

Para crear una nueva página sigue los pasos presentes en este artículo: [Gestión de páginas en Headless CMS](https://help.vtex.com/es/tutorial/managing-pages--3DO6rBhZ1p3zndnFu5BgRt)

## Configuración del proyecto
En Configuración, puedes realizar ajustes en el proyecto en dos categorías principales:

[General](#general): permite editar el ID del proyecto, la configuración de la API y archivar el proyecto.
[Compilar](#compilar): permite establecer la conexión entre el proyecto CMS y el código de tu proyecto.

### General

| Nombre del campo     | Descripción     | Ejemplo de valor    |
| ---------- | ---------- | ---------- |
| ID del proyecto (obligatorio)      | ID del proyecto.       | `Sales App`        |
| API       | URL base de producción del sitio web.       | `https://{accountName}.vtex.com/`      |

### Compilar

| Nombre del campo    | Descripción     | Ejemplo del valor     |
| ---------- | ---------- | ---------- |
| URL de las secciones       | URL del webhook para recibir y guardar las secciones creadas en el código fuente en Headless CMS.      | `https://infra.io.vtex.com/vbase/v0/{accountName}/master/buckets/vtex.admin-cms-graphql-rc/store/files/{builderId}/sections`       |
| URL de los tipos de contenido       | URL del webhook para recibir y guardar los tipos de contenido creados en el código fuente en Headless CMS.       | `https://infra.io.vtex.com/vbase/v0/{accountName}/master/buckets/vtex.admin-cms-graphql-rc/store/files/{builderId}/content-types`       |
| URL de compilación del webhook       | URL del webhook para iniciar una nueva compilación en Headless CMS cuando se agrega o edita una página o contenido.       | `https://app.io.vtex.com/vtex.cms-builder-sf-jamstack/v1/{accountName}/{workspace}/build-releases`      |
| Guardar URL de webhook      | URL de webhook para permitir previsualizaciones del proyecto en tiempo real, enviando una notificación para actualizar la página y que se reflejen los últimos cambios en Headless CMS.      | -       |
| URL de previsualización      | URL de webhook que permite la previsualización de páginas en el Headless CMS. | `https://{accountName}.vtex.app/api/preview` |

## Editar proyecto
Después de crear el proyecto, también puedes editar toda la información definida durante la [creación del proyecto](#crear-nuevo-proyecto).
En la página principal **Proyectos**, haz clic en **Configuración** (⚙️), y se abrirá una ventana con dos pestañas para realizar ajustes: [General](#general) y [Compilar](#compilar).

## Archivar proyecto
Al archivar un proyecto se desactiva la API y el acceso al contenido del proyecto. 
Para archivar un proyecto sigue los pasos a continuación:

1. Accede a **Storefront > Proyectos**.
2. Selecciona el proyecto que deseas archivar y haz clic en **Configuración** (⚙️). 
3. Haz clic en `Archivar proyecto` en la página `General`. Aparecerá un mensaje emergente para confirmar que deseas archivar el proyecto.
![Arquivar projeto - ES](//images.ctfassets.net/alneenqid6w5/3FkQ3UCU68HH8QkP4LH91I/a7f9e04f4b9dc6161bd3f9a9c683f99c/projects-three-es.png)
4. Haz clic en `Archivar`. A continuación aparecerá un mensaje informando que el proyecto se archivó con éxito.

Para restaurar un proyecto archivado, sigue los pasos descritos en [Restaurar proyecto] (#restaurar-proyecto).

### Restaurar proyecto
Al restaurar un proyecto la API se reactiva y se puede acceder de nuevo a su contenido.
Para restaurar un proyecto sigue los pasos a continuación:

1. Accede a **Storefront > Proyectos**.
2. Haz clic en la tarjeta del proyecto archivado.
3. Haz clic en `Restaurar proyecto`. Aparecerá un mensaje emergente para confirmar que deseas restaurar el proyecto.
4. Haz clic en `Restaurar`. A continuación aparecerá un mensaje informando que el proyecto se restauró con éxito.

