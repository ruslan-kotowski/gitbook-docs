---
title: Gestión de licencias en el Programa de Licencias Flexibles (PLF)
article_id: 360018622159
translation_id: 360018622159
locale: es
sidebar_position: 5
created_at: '2020-12-29T10:44:01Z'
updated_at: '2026-02-23T18:22:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Relevante para: plan Enterprise'
---

Obtén información sobre la gestión de licencias en el Programa de licencias flexibles (PLF), incluidas qué opciones de gestión de licencias están disponibles para nuevos usuarios y cómo convertir licencias existentes.

:::tip
Si eres nuevo en licencias del PLF, te recomendamos leer primero [Programa de Licencias Flexibles](03-flexible-licensing-program-flp.md) y [Niveles de acceso del usuario en el plan Enterprise](../../user-management/11-user-access-levels-on-enterprise-plan.md) para comprender cómo funcionan juntos nuestros modelos de licencias, tipos de licencias y roles de Miro.
:::

## Cómo asignar licencias a nuevos usuarios

Miembros Invitados Visitantes

Según la configuración por defecto para licencias de tu empresa, a los nuevos miembros se les asignan licencias Free o licencias gratuitas limitadas. Para establecer una licencia predeterminada para nuevos miembros en tu suscripción, comunícate con tu persona de contacto en Miro.

Los nuevos miembros reciben la licencia predeterminada:

- cuando son invitados por miembros que no son admins
- automáticamente a través de [Just-in-Time provisioning](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), [control de dominio](../../canvas-25-admin-features/domain-control/01-domain-control.md) o [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)

Los admins de empresa también tienen la opción de seleccionar una licencia para los miembros invitados.

- selecciona **Gratis** si quieres que los usuarios tengan la opción de editar (se mejorarán a una licencia Standard o Full (legado) tan pronto como editen o creen un tablero, se les invite a editar un tablero, se les otorgue la copropiedad del tablero o se les agregue a un [proyecto](../../../using-miro/sharing-boards/16-projects.md) como editores)
- selecciona **Gratis Limitado** para invitar al miembro sin derechos de edición

Los invitados a un tablero siempre reciben una licencia **Gratis**. Aprende cómo [invitar invitados en un plan Enterprise](../../../using-miro/sharing-boards/07-collaboration-with-guests.md).

[Los visitantes](../../../using-miro/sharing-boards/08-collaboration-with-visitors.md) de tableros compartidos públicamente son gratuitos y no tienen licencias.

## Cómo mejorar o cambiar a plan inferior las licencias

> **Quién puede hacerlo:** Admins de empresa

Las licencias **Free** se mejoran automáticamente a una licencia Standard o Full (legacy) tan pronto como el usuario crea o edita un tablero.

Gratuita limitada a Standard o Full (legado)  Standard o Full (legado) a Gratuita limitada Convertir licencias de manera masiva

Las licencias gratuitas limitadas se pueden mejorar a una licencia estándar o con acceso completo de forma manual por los admins de empresa, o como parte de la [automatización del flujo de trabajo de Enterprise](../enterprise-workflow-automation/01-enterprise-workflow-automation.md).

Para mejorar una licencia gratuita limitada a una licencia con acceso completo:

1. Abre **Equipos** o abre **Preferencias de organización** > **Usuarios** > **Todos los usuarios** > **Usuarios activos**.
2. Haz clic en el icono de **tres puntos** (**...**) junto a un usuario de licencia gratuita limitada.
3. Selecciona **Cambiar a miembro estándar**.

Las licencias con acceso completo se pueden bajar de categoría a una licencia gratuita limitada si los admins de la empresa desean limitar el acceso del usuario y liberar licencias adicionales con acceso completo.

Los miembros con acceso completo no pueden bajar de categoría a una licencia gratuita, ya que las licencias gratuitas solo se asignan a nuevos usuarios.

Realiza lo siguiente para bajar de categoría una licencia con acceso completo a una licencia gratuita limitada:

1. Abre **Equipos** o abre **Configuración de la organización** > **Usuarios** > **Todos los usuarios** >**Usuarios activos**.
2. Haz clic en el icono de **tres puntos** (**...**) junto a un usuario con licencia completa.
3. Selecciona **Cambiar a gratuito limitado**.

Para convertir varias licencias a la vez:

1. Abre **Configuración de la organización** > **Usuarios** > **Todos los usuarios** > **Usuarios activos**.
2. Selecciona individualmente a todos los usuarios cuyas licencias desees convertir o aplica filtros para seleccionar usuarios. Puedes seleccionar hasta 50 usuarios.
3. Haz clic en **Acciones en bloque** y selecciona una nueva opción de licencia.
