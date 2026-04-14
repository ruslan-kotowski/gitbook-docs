---
title: Registros de auditoría
article_id: 360017571434
translation_id: 360017571434
locale: es
sidebar_position: 1
created_at: '2019-02-11T10:09:04Z'
updated_at: '2026-03-12T09:21:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible para: Enterprise Plan Configurado por: admins de empresa'
---

Los registros de auditoría permiten a los admins de la organización con privilegios pertinentes rastrear la actividad de los usuarios en su organización de Miro. Los registros son extremadamente útiles cuando investigas un problema o necesitas un informe detallado de eventos importantes (por ejemplo, cambios en las configuraciones de seguridad global, invitaciones de nuevos usuarios o nuevos tableros creados).

:::note
Actualmente, los eventos se registran desde el momento de la creación de la suscripción a Enterprise y se almacenan durante 180 días por defecto:
a) Si mejoras a Enterprise desde un plan diferente, los eventos se registrarán desde el momento de la mejora.
b) Si migras algunos equipos a la suscripción Enterprise, sus datos se registrarán solo cuando formen parte de la suscripción.
:::

## Acceder a los registros de auditoría

Para acceder a los registros de auditoría, haz lo siguiente:

1. Ve a **Configuración de la empresa**.
2. En el panel izquierdo, haz clic en **Seguridad** > **Registros de auditoría**.
3. Puedes filtrar los registros de auditoría eligiendo un **Rango de fechas**, un **Responsable**, una **Categoría de eventos** y un **Evento** específico.

Haz clic en el botón Ver eventos para previsualizar los eventos que coinciden con tus criterios de filtrado. El tiempo se muestra en formato **ISO 8601**, en la zona horaria **local**. Puedes ver los detalles de un evento particular haciendo clic en los tres puntos en la columna de **Detalles**.

:::note
Solo los eventos que ocurrieron durante los últimos 90 días están disponibles para vista previa.
:::

## Exportar registros de auditoría

Puedes exportar registros en formato de archivo **CSV**.

En el archivo de exportación CSV, la fecha y hora del evento se proporcionan en formato ISO 8601, zona horaria UTC. No hay límite en el número de registros que se pueden exportar a la vez; sin embargo, cuanto más datos exportes, más tiempo llevará preparar el archivo para descargar. También ten en cuenta que las aplicaciones populares para trabajar con tablas tienen sus límites para el volumen de datos que pueden abrir.

Para exportar registros, haz clic en el botón **Exportar a CSV**.

La barra con los detalles de tu archivo de exportación aparecerá abajo. Cuando el archivo esté listo para descargar, podrás hacer clic en el botón Descargar CSV. El archivo estará disponible para descargar durante 24 horas.

:::note
Actualmente, solo un archivo de exportación está disponible para descargar por organización a la vez. Al hacer clic en el botón **Exportar a CSV** se reemplazará el archivo de exportación actual.
:::

## Acceder a los registros de auditoría mediante API

Los administradores pueden usar la [API del Registro de Auditoría](https://developers.miro.com/reference/audit-logs) o las [Integraciones SIEM](https://help.miro.com/hc/sections/4404757427090-Security-information-and-event-management-SIEM) soportadas para acceder y recopilar programáticamente datos de registros de auditoría.

## Eliminar registros de auditoría

Los administradores pueden establecer una política de retención para los registros de auditoría. Puedes elegir entre 30, 90, 180 o 365 días.

:::warning
Una vez que se eliminan los registros de auditoría, no se pueden recuperar.
:::

:::note
La retención indefinida de los registros de auditoría ha quedado obsoleta.
:::

Para establecer un período de eliminación, haz lo siguiente:

1. Ve a **Configuración de la empresa**.
2. En el panel izquierdo, haz clic en **Seguridad** > **Registros de auditoría**.
3. Bajo **Registros de auditoría**, haz clic en la pestaña de **Configuración**.
4. Elige una opción de la lista desplegable. Se te pedirá que confirmes tu elección.

## Eventos en los Registros de auditoría

Los registros de auditoría incluyen registros sobre las siguientes categorías de eventos:

**Administración**

- Cambio de nombre de la compañía
- Cambio o eliminación del logo de la compañía
- Creación de solicitud de acceso
- Solicitud de acceso rechazada
- Habilitar, deshabilitar métricas de actividad de usuarios en Estadísticas
- Habilitar, deshabilitar o cambiar configuración de inicio de sesión único (SSO/SAML)
- Habilitar, deshabilitar SCIM
- Generación de token para SCIM API
- Habilitar, deshabilitar notificaciones SCIM
- Habilitar, deshabilitar, cambiar [lista de admitidos](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Habilitar, deshabilitar el uso compartido con invitados fuera de los dominios permitidos
- Habilitar, deshabilitar el uso compartido [a través de enlace público](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Habilitar, deshabilitar el uso compartido [a través de enlace público para editar](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Habilitar, deshabilitar [la privacidad del equipo](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Habilitar, deshabilitar, actualizar la configuración de [dominio](../../canvas-25-admin-features/domain-control/01-domain-control.md)
- Habilitar, deshabilitar [bloquear usuarios desactivados](../../user-management/02-block-deactivated-users.md)
- Cambiar [la configuración de administración de solicitudes](../../user-management/09-request-management-on-enterprise-plan.md) (incluyendo cambiar el correo electrónico de ServiceNow o la URL del servicio de asistencia)
- Creación, eliminación de un equipo
- Cambio de nombre de un equipo
- Cambio, eliminación del logo de un equipo
- Cambiar las [preferencias de invitación del equipo](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Cambiar el [descubrimiento de equipos](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Habilitar, deshabilitar [invitados para un equipo](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Cambiar las [preferencias predeterminadas de compartir tableros](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Cambiar [la configuración predeterminada de uso compartido de proyectos](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Instalación, desinstalación de una aplicación
- [Aprobar, restringir una aplicación](../../../integrations-apps/integrations-basics/04-how-to-install-apps.md)
- [Moderación de Miro AI](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md)

**Gestión de usuarios**

- Invitar a un nuevo miembro del equipo
- Convertir un miembro en invitado
- Convertir un usuario en miembro con acceso completo
- Promover un usuario a admin de empresa, revocar admin de empresa
- Promover un usuario a admin de equipo, revocar admin de equipo
- Eliminar un usuario de un equipo o de una empresa (si un usuario deja un equipo, actúa como actor y también como objeto afectado)
- Revocar invitación
- Desactivar, reactivar un usuario
- Usuario se une a un equipo/empresa

**Tableros**

- Abrir un tablero
- Crear, eliminar, restaurar un tablero
- Renombrar un tablero
- Cambiar la descripción de un tablero
- Cambiar la portada de un tablero
- Mover un tablero a otro equipo
- Agregar un tablero a un proyecto, eliminar de un proyecto, mover a otro proyecto
- Cambiar el propietario de un tablero
- Compartir un tablero con un visualizador/autores del comentario/editor
- Eliminar a un usuario de un tablero
- Habilitar, deshabilitar, cambiar el [enlace público](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartir-tableros-a-traves-de-un-enlace-publico) del tablero
- Habilitar, deshabilitar, cambiar la [contraseña de un tablero público](../../../using-miro/sharing-boards/13-password-protection-for-public-boards.md)
- Habilitar, deshabilitar, cambiar la [compartición de un tablero con la empresa](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Habilitar, deshabilitar, cambiar la [compartición de un tablero con el equipo](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Exportar un tablero, descargar un archivo de un tablero.
- Estado creado
- Estado actualizado
- Estado eliminado
- Cargar un archivo (obsoleto, disponible en [registro de contenido](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md))

Ten en cuenta que el registro de auditoría **no** registra información relacionada con los cambios en los tableros.

**Plantillas**

- Abrir una plantilla
- Crear, eliminar, restaurar una plantilla
- Renombrar una plantilla
- Cambio de propietario de una plantilla
- Estado creado
- Estado actualizado
- Estado eliminado

**Proyectos**

- Crear, eliminar un proyecto
- Renombrar un proyecto
- Compartir un proyecto con un usuario, eliminar un participante del proyecto
- Habilitar, deshabilitar el uso compartido dentro del equipo para un proyecto
- Cambiar el propietario de un proyecto

**Inicios de sesión**

- Iniciar sesión
- No se pudo iniciar sesión
- Cerrar sesión
- Perfil bloqueado, desbloqueado

:::warning
Los eventos de inicio de sesión incluirán la actividad de [Usuarios desactivados](../../user-management/01-deactivated-users.md).
:::

**Detalles del perfil**

- Cambiar detalles del perfil
- Solicitar un cambio de dirección de correo electrónico
- Cambiar la dirección de correo electrónico

**Planes de acción**

- Crear un plan de acción
- Eliminar un plan de acción
- Crear una sección en el plan de acción
- Eliminar una sección del plan de acción
- Cambiar el propietario del plan de acción

**Miro AI**

- Usar la función de Miro AI

### Preguntas frecuentes

¿Hay una manera de extraer automáticamente los registros de auditoría?

Sí, puedes configurar la [aplicación de Miro para Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md) para acceder a los registros de Miro desde Splunk.
