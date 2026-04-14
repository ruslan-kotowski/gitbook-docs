---
title: Solicitudes de licencias en el plan Enterprise
article_id: 17693037972370
translation_id: 17693037972370
locale: es
sidebar_position: 4
created_at: '2024-03-15T08:43:14Z'
updated_at: '2026-02-19T10:46:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: access-request-management
availability:
  notes: 'Disponible para: Plan Enterprise Rol requerido: admin de empresa o admin'
---

Gestiona todas las solicitudes de licencias desde un solo lugar. Al recibir solicitudes de licencias directamente en Miro, puedes simplificar los procesos de uso y aprobación de licencias dentro de tu organización.

## Configuración de solicitudes de licencias

Dentro de la configuración de **Solicitudes de acceso**, encontrarás un resumen de todas las **solicitudes de licencias** actuales. Estas solicitudes de licencias se inician cuando un usuario requiere una mejora de un licencia Free a una licencia Avanzada, Estándar o Completa (anterior).

Los detalles de la solicitud de licencia incluyen:

- El nombre del usuario para el que es la solicitud de licencia
- El nombre del grupo de facturación (si lo hay) al que se asignará al usuario
- El nombre del solicitante
- La fecha de la solicitud

Las solicitudes pueden ser presentadas por la persona que necesita la mejora de plan o en nombre de otra persona. Aprende sobre los diferentes escenarios de mejora de plan para el Enterprise Plan.

:::note
Para recibir solicitudes de licencias directamente en Miro, actualiza tus preferencias de [administración de solicitudes](09-request-management-on-enterprise-plan.md).
:::

## Cómo aceptar o denegar solicitudes de licencias

:::note
Todas las solicitudes caducarán automáticamente y se eliminarán a los 30 días.
:::

1. Ve a tu configuración de Miro.
2. Haz clic en **Empresa**.
3. Bajo **Usuarios**, haz clic en **Solicitudes de acceso**.
4. Selecciona la pestaña **Solicitudes de licencias**. Aquí puedes ver todas las solicitudes de licencias pendientes.
5. Bajo la columna **Acciones**, haz clic en el check (**✓**) para aceptar, o en la cruz (**x**) para declinar la solicitud.
6. (opcional) Para aceptar solicitudes de licencia en bloque, junto a la columna **Nombre**, haz clic en la casilla de verificación para seleccionar todas las solicitudes, y luego haz clic en **Aprobación masiva**.
7. Cuando aceptes o rechaces solicitudes, se abrirá un modal con los detalles del solicitante junto con para quién es la solicitud de licencia.
8. Haz clic en **Aprobar** para aprobar la solicitud, o en **Denegar** para rechazar la solicitud. Cuando aceptes o deniegues una solicitud, se eliminará de tu resumen de solicitudes de licencia.
9. Una vez que la solicitud de licencia sea aprobada, el usuario será mejorado de una licencia Free Restricted a una licencia Advanced, Standard, o Full (legacy).

## Escenarios de mejora de licencia

Ciertas acciones o eventos en Miro llevan a los usuarios a enviar solicitudes para mejorar su plan de licencia. Los escenarios descritos a continuación explican cómo estas solicitudes se inician para los usuarios del plan Enterprise. Una vez aprobadas, la licencia del usuario se actualizará de una Free Restricted a una Advanced, Standard, o Full (legacy). Los usuarios mantendrán su pertenencia a los mismos equipos de los que formaban parte previamente.

:::note
Para ver tu uso actual de licencias, ve a **Gestión de usuarios** > **Usuarios activos**.
:::

|  |  |  |
| --- | --- | --- |
| **Tipo de usuario** | **Acción** | **Escenario** |
| **Miembros existentes (licencia gratuita limitada)** | Crear un tablero o proyecto | El usuario con licencia gratuita limitada intenta crear un nuevo tablero o proyecto dentro de un equipo |
| Acceso para editar | El usuario con licencia gratuita limitada solicita permiso para editar un tablero |
| Invitado a editar | Un miembro existente solicita acceso de edición para el usuario de Free Restricted |
| Propietario del tablero | El usuario de Free Restricted es asignado al rol de [propietario del tablero](../../getting-started/start-here/05-roles-in-miro.md) por un admin de equipo |
