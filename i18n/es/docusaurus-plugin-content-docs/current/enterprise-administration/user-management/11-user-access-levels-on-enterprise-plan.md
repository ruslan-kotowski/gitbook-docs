---
title: Niveles de acceso de los usuarios en el plan Enterprise
article_id: 360017571514
translation_id: 360017571514
locale: es
sidebar_position: 11
created_at: '2019-02-11T10:09:11Z'
updated_at: '2026-02-19T10:32:42Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

El nivel de acceso que tiene un usuario en tu plan Enterprise depende de su tipo de licencia y de su rol en Miro.  Verifica qué nivel de acceso tienen tus usuarios en la siguiente guía.

## Acceso del usuario en el programa de licencias flexibles (FLP)

Consulta en la tabla el tipo de licencia y el rol en Miro, para entender los derechos de acceso de tu tipo de usuario.

Con las licencias gratuitas, el usuario se actualiza automáticamente [tan pronto como edita o crea un tablero, recibe una invitación para editar un tablero, la copropiedad del tablero o se lo agrega a un](../../using-miro/sharing-boards/16-projects.md) proyecto como editor.

Obtén más información sobre el [Programa de licencias flexibles](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) y [la gestión de licencias en el Programa de licencias flexibles](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

|  |  |  |  |  |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  | **Admin de empresa** | | | admin de equipo | | | Miembro | | | Invitado | |
| Con acceso completo | Gratuita | Gratuita limitada | Completa | Gratuita | Gratuita limitada | Con acceso completo | Gratuita | Gratuita limitada | Gratuita | Gratuita limitada |
| Administrar la configuración de la empresa | **✔** | **✔** | **✔** | **✘** | **✘** | **✘** | **✘** | **✘** | **✘** | **✘** | **✘** |
| Administrar la configuración del equipo | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✘** | **✘** | **✘** | **✘** | **✘** |
| Crear tableros y proyectos | **✔** | actualización automática | **✘** | **✔** | actualización automática | **✘** | **✔** | actualización automática | **✘** | **✘** | **✘** |
| editar tableros compartidos | **✔** | actualización automática | **✘** | ✔ | actualización automática | **✘** | **✔** | actualización automática | **✘** | ✔  *por suscripción | **✘** |
| Visualizar y comentar en tableros compartidos | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** |

*El acceso de edición para invitados debe estar habilitado desde el lado de Miro y habilitado en la configuración de la empresa por el admin de empresa.  Solicita más detalles a tu persona de contacto de Miro.

## Acceso de usuario en licencias no flexibles (no FLP)

Consulta en la tabla el tipo de licencia y el rol en Miro, para entender los derechos de acceso de tu tipo de usuario.

|  |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- |
|  | **Admin de empresa** | | admin de equipo | | Miembro | | **Invitado** |
| Con acceso completo | Gratuita Restringido | Con acceso completo | Gratuita Restringido | Con acceso completo | Gratuita Restringido | Gratuita |
| Administrar la configuración de la empresa | ✔ | ✔ | **✘** | **✘** | **✘** | **✘** | **✘** |
| Administrar la configuración del equipo | ✔ | ✔ | ✔ | ✔ | **✘** | **✘** | **✘** |
| Crear tableros y proyectos | ✔ | **✘** | ✔ | **✘** | ✔ | **✘** | **✘** |
| editar tableros compartidos | ✔ | **✘** | ✔ | **✘** | ✔ | **✘** | **✘** |
| Visualizar y comentar en tableros compartidos | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |

## Tipos de licencia

El [Programa de licencias flexibles (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) incluye el beneficio adicional de licencias **gratuitas** ilimitadas, así como la capacidad de bajar de categoría las licencias a gratuitas restringidas en cualquier momento.

|  |  |  |
| --- | --- | --- |
| **Con acceso completo** | **Gratuita (solo FLP)** | **Gratuita limitada** |
| El usuario tiene derechos totales para [ver, comentar y editar,](../../using-miro/sharing-boards/01-board-access-rights.md) así como la capacidad de crear tableros. | El usuario puede [ver y comentar](../../using-miro/sharing-boards/01-board-access-rights.md) y su categoría se actualiza automáticamente a una licencia **completa** una vez que [edita o crea un tablero, recibe una invitación para editar un tablero, la copropiedad de un tablero o se lo agrega a un](../../using-miro/sharing-boards/16-projects.md) proyecto como editor. | Los usuarios solo pueden [ver y comentar](../../using-miro/sharing-boards/01-board-access-rights.md), pero son parte del equipo y pueden ver todos los tableros compartidos. Pueden solicitar una actualización de licencia |

## Roles de Miro

Los roles en Miro definen el nivel de acceso de un usuario a la configuración de tu plan Enterprise.

:::note
Los admins de empresa y los admins de equipo son miembros siempre y tienen los mismos permisos que los miembros.
:::

|  |  |  |  |
| --- | --- | --- | --- |
| **admins de empresa** | **Admins de equipo** | **Miembros** | **Invitados** |
| **Puede** ver todos los equipos y administrar la configuración del equipo y de la empresa. | **Puede** ver y administrar la configuración de un equipo específico. | **puedes** [ver, comentar y editar tableros](../../using-miro/sharing-boards/01-board-access-rights.md)  **no puedes** gestionar la configuración del equipo o de la empresa | **Puede** [ver, comentar y/o editar](../../using-miro/sharing-boards/01-board-access-rights.md) tableros compartidos (según el [modelo de licencias](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md)).  **No puede** crear ni poseer tableros, ver otros equipos y detalles de la empresa, administrar la configuración del equipo o de la empresa, o solicitar una licencia. |

## Preguntas frecuentes

**¿Cómo bajo la categoría de la licencia de un usuario?**

En las suscripciones FLP para empresas, los admins de empresa pueden reducir la licencia de un usuario a Free limitada en Configuración de la empresa > **Usuarios** > **Todos los usuarios** o **Equipos**, seleccionar el equipo del que forma parte el usuario y, a continuación, buscarlo en la lista.

**Para ser miembro de dos equipos, ¿necesito tener una licencia en cada equipo?**

Si los equipos son parte de una suscripción de Enterprise, solo necesitas una licencia. Si los equipos están asociados con diferentes suscripciones, necesitas una licencia en cada equipo.

**¿Qué tipo de licencia debe tener un admin?**

Los admins de los planes del FLP pueden tener una licencia completa, gratuita o gratuita con restricciones.  Los admins de planes que no sean FLP pueden tener una licencia gratuita limitada o completa.
