---
title: Cómo configurar AWS SSO
article_id: 360022411353
translation_id: 360022411353
locale: es
sidebar_position: 2
created_at: '2019-04-29T20:13:47Z'
updated_at: '2025-11-25T16:04:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible para: [Empresa](../../../plans-billing/miro-plans/04-enterprise-plan.md),
    planes [Business](../../../plans-billing/miro-plans/06-business-plan.md) Configurado
    por: admins de empresa'
---

Miro es compatible con inicios de sesión únicos (SSO) a través de SAML 2.0.

Un proveedor de identificación SAML 2.0 (IDP) puede tomar muchas formas, incluido un servidor de Servicios de federación de Active Directory (ADFS). El ADFS es un servicio proporcionado por Microsoft como función estándar para Windows Server que proporciona inicio de sesión web con credenciales de Active Directory existentes.

Esta guía utiliza capturas de pantalla de **Server 2012R2**, pero es posible seguir pasos similares en otras versiones.

Primero, debes instalar ADFS en tu servidor. Cómo configurar e instalar ADFS está más allá del alcance de esta guía, pero puedes consultarlo en detalle en este [artículo de Microsoft](http://msdn.microsoft.com/library/gg188612.aspx).

Durante las pruebas, asegúrate de que la autenticación de tu estación de trabajo esté configurada con el mismo correo electrónico que estás usando para las pruebas, si no, ADFS no te permitirá iniciar sesión ni siquiera con la configuración y el perfil correctos.

> *Se recomienda enfáticamente configurar el SSO en una ventana en modo incógnito por separado del navegador.* De esta manera, mantienes la sesión en la ventana estándar, lo que te permite desactivar la autorización de SSO en caso de que algo esté configurado de forma incorrecta.

Si deseas configurar una instancia de prueba antes de activar el SSO en la producción, solicítala a tu Account Executive o representante de Ventas. Solo se agregará a esta instancia de prueba a quienes configuren SSO.

> **⚠️ Consulta aquí nuestro artículo principal sobre SSO** **para conocer las reglas, las funciones compatibles y la configuración opcional desde Miro.**

## Paso 1: agregar una relación de confianza para un usuario autenticado

1) Inicia sesión en el servidor ADFS y lanza la **consola de gestión de ADFS**.

2) Selecciona la carpeta de relación de **confianza para usuario** autenticado de **gestión de ADFS** y agrega una nueva relación de **confianza para** usuario autenticado estándar desde la barra lateral **de** Actions (acciones). Esto inicia el asistente de configuración para una nueva relación de confianza.

añadir_una_relación_de_confianza.jpg
Agregar una nueva relación de confianza

3) En la pantalla **de Seleccionar fuente de datos,** selecciona la última opción, I**ngresar datos sobre la relación manualmente.**

step_3.jpg
**Elige Enter Data About the Party Manually (ingresar datos sobre la relación manualmente)**

4) Introduce un **nombre para mostrar** que reconozcas en el futuro y cualquier nota que quieras dejar.

nombre_para_mostrar.jpg
Agregar un nombre para mostrar

5) Selecciona el botón de **perfil de ADFS FS (ADFS 2.0)**.

step_5.jpg

siguiente.jpg
Te pediremos que busques un certificado para encriptar y desencriptar los reclamos. Esto es opcional y se puede omitir presionando **Next (siguiente)**.

6) Marca la casilla con la etiqueta **Habilitar Soporte para el protocolo SAML 2.0 WebSSO**.
La URL del servicio será https://miro.com/sso/saml.

**Ten** en cuenta que no hay ninguna barra inclinada al final de la URL.

paso_6.jpg
Habilitar soporte para el protocolo SAML 2.0 WebSSO

7) Añadir una **relación de confianza** para usuario autentificado en `https://miro.com/`

paso_7.jpg
**Añadir un identificador de la relación de confianza para usuario autentificado**

*En la pantalla siguiente, puedes configurar la autentificación multifactor, pero esto queda por fuera del alcance de esta guía.*

rejecting_on_step_7.jpg
*Rechazar la configuración de autentificación multifactor*

8) Seleccionar el botón **Permit all users to access this relying party (Permitir a todos los usuarios el acceso a esta relación de confianza).**

paso_8.jpg
Permitir a todos los usuarios el acceso a la relación de confianza

En las dos pantallas siguientes, el asistente mostrará una descripción general de tus ajustes.

En la pantalla final, usa el botón **de Cerrar** para salir y abrir el editor **de Recla**mo de reglas.

paso_final.jpg
Terminar de agregar una relación de confianza para usuario autenticado

Asegúrate de que la configuración incluya **una afirmación firmada**.

## Paso 2: crear reglas de reclamo

Una vez creado el fideicomiso de la parte confiada, puedes crear las reglas de reclamación.
Por defecto, el editor de reglas de reclamación se abre una vez que has creado el fideicomiso.

1) Para crear una regla nueva, haz clic en **Add Rule (añadir regla).**

añadir_regla.jpg
Añadir una nueva regla

2) Crear una regla para **Enviar atributos LDAP como reclamos**.

plantilla_reclamo_de_reglas.jpg
Crear una regla

3) En la siguiente pantalla, ponle un nombre a la regla y usa **Active Directory** como tienda de atributos, trazada de la siguiente manera:

| Atributo LDAP | Tipo de reclamo saliente |
| --- | --- |
| Direcciones de correo electrónico | Dirección de email |
| Nombre otorgado | Nombre |
| Apellido | Apellido |

trazado_de_atributos_LDAP.jpg
Trazado de atributos LDAP

Haz clic en **OK** para guardar la nueva regla.

4) Crea otra regla nueva haciendo clic en **Añadir regla**, esta vez seleccionando **Transformar un reclamo entrante** como plantilla.

añadir_otra_regla.jpg
**Selecciona Transformar un reclamo entrante como plantilla**

5) Luego, ponle un nombre a la regla y establece los siguientes parámetros:

|  |  |
| --- | --- |
| **Tipo de reclamo entrante** | Dirección de correo electrónico |
| **Tipo de reclamo saliente** | ID de nombre |
| **Formato de ID de nombre saliente** | Correo electrónico |

establecer_parámetros_de_la_regla.jpg
Establecer los parámetros de la regla

Finalmente, haz clic en **OK** para crear la regla de reclamo, y luego **en O**K nuevamente para terminar de crear las reglas.

Con esto, completaste la configuración de ADFS. Después, simplemente habilita [la función SSO para tu cuenta de Miro](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md); tus usuarios finales podrán comenzar a usar SAML para autenticarse en Miro.

## Probar la configuración de SSO en Miro

1. Completa los pasos anteriores para configurar tus ajustes SSO.
2. Haz clic en el botón **Probar configuración SSO**.
3. Revisa los resultados:

1. Si no se encuentra ningún problema, se mostrará un mensaje de confirmación de que **la prueba de configuración SSO se ha realizado correctamente**.
2. Si se encuentran problemas, se mostrará un mensaje de confirmación **Prueba de configuración SSO fallida**, seguido de mensajes de error detallados para orientarte sobre lo que hay que arreglar.

![prueba-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Probar la configuración de SSO en Miro*
