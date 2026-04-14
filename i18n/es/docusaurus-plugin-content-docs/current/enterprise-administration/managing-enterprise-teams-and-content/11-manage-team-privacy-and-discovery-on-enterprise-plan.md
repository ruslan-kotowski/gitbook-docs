---
title: Gestiona la privacidad y el descubrimiento de equipos en el plan Enterprise
article_id: 360011821219
translation_id: 360011821219
locale: es
sidebar_position: 12
created_at: '2020-02-07T12:46:14Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: sharing-settings
availability:
  notes: 'Disponible para: plan Enterprise Rol requerido: admin de empresa'
---

Trabajar en una organización grande a menudo significa que el contenido y los usuarios quedan distribuidos entre múltiples equipos. Asegúrate de que todos tengan acceso a lo que necesitan permitiendo a los miembros de tu subscripción ver y unirse a los equipos relevantes.

### Descubrimiento de equipos

**El Descubrimiento de equipos es un ajuste a nivel del equipo que controla la forma en que los miembros de la organización pueden encontrar y unirse al equipo.** Para gestionar los ajustes de descubrimiento de un equipo, ve a **Ajustes de la empresa > Equipos** y, a continuación, haz clic en el equipo para el que quieras cambiar los ajustes. A continuación, selecciona la pestaña **Configuración**.

![lista-gestión-de-equipos.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921803038994_team-management-list.png) *Lista de equipos dentro de la configuración de la empresa*

> [⚠️](../../administration/user-management/02-invitation-settings.md)Los admins de empresa y de equipo pueden configurar el descubrimiento de equipos, siempre y cuando los admins del equipo tengan permitido invitar usuarios al mismo (también recibirán solicitudes de usuarios para unirse al equipo).

El descubrimiento de equipos tiene tres estados:

- **Oculto**: ningún miembro podrá encontrar el equipo a menos que se le invite a unirse a él
- Los miembros pueden unirse una vez que reciben la aprobación: el equipo es visible y los miembros pueden solicitar unirse
- **Abierto a los miembros**: el equipo es visible y los miembros pueden unirse de inmediato

Si un equipo tiene [restricciones en la lista de dominios permitidos](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)sólo los usuarios cuyos dominios de correo electrónico estén en la lista de permitidos del equipo podrán descubrirlo y solicitar unirse a él. Esta configuración garantiza que la descubribilidad del equipo siga las restricciones de dominio establecidas a nivel de equipo.

> Habilita nuestra función Descubrimiento de equipos junto con el [aprovisionamiento justo a tiempo](../user-management/13-user-provisioning-on-enterprise-plan.md)), y el equipo predeterminado que establezcas para los usuarios recién registrados también estará visible para que los usuarios existentes se unan.

![configuracion-descubrimiento-de-equipos.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780537234_team-management-discovery-settings.png)
*Ajustes de descubrimiento de equipos*

El Descubrimiento de equipos no afecta la manera en que los miembros ven a otros usuarios en tu suscripción.  Así que, a menos que esto se anule por medio de la Privacidad de equipo, los miembros podrán ver la lista completa de otros usuarios en los ajustes./span>

Los miembros de tu plan Enterprise podrán encontrar equipos a los que unirse abriendo el menú Equipos en la parte superior izquierda del panel y seleccionando ![icon-zoom-in.svg](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921803048338_icon-zoom-in.svg) **Unirse a un equipo**. Aparecerá una lista de equipos con la opción de **Unirse** o **Pedir Unirse**, dependiendo de la configuración de seguridad de cada equipo.

![gestión de equipos-unirse.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780544914_team-management-join.png) *Lista de equipos localizables*

### Privacidad del equipo

La **Privacidad de equipo** es una funcionalidad del nivel de empresa que establece la visibilidad tanto de los equipos como de los usuarios. Se encuentra en la Configuración de **la empresa** > **Seguridad** > **Compartir,** en la sección **Privacidad del equipo**.

![gestión-del-equipo-privacidad.pngConfiguración](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780547218_team-management-privacy.png)
*de la privacidad*

- Cuando se desactiva la Privacidad de equipo, los miembros de la subscripción pueden ver tanto la lista completa de usuarios como la lista de equipos detectables en los ajustes.  Es la condición predeterminada de las suscripciones del plan Enterprise garantizar que todos los miembros puedan encontrar contenido relevante y colaborar con otros usuarios para fomentar el intercambio de conocimientos, la transparencia y reducir la duplicación de trabajos./span>
- Cuando se activa, la Privacidad de equipo permite a los miembros de la subscripción ver solo los equipos a los que están invitados y a los demás usuarios de estos equipos.  Se puede utilizar cuando se trabaja con diferentes clientes en equipos separados, para garantizar que no sepan los unos de los otros. Con la Privacidad de equipo activada no es posible compartir tableros con toda la empresa con un solo clic/span>

### La Privacidad de equipo y el Descubrimiento de equipos trabajan juntos

En el nivel de equipos, la Privacidad tiene un nivel de prioridad superior al Descubrimiento. Verás una notificación sobre la falta de efectividad de la función de Descubrimiento de equipos. Aun así, puedes administrar sus opciones, las cuales entrarán en efecto una vez que se desactive la Privacidad de equipo.

> [✏️](../user-management/13-user-provisioning-on-enterprise-plan.md) Los ajustes tanto de la Privacidad de equipo como del Descubrimiento de equipos afectan la experiencia de los miembros de la subscripción y no tienen ningún impacto sobre el modo en que un usuario puede unirse a la subscripción en sí.
