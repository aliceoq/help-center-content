---
title: 'Autenticación'
id: 21CkKHLKP1o41lUpGhuRUs
status: PUBLISHED
createdAt: 2021-10-25T19:06:37.982Z
updatedAt: 2023-10-26T14:49:32.469Z
publishedAt: 2023-10-26T14:49:32.469Z
firstPublishedAt: 2021-11-08T18:39:50.432Z
contentType: tutorial
productTeam: Identity
author: 1malnhMX0vPThsaJaZMYm2
slug: autenticacion
locale: es
legacySlug: pagina-de-autenticacion
subcategory: 14V5ezEX0cewOMg0o0cYM6
---

La autenticación es el procedimiento de validación de la identidad de los usuarios. En VTEX, este proceso tiene lugar en tres escenarios diferentes:

* [Inicio de sesión](#inicio-de-sesion): verificación y validación de la identidad de los usuarios que desean acceder a una tienda virtual o al Admin VTEX.
* [Desarrollo de integraciones](#desarollo-de-integraciones): autentica las requests realizadas a las API de VTEX a partir de integraciones con servicios externos. Esta validación suele realizarse mediante claves de API o tokens de usuario.
* [Desarrollo de aplicaciones](#desarollo-de-aplicaciones): garantiza la legitimidad de la comunicación entre las aplicaciones desarrolladas con VTEX IO y las API de VTEX. Esta validación suele realizarse mediante tokens de autenticación.

## Inicio de sesión

En VTEX, la autenticación por inicio de sesión se produce en dos contextos: en la tienda virtual, cuando los clientes inician sesión para acceder a su perfil o realizar una compra, y en el Admin VTEX, cuando los usuarios administrativos inician sesión para operar en el entorno administrativo de la tienda.

Es necesario configurar el método de autenticación que se ofrecerá en cada contexto. Consulta las opciones disponibles en la siguiente tabla:

| Opciones de inicio de sesión | Descripción | Tienda virtual | Admin |
|---|---|---|---|
| Código de acceso | Se envía al email del usuario un código numérico aleatorio; el usuario debe informar dicho código para iniciar sesión. | Se puede activar | Siempre activa |
| Contraseña | El usuario puede registrar una contraseña e iniciar sesión utilizando el email y la contraseña registrados. | Se puede activar | Siempre activa |
| Facebook | El usuario inicia sesión utilizando su cuenta de Facebook. | Se puede activar | No disponible |
| Google | El usuario inicia sesión utilizando su cuenta de Google. | Se puede activar | Se puede activar |
| Integración con otros proveedores de identidad | El usuario puede iniciar sesión utilizando su cuenta de otros proveedores de identidad externos a partir de una integración. Consulta la guía para desarrolladores [Login (SSO)](https://developers.vtex.com/docs/guides/login-integration-guide) para obtener más detalles. | Se puede activar utilizando el protocolo OAuth.  Consulta la guía para desarrolladores [Webstore (OAuth 2.0)](https://developers.vtex.com/docs/guides/login-integration-guide-webstore-oauth2) para obtener más detalles. | Se puede activar utilizando o protocolo SAML. Consulta la guía para desarrolladores [Admin (SAML 2.0)](https://developers.vtex.com/docs/guides/login-integration-guide-admin-saml2) para obtener más detalles. |

<div class="alert alert-info">
  <p>Al menos una de las opciones de inicio de sesión de la tabla anterior debe estar activa en la tienda virtual.</p>
</div>

<div class="alert alert-warning">
  <p>Para acceder al Admin VTEX es necesario tener un <a href="https://help.vtex.com/es/tutorial/gestionar-usuarios--tutorials_512">usuario</a> administrativo registrado. Los <a href="https://help.vtex.com/es/tutorial/roles--7HKK5Uau2H6wxE1rH5oRbc">roles</a> relacionados con el usuario y los permisos propios de dicho rol determinan los <a href="https://help.vtex.com/es/tutorial/recursos-del-license-manager--3q6ztrC8YynQf6rdc6euk3">recursos</a> que ese usuario puede utilizar en el Admin.</p>
</div>

### Activar formas de inicio de sesión

En la página **Autenticación**, puedes elegir las opciones de inicio de sesión que deseas ofrecer a los clientes de tu tienda y a los usuarios administrativos que tendrán acceso al Admin de tu cuenta.

![Página de autenticación](//images.ctfassets.net/alneenqid6w5/6cbXmuu9GiTfuYnIsuFKQp/ed710d537b491e8a182de685fa8d0d97/Tela_de_Autentica____o_ES.png)

Sigue estos pasos para activar las opciones de inicio de sesión que desees:

1. En la barra superior del Admin VTEX, haz clic en el avatar de tu perfil que tiene la inicial de tu email.
2. Haz clic en **Configuración de la cuenta > Autenticación**.

    Se te redirigirá a la pestaña **Tienda virtual**, donde se muestran los métodos de inicio de sesión disponibles en tu tienda virtual. En esta pestaña puedes activar las opciones para el inicio de sesión de los clientes.

    Para configurar métodos de inicio de sesión en el Admin para usuarios administrativos, haz clic en la pestaña **Admin**.

    Consulta la tabla en la sección [Inicio de sesión](#inicio-de-sesion) para conocer los métodos de inicio de sesión disponibles y acceder a la documentación que explica cómo configurarlos.

## Desarrollo de integraciones

Al desarrollar integraciones utilizando las [API](https://developers.vtex.com/docs/guides/getting-started) de VTEX, es necesario proporcionar parámetros de autenticación para realizar las operaciones deseadas. Consulta a continuación los métodos disponibles:

* **Claves de aplicación (appKeys):** las [claves de aplicación](https://help.vtex.com/es/tutorial/chaves-de-aplicacao--2iffYzlvvz4BDMr6WGUtet) se utilizan para autenticar los requests a las API de VTEX. Los administradores de la tienda pueden crear claves y asociarlas a [roles](https://help.vtex.com/es/tutorial/roles--7HKK5Uau2H6wxE1rH5oRbc) con permisos para utilizar determinados [recursos](https://help.vtex.com/es/tutorial/recursos-del-license-manager--3q6ztrC8YynQf6rdc6euk3) de la plataforma. Consulta más información en la siguiente guía para desarrolladores, [API authentication using application keys](https://developers.vtex.com/docs/guides/api-authentication-using-application-keys).
* **Tokens de usuario:** los tokens de usuario se utilizan para autenticar los requests de API, especialmente para aplicaciones [frontend](https://help.vtex.com/es/tracks/desarrollo-de-la-tienda--3fHF3GIjK8UugnQKIakpl9/5DTcawNjc5MovtD7HNqURl) desarrolladas con VTEX IO. Consulta más información en la siguiente guía para desarrolladores, [API authentication using user tokens](https://developers.vtex.com/docs/guides/api-authentication-using-user-tokens).

## Desarrollo de aplicaciones

El uso de tokens de autenticación (auth tokens) es necesario para la autenticación cuando se desarrollan aplicaciones en VTEX IO. Consulta más información en la siguiente guía para desarrolladores, [App authentication using auth tokens](https://developers.vtex.com/docs/guides/app-authentication-using-auth-tokens).
