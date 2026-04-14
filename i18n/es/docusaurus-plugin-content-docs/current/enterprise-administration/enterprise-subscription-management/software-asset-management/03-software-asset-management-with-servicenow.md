---
title: "Gesti\xF3n de activos de software con ServiceNow"
article_id: 360021758459
translation_id: 360021758459
locale: es
sidebar_position: 3
created_at: '2021-05-20T05:00:32Z'
updated_at: '2025-02-26T11:53:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Analiza y personaliza el uso de tu subscripción a escala con la ayuda de la integración de ServiceNow y Miro. La integración permite obtener la lista de usuarios no activos y desactivarlos desde la aplicación de gestión de activos.

> **Disponible para: [Plan Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configurado por:** admins de empresa**

## Características admitidas

La integración otorga acceso a las siguientes características:

- **Descargar suscripciones**
  - Obtén una lista del uso de subscripción del usuario y la cantidad de licencias asignadas en tu subscripción a Miro Enterprise.
- **Reclamar suscripciones**
  - Desactiva usuarios en tu plan Miro Enterprise según su uso de la subscripción.

## Pasos para la configuración

### integración

1. En ServiceNow, ve al módulo **SaaS License (licencia SaaS)** y selecciona **la** opción **Direct Integration Profiles (perfiles de integración directa)**, luego haz clic en New (nuevo):

   módulo_licencia_saas.jpg
   Módulo de licencia SaaS

   > ✏️ En caso de que el módulo de **Licencia Saas** no esté presente en tu instancia de ServiceNow, tendrás que instalarlo siguiendo estos pasos:
2. Busca **el perfil de integración de Miro** Enterprise:

   perfil_de_integración_de_Miro_Enterprise.jpg
   Perfil de integración de Miro Enterprise
3. Verás dos subflujos predefinidos para **Descargar suscripciones** y **Reclamar suscripciones:**
   download_subscription_sybflow.jpg
   *Descargar Subflow de suscripción*

   reclamar.jpg
   *Reclamar subflujo de suscripción*

### Cómo crear una nueva conexión

1. Para crear una nueva Conexión ve a **Credenciales y Conexiones** > **Alias de Conexión y Credenciales** y haz clic en **Nuevo**.
   nuevo_alias.jpg
   *La opción de crear un nuevo Alias de Conexión y Credencial*

  Haz clic en el enlace **Create New Connection & Credentials** (Crear nueva conexión y credenciales):

create_connection.jpg
Conexión y alias de credenciales

Para el subflujo de **Descarga de suscripciones**, tendrás que brindar **el ID de cliente** y **el Secreto del cliente.**

diálogo_crear_conexión.jpg
Creación de conexión y credencial

2. Para obtener el**ID de cliente** y el **Secreto de cliente** **de**  **,** en Miro ve a **Configuración > Configuración del perfil > Tus apps** y selecciona **Crear nueva app.**

![](../../../../../../../docs/enterprise-administration/enterprise-subscription-management/software-asset-management/images/23921803379090_image.png)*Crea una nueva app en la configuración de tu perfil*

3. Configura el **nombre de la app**, selecciona un equipo y haz clic en **Crear app.** Ten en cuenta que necesitas tener un [equipo de Desarrolladores](../../managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md).

4. 4. En la página de la aplicación, en la sección **Permissions (Permisos)**, tendrás que marcar la opción **organizations:read (organizaciones:leer)** y hacer clic en **Install app and get OAuth Token (Instalar la aplicación y obtener el token de OAuth).**

5. 5. Selecciona un equipo que sea parte de tu organización Enterprise e instala la aplicación.

6. Copia el**ID de cliente** y el **secreto de cliente****de**  .

Para el subflujo **Reclamar suscripciones** tendrás que proporcionar un token de **API SCIM**. Para obtener un token de API SCIM, en Miro accede a la consola de admins y ve a **Apps e integraciones** > **Integraciones empresariales** > **Aprovisionamiento SCIM** y copia el token en **Token de API**.

## Personalización del uso de la suscripción

De manera predeterminada, **el umbral de la última actividad** está configurado en 60 días.  Para cambiarlo, navega a la sección Reclamation Rules (reglas de reclamos) y selecciona la regla de Miro, luego podrás modificar el umbral de la última actividad de la siguiente manera:

umbral_última_actividad.jpg
Umbral de la actividad más reciente

## Posibles dificultades y cómo resolverlas

Al intentar instalar la app para un equipo, aparece el mensaje de error "No hemos podido instalar esta app. No puedes instalar esta aplicación. Sus alcances no están disponibles en tu plan actual".
- Este es el comportamiento esperado cuando se instala la app en un equipo de desarrollo, ya que el equipo de desarrollo no tiene acceso a los alcances a nivel de organización. Querrás instalar la aplicación bajo uno de tus equipos Enterprise, en los que sí tiene acceso a los alcances de la organización para la integración de ServiceNow.

error_instalación_aplicación.jpg
El error cuando se instala la aplicación para un equipo de desarrolladores
