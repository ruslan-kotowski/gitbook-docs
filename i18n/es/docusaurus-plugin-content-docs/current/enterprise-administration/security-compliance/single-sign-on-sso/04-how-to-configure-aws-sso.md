---
title: Cómo configurar SSO de AWS
article_id: 360014798100
translation_id: 360014798100
locale: es
sidebar_position: 4
created_at: '2020-07-01T20:03:44Z'
updated_at: '2025-02-26T11:33:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible para: [Empresa](../../../plans-billing/miro-plans/04-enterprise-plan.md),
    planes [Business](../../../plans-billing/miro-plans/06-business-plan.md) Configurado
    por: admins de empresa'
---

> *Se recomienda enfáticamente configurar el SSO en una ventana en modo incógnito por separado del navegador.* De esta manera, mantienes la sesión en la ventana estándar, lo que te permite desactivar la autorización de SSO en caso de que algo esté configurado de forma incorrecta.

Si deseas configurar una instancia de prueba antes de activar el SSO en la producción, solicítala a tu Account Executive o representante de Ventas. Solo se agregará a esta instancia de prueba a quienes configuren SSO.

> **⚠️ Consulta aquí nuestro artículo principal sobre SSO** **para conocer las reglas, las funciones compatibles y la configuración opcional desde Miro.**

## Requisitos previos

Necesitarás lo siguiente para configurar el acceso al SSO de AWS con Miro:

1. El acceso a la consola de AWS SSO con permisos de IAM para administrar aplicaciones.
2. Permisos de admin a nivel de empresa en los planes Enterprise o Business de Miro.

## Instrucciones de configuración

1. En la página de configuración de AWS SSO, agrega una nueva aplicación y búsqueda para **Miro**.    Al añadir la aplicación Miro, se pueden actualizar el nombre para mostrar y la descripción.
   catálogo_de_aplicaciones.jpg
   Catálogo de aplicaciones de AWS SSO
2. Inicia sesión en el panel de Miro en una ventana de navegador diferente.  Te recomendamos que uses una ventana diferente de navegador de incógnito./span>
3. En la parte superior derecha, haz clic en el icono del perfil y, luego, ve a **Settings** (Ajustes).  En el panel izquierdo, asegúrate de que se haya seleccionado el equipo correcto en el menú desplegable en la parte superior izquierda.
4. En el panel izquierdo, ve a **Enterprise integrations** (Integraciones de Enterprise) (los usuarios de planes Business tienen que ir a **Security** [Seguridad]) y activa la opción **Enable SSO/SAML** (Habilitar SSO/SAML).  Ingresa el siguiente valor para SAML Sign-in URL (URL de inicio de sesión SAML) de AWS SSO.

página_configuración_aplicaciones.jpg
Página de ajustes de aplicaciones del SSO de AWS

5. Descarga el archivo de metadatos SAML del SSO de AWS y copia y pega el Certificado X509 en **Key x509 Certificate** (Certificado Key x509).  Tu configuración de Miro ahora debería verse parecida a la siguiente.

ajustes_SSO_Miro.jpg
Ajustes de configuración SSO de Miro

6. En la configuración de SSO de Miro, ingresa el nombre de dominio del correo electrónico de tu empresa en el valor correspondiente a **Domains** (Dominios).  Asegúrate de haber agregado al menos un dominio de empresa.
7. Haz clic en **Save** (Guardar) para guardar los cambios.
8. Regresa a tu aplicación para Miro en la consola web del SSO de AWS.  En los metadatos de las aplicaciones, asegúrate de que aparezcan los siguientes valores. Deberían aparecer automáticamente si buscaste y agregaste la aplicación de Miro en lugar de crear una aplicación personalizada.
9. |  |  |
   | --- | --- |
   | **Campo** | **Valor** |
   | ACS URL de la aplicación | [https://miro.com/sso/saml](https://Miro.com/sso/saml) |
   | Audiencia SAML de la aplicación | https://miro.com/ |
10. Elige **Save Changes** (Guardar cambios).
11. [Asigna un usuario](https://docs.aws.amazon.com/singlesignon/latest/userguide/assignuserstoapp.html) a la aplicación en Application's Assigned Users (Usuarios asignados a la aplicación) de la consola del SSO de AWS.

¡Y eso es todo! La configuración de SSO ya está completa.

Si deseas habilitar también el aprovisionamiento automático para Miro, consulta [este artículo](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

## pruebas

Usa la siguiente sección para verificar la integración de SSO.  Antes de la verificación, asegúrate de que el usuario que realiza la verificación haya cerrado la sesión del SSO de AWS y Miro antes de realizar los siguientes pasos. Los usuarios no podrán iniciar sesión usando SSO a menos que el usuario exista en tu directorio, sea un miembro de tu plan Enterprise o Business en Miro y haya sido asignado a la aplicación./span>

### Verificación de SSO iniciado por IdP desde AWS SSO

1. Accede al portal del usuario final de AWS SSO mediante las credenciales de un usuario asignado a la aplicación de Miro.
2. En la lista de aplicaciones, elige la aplicación de Miro para comenzar un inicio de sesión en Miro.
3. Si se pudo realizar el inicio de sesión, estarás registrado en el panel de Miro.

### Verificación de SSO iniciada por proveedor de servicio desde Miro

1. Accede a [https://miro.com/login/](https://Miro.com/login/) y elige **Sign in with SSO** (Iniciar sesión con SSO).  Luego, ingresa tu correo electrónico laboral.
2. Se te redirigirá al portal del SSO de AWS, en el que debes escribir las credenciales de un usuario asignado a la aplicación en la consola del SSO de AWS.
3. Si el inicio de sesión fue exitoso, estarás registrado en el panel de Miro.

### También puedes probar en Miro

1. Completa los pasos anteriores para configurar tus ajustes SSO.
2. Haz clic en el botón **Probar configuración SSO**.
3. Revisa los resultados:
   1. Si no se encuentra ningún problema, se mostrará un mensaje de confirmación de que **la prueba de configuración SSO se ha realizado correctamente**.
   2. Si se encuentran problemas, se mostrará un mensaje de confirmación **Prueba de configuración SSO fallida**, seguido de mensajes de error detallados para orientarte sobre lo que hay que arreglar.![prueba-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*Prueba de configuración SSO desde Miro*

## Resolución de problemas

Por problemas generales, consulta la [Guía de resolución de problemas de AWS SSO](http://docs.aws.amazon.com/singlesignon/latest/userguide/troubleshooting.html).
