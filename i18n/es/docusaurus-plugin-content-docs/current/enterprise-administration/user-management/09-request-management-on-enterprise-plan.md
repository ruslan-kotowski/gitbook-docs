---
title: Administración de solicitudes en el plan Enterprise
article_id: 360017237379
translation_id: 360017237379
locale: es
sidebar_position: 9
created_at: '2020-10-27T12:09:40Z'
updated_at: '2026-02-19T11:00:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: access-request-management
availability:
  notes: 'Relevante para: plan Enterprise Quién puede hacerlo: admin de empresa'
---

En Miro, las solicitudes de licencias, acceso a equipos y organizaciones, e inicio de sesión único (SSO) se envían a los admins de empresa por correo electrónico de forma predeterminada. Con las funciones avanzadas de gestión de solicitudes, los admins de empresa pueden personalizar cómo se reciben y manejan estas solicitudes.

### Tipo de solicitud

Los tipos de solicitud se dividen en cuatro categorías:

- Solicitudes de unirse a tu organización
- Solicitudes de unirse a un equipo
- Solicitudes de licencia
- Solicitudes relacionadas con problemas de inicio de sesión único (SSO)

Conoce los diferentes escenarios de solicitudes para el plan Enterprise.

### Opciones de administración de solicitudes

Los admins de empresa tienen una variedad de opciones de administración de solicitudes, lo que les permite personalizar los procesos según el tipo de solicitud:

:::note
Las opciones para enviar correos electrónicos a todos los admins de empresa, o a admins de empresa específicos, incluyen a los admins de equipo.
:::

- Enviar correo electrónico a todos los admins de empresa
- Enviar correo electrónico a admins de empresa específicos
- Crear un ticket de servicio de asistencia
- Redirigir a una URL personalizada

## Configurar la administración de solicitudes

:::note
Para [gestionar las solicitudes de licencias directamente en Miro](04-license-requests-on-enterprise-plan.md), selecciona "**Enviar por correo electrónico a todos los admins de empresa**" o "**Enviar correo a admins específicos**". Recibirás todas las solicitudes de licencias futuras en tus configuraciones de solicitud de licencia.
:::

### Enviar por correo electrónico a todos los admins de empresa

Todos los admins de empresa recibirán una notificación por correo electrónico cuando un usuario genere una solicitud de acceso.

1. En **configuración de la empresa** ve a **Usuarios** > **Solicitudes de acceso** > **Gestión de solicitudes**.
2. Haz clic en el **tipo de solicitud** que deseas administrar.
3. Aparecerá una ventana emergente. Haz clic en el menú desplegable y selecciona **Enviar por correo electrónico a todos los admins de empresa**.

:::note
Las opciones para enviar por correo electrónico a todos los admins de empresa o a admins de empresa específicos incluyen a los admins de equipo.
:::

### Enviar correo electrónico a admins de empresa específicos

Los admins de empresa pueden especificar hasta 5 direcciones de correo electrónico. Solo los correos electrónicos especificados recibirán la solicitud. Los correos electrónicos no tienen que pertenecer a usuarios de Miro.

1. Ve a **Company** settings > **Users** > **Access requests** > **Request management**.
2. Haz clic en el **Type of request** que deseas administrar.
3. Aparecerá una ventana emergente. Haz clic en el menú desplegable y selecciona **Email specific company admins**.
4. Añade hasta 5 correos electrónicos. Haz clic en **Add** cada vez que ingreses una dirección de correo electrónico en el campo correspondiente.

:::note
Las opciones para enviar correos electrónicos a todos los Company admins, o a Company admins específicos, incluyen a los Team admins.
:::

### Crear un ticket de servicio de asistencia

Crea automáticamente un ticket de servicio de asistencia cada vez que un usuario genere una solicitud de acceso. Esta función es compatible actualmente con **ServiceNow** y **Jira Service Management**.

ServiceNow Jira Service Management

1. Configura los ajustes de correo electrónico para ServiceNow. Crea un elemento de catálogo para Miro en ServiceNow. Abre ServiceNow, ve a **Propiedades del sistema** > **Propiedades de correo electrónico** y habilita la recepción de correos electrónicos entrantes.

2. [Crea una acción de correo electrónico entrante](https://docs.servicenow.com/bundle/tokyo-servicenow-platform/page/administer/notification/task/t_CreatingAnInboundEmailAction.html). En el campo **De**campo **De**, bajo la línea **Solo los correos electrónicos de este remitente activarán esta acción de correo entrante**, introduce la dirección [notification@miro.com](mailto:notification@miro.com).

3. [Configura los valores de los campos desde el cuerpo del correo](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/notification/reference/r_SetFieldValsFromTheEmailBody.html) para ajustar configuraciones adicionales y establecer el proceso de conversión de un correo de Miro en un ticket de ServiceNow. Por ejemplo, puedes asignar un ticket recién creado a una persona en particular.

4. Ve a Miro, abre **configuración de la compañía** > **Usuarios** > **Solicitudes de acceso** > **Administración de solicitudes**, y selecciona **Crear un ticket en ServiceNow**. En el campo de correo electrónico, ingresa tu dirección de correo electrónico de ServiceNow.

1. Configura la configuración de correo electrónico para Jira Service Management. Desde tu proyecto de servicio, selecciona **Configuración del proyecto** > **Solicitudes de correo electrónico**. [Elige tu proveedor de servicio de correo electrónico y sigue las instrucciones para vincular Miro](https://support.atlassian.com/jira-service-management-cloud/docs/receive-requests-from-an-email-address/).

2. Ve a Miro, abre **Configuración de la empresa** > **Gestión de usuarios** > **Solicitudes de acceso** > **Administración de solicitudes**, y selecciona **Crear un ticket en Jira Service Management**. En el campo de correo electrónico, ingresa tu dirección de correo para Jira Service Management.

### Redirigir a una URL personalizada

El solicitante será redirigido a una URL de tu elección para los siguientes pasos.

1. En **Configuración de la compañía** ve a **Usuarios** > **Solicitudes de acceso** > **Administración de solicitudes**.
2. Haz clic en el **Tipo de solicitud**que deseas administrar.
3. Aparecerá una ventana emergente. Haz clic en el menú desplegable y selecciona **Redirigir a una URL personalizada**.
4. Introduce el enlace de redirección en el campo **URL personalizada**.

## Escenarios de solicitud

Los siguientes escenarios describen cómo se activan las diferentes solicitudes en Miro. Revisa los escenarios para decidir cómo te gustaría administrar cada tipo de solicitud.

|  |  |
| --- | --- |
| **Solicitudes para unirse a tu organización** | - Cuando un nuevo usuario solicita unirse a un equipo que es una suscripción gestionada por la empresa con [control de dominio](../canvas-25-admin-features/domain-control/01-domain-control.md) (a menos que el control de dominio esté configurado para capturar nuevos usuarios). |
| **Solicitudes de licencia** | - Cuando un [usuario Free Restrictivo](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) solicita una licencia Estándar o Completa (heredada). - Cuando un miembro solicita una licencia Estándar o Completa (legado) para un usuario con licencia gratuita limitada, a menos que a los miembros se les permita invitar a nuevos usuarios a la suscripción en la [configuración de invitaciones](03-invitation-settings-on-enterprise-plan.md). - Cuando un usuario Estándar o Completo (legado) solicita una licencia Avanzada. - Cuando un miembro intenta invitar o dar acceso de edición a un usuario con una licencia gratuita limitada. |
| **Solicitudes de unirse a un equipo** | - Cuando un usuario que no es admin intenta compartir un tablero con un usuario que *no* es miembro del equipo, las invitaciones para invitados están desactivadas en la [configuración de invitación](03-invitation-settings-on-enterprise-plan.md), y solo los admins pueden invitar a nuevos miembros al equipo. - Cuando un miembro al que no se le permite invitar a nuevos miembros intenta otorgar el rol de propietario o [copropietario](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) en un tablero específico a un usuario que no es miembro del equipo. - Cuando un usuario de Enterprise solicita unirse a un equipo [descubrible para usuarios en su organización](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md). - Cuando un [invitado](../../using-miro/sharing-boards/07-collaboration-with-guests.md) a tableros específicos en un equipo solicita unirse al equipo |
| **Solicitudes relacionadas con problemas de SSO** | - Cuando no se ha dado acceso a un usuario a Miro en IdP y tiene problemas para iniciar sesión a través de SSO. |

## Preguntas frecuentes

**¿Por qué sigo recibiendo correos electrónicos aunque configuré mis parámetros para crear tickets?**

Si los admins de equipo tienen permitido invitar a nuevos usuarios a un equipo en [la configuración de invitaciones](03-invitation-settings-on-enterprise-plan.md), recibirán las solicitudes de invitación relacionadas con este equipo por correo electrónico, aunque la administración de solicitudes esté configurada de otro modo. Los admins de empresa que también son admins de equipo también seguirán recibiendo estos correos.

**¿Cómo saben los admins de equipo si hay una solicitud para unirse a su equipo?**

Si los admins de equipo tienen permitido invitar usuarios a sus equipos, recibirán un correo sobre las solicitudes, independientemente de la configuración de administración de solicitudes.
