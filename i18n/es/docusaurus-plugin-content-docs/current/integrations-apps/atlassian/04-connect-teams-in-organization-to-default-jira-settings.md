---
title: Conectar equipos en la organización a la configuración predeterminada de Jira
article_id: 26438407676434
translation_id: 26441962382610
locale: es
sidebar_position: 6
created_at: '2025-05-02T14:36:51Z'
updated_at: '2025-10-21T12:07:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quién puede hacerlo: admins de empresa ¿Qué planes?: Enterprise ¿Qué plataformas?:
    Navegador, Escritorio'
---

Los admins de empresa pueden conectar masivamente a los equipos de su organización para usar la configuración global de Jira, lo que anula las configuraciones especificadas a nivel de equipo.

## Requisitos previos

- Asegúrate de tener el rol de admin de empresa en Miro.
- Asegúrate de tener una conexión predeterminada a un [Conexión al centro de datos de Jira usando OAuth 2.0](https://help.miro.com/hc/articles/25753304280466).

## Conectar equipos a la configuración predeterminada de Jira

1. Desde tu panel de Miro, selecciona tu avatar en la esquina superior derecha y ve a **Consola de administración** | **Configuración**.
2. En la barra lateral izquierda, ve a **Apps e integraciones ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Apps** > pestaña **Administrar apps**.
3. Asegúrate de que **Permitir solo apps de la lista a continuación** esté habilitado.
4. En la columna **App**, para **Tarjetas de Jira** selecciona **Configuración**.
5. En **Agregar equipos a la instancia predeterminada**, selecciona cada equipo que deseas conectar o haz clic en **Seleccionar todos**.

   > ✏️ La lista solo muestra los equipos que no utilizan las configuraciones globales de la organización.
6. Haz clic en **Agregar <número de equipos> a predeterminado**.

   > ✏️ Los usuarios que no estén usando ya la instancia global de Jira en tu organización son migrados y deben reautenticarse.

   > ✏️ Los usuarios migrados desde otra instancia de Jira recibirán una instrucción para reautenticarse la primera vez que intenten realizar una acción relacionada con Jira en Miro.

## Preguntas frecuentes

**¿Los equipos seguirán utilizando la conexión global de Jira indefinidamente?**

No. Puedes cambiar la configuración de Jira para un equipo determinado más tarde.

**¿Qué equipos deberían utilizar la conexión global de Jira?**

Generalmente se prefiere utilizar la configuración de la organización, ya que requiere menos administración por tu parte. Si alguna de tus conexiones de equipo comparte las mismas configuraciones que la organización, te recomendamos integrar los equipos con las configuraciones predeterminadas de la organización por esta razón.
