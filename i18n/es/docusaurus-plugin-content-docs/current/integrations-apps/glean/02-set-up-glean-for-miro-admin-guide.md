---
title: "Configurar Glean para Miro (gu\xEDa del admin)"
article_id: 27581463837330
translation_id: 27581463837330
locale: es
sidebar_position: 2
created_at: '2025-06-23T10:52:57Z'
updated_at: '2026-01-02T09:57:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Requisitos previos

1. Eres un **admin de Miro** y un **admin de Glean**.
2. En Glean, **registra un ID de Cliente OAuth.** Lee la [documentación de Glean](https://developers.glean.com/api-info/client/authentication/oauth) para más detalles.
3. Habilita la configuración de privacidad a nivel de usuario **Permitir que el historial de chat se guarde hasta 30 días**.

## Instalar la app de Glean

Para comenzar, instala la app de Glean desde el Marketplace de Miro para los equipos relevantes de tu organización.

1. Ve a la **configuración de tu empresa** y haz clic en **Apps & Integrations**.
2. En la pestaña de **Apps**, haz clic en **Add apps** para abrir el Marketplace.
3. Busca "Glean". También puedes encontrarlo pegando su ID de cliente en la barra de búsqueda: `1202342442818548396`.
4. Desde el perfil de la aplicación, selecciona dónde agregar la aplicación: ya sea para **Todos los equipos** o selecciona **Equipos específicos...**.
5. Revisa la página de permisos. La aplicación Glean es desarrollada y mantenida por Miro y no requiere permisos específicos.
6. Selecciona **Agregar** para completar la instalación.

## Configuración de inicio de sesión único (Okta)

Si tu organización utiliza Okta como su proveedor de inicio de sesión único (SSO), necesitas crear una aplicación web Okta OpenID Connect (OIDC) antes de continuar con las siguientes secciones.

1. Crea una nueva aplicación de Okta utilizando los pasos mencionados en la documentación [aquí](https://help.okta.com/en-us/content/topics/apps/apps_app_integration_wizard_oidc.htm).
   1. Selecciona **OIDC - OpenID Connect** como el método de inicio de sesión.
   2. Selecciona **Aplicación Web** como el tipo de aplicación.
   3. Asegúrate de que el **Token de actualización** esté habilitado en los ajustes de **Tipo de concesión** > **Concesiones principales**.
   4. Agrega `https://integrations.miro.com/api/external-auth/oauth2/callback` como las **URIs de redireccionamiento de inicio de sesión**.
   5. Selecciona **Guardar**.
2. Copia el **ClientId** y el **Client Secret** de la sección de Credenciales del Cliente. Estos serán necesarios en las siguientes secciones para completar la configuración de la integración.

## Configurar el inicio de sesión único (SSO)

Sigue estos pasos para configurar la aplicación:

1. Desde la página de **Apps & Integrations**, navega a **Gestionar aplicaciones**.
2. Encuentra "Glean" en tu lista de aplicaciones instaladas y haz clic en su **Configuración**. Si no ves la aplicación, búscala por el ID de cliente (`1202342442818548396`) y apruébala primero.
3. En la configuración, seleccionael **proveedor de inicio de sesión único (SSO)**.
   1. Okta
   2. Azure
   3. Google
4. Introduce los detalles requeridos de SSO.
   1. Okta: **URL de base de Glean, detalles de la app de Okta (URL del servidor de autorización**, **URL del token de acceso**, **ID de cliente**, **Secreto del cliente)**.
   2. Azure: **URL de base de Glean**.
   3. Google: **URL de base de Glean**.
5. Haz clic en **Guardar** para aplicar la configuración.

:::note
Si estás usando Azure, asegúrate de que tu admin de Microsoft Entra haya seleccionado "Consiento en nombre de tu organización" para la aplicación Glean en el centro de administración de Microsoft Entra, para permitir que los usuarios se autentiquen correctamente.
:::

## Configurar la consola de administración de Glean

Antes de usar Glean en Miro, necesitas configurar acceso basado en tokens OAuth en tu consola de administración de Glean.

1. Abre tu **Glean Admin console** y navega a **Configuración** > **Acceso de terceros (OAuth)**.
2. En la sección **OAuth configurado por IdP**, habilita **Habilitar OAuth de IdP para acceso de API**.
3. Haz clic en **Gestionar Configuración**, selecciona tu **proveedor de SSO**.
4. Completa los detalles del proveedor según tu proveedor de inicio de sesión único (SSO).
   - **Okta**
     - URL del servidor de autorización: `https://<subdomain>.okta.com`
     - ID(s) de cliente permitido(s): ID del cliente de la aplicación de Okta creada en la sección anterior.
     - El resto de los campos del formulario pueden dejarse vacíos.
   - **Azure**
     - Subdominio del emisor: `https://login.microsoftonline.com/<tenant-id>/v2.0`
     - ID(s) de cliente permitidos: `a49fdb25-3b5f-4d3b-bedf-6da7be2b4bf4`
   - **GSuite**
     - ID(s) de cliente permitidos: `1062019541050-pf2ndc9f3o4lrmkupj3cj0fep5hkecns.apps.googleusercontent.com`
5. Selecciona **Guardar** para aplicar la configuración.

> ⏰ **Nota:** Los cambios pueden tardar hasta 30 minutos en aplicarse en la consola de administración de Glean.

## Usar la app de Glean

Una vez que hayas instalado y configurado la app, los usuarios de los equipos designados podrán comenzar a usarla. La primera vez que un usuario abra la app de Glean en Miro, se le solicitará autenticarse.

1. Abre un tablero de Miro y haz clic en el ícono de Glean en la barra de herramientas para abrir el panel lateral.
2. Haz clic en **Conectar Glean** para iniciar la autorización.
3. Aparecerá un diálogo de autorización de inicio de sesión único.
4. Después de una autenticación exitosa, la interfaz de usuario de Glean aparecerá lista para su uso.

## Seguridad

Para obtener más información sobre datos y seguridad, consulta este [documento de seguridad](https://docs.google.com/document/d/1lGLF7eASQb2uMRmMEAaH-GzFhyz4UKfwMeqSQOSYPdM/edit?tab=t.0#heading=h.gu9ng058yy7y).
