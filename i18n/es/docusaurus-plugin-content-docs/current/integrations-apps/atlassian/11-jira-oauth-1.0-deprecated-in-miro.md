---
title: OAuth 1.0 de Jira obsoleto en Miro
article_id: 28738797627538
translation_id: 28739476844050
locale: es
sidebar_position: 13
created_at: '2025-08-13T12:34:44Z'
updated_at: '2025-10-20T14:48:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Personas: Admins de empresa Planes: Starter, Business, Enterprise, Education
    Plataformas: Navegador, Escritorio'
---

La autenticación OAuth 1.0 de Jira se volverá obsoleta a partir de agosto de 2025.

Si tu organización ya actualizó a OAuth 2.0 de Jira, puedes ignorar este artículo. No se requiere ninguna acción por parte de tu admin de empresa. Puedes verificar con tu admin de empresa que tu organización esté utilizando OAuth 2.0.

:::warning
Si tu organización no ha actualizado a OAuth 2.0, entonces tu integración de Jira con Miro, incluyendo Jira Cloud, Server y Data Center, puede verse interrumpida.
:::

Solo los admin de empresa pueden mejorar equipos en su organización.

En caso de interrupción, la sincronización entre Miro y Jira se detiene hasta que tu organización actualice a la autenticación OAuth 2.0. Las tarjetas de Jira existentes permanecen en tus tableros de Miro.

La interrupción significa que la importación no está disponible, las tarjetas no se actualizan, los detalles no se pueden cargar y crear y actualizar un planificador no está disponible.

Para evitar interrupciones, Miro recomienda que el admin de empresa actualice a Jira OAuth 2.0 de inmediato.

:::tip
Los admin pueden Comprobar tu versión de OAuth.
:::

## ¿Por qué OAuth 1.0 es obsoleto?

Atlassian ha discontinuado y ya no ofrece soporte para el protocolo de autenticación OAuth 1.0.

**Más información:** Consulta (externo) [OAuth 1.0a para APIs REST (Obsoleto)](https://developer.atlassian.com/cloud/jira/platform/jira-rest-api-oauth-authentication/).

## Verifica tu versión de OAuth

Como admin de equipo Enterprise, o admin de plan Starter o Business, puedes verificar si tu equipo está usando OAuth 1.0 o OAuth 2.0.

Sigue estos pasos:

1. Desde el panel de Miro, haz clic en tu avatar en la esquina superior derecha y selecciona **Consola de administración**.
2. Ve a **Equipos** > **[Nombre del equipo]**.
3. Haz clic en **Apps**.
4. Busca y haz clic en **Tarjetas de Jira**.
5. Ve a **Configuración de administración** > **Configuración de Jira**.
   La configuración indica qué versión de OAuth está utilizando tu equipo.
6. (Opcional) Repite los pasos 1-5 para otros equipos que quieras verificar.
7. Notifica a tu/tu(s) admin(s) de empresa acerca de cualquier equipo que no esté utilizando OAuth 2.0.

## Encuentra a tu admin de empresa

Para identificar a tu(s) admin(s) de empresa, sigue estos pasos:

:::note
(Enterprise) Si la privacidad del equipo está habilitada, los que no son admin de empresa no pueden ver las listas de miembros.
:::

1. Ve a **configuración del perfil del equipo** en Miro.
2. Abre la página de **Usuarios**.
3. Haz clic en **Roles adicionales**.
4. Encuentra usuarios con el rol de **Admin de empresa**.

:::tip
Para asegurarte de que tu equipo mejore a OAuth 2.0 y evite posibles interrupciones, comparte este artículo con tu(s) admin(s) de empresa.
:::

## Mejora a OAuth 2.0 para admins de empresa

Como admin de empresa, tienes los siguientes recursos para ayudarte a actualizar tu organización a OAuth 2.0:

- [Conectar a Jira Cloud usando OAuth 2.0](https://help.miro.com/hc/articles/8588617184402)
- [Conectar a Jira Data Center usando OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
- [Conectar equipos en la organización a la configuración por defecto de Jira](https://help.miro.com/hc/articles/26438407676434)

## Solución provisional

Si OAuth 2.0 no es una opción para tu organización en este momento, Miro proporciona una [solución provisional utilizando OAuth 1.0](https://help.miro.com/hc/articles/27689156602514).

Sin embargo, Miro recomienda actualizar a OAuth 2.0 para un método de autenticación más seguro y preparado para el futuro, que siga los estándares actuales de Atlassian.

## Ayuda adicional

Si tú o tu admin de empresa tienen preguntas, contacta al [soporte de Miro](https://help.miro.com/hc/articles/360020185799).
