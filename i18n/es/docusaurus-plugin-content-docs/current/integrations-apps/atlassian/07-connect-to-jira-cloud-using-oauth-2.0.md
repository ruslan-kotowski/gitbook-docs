---
title: Conectar a Jira Cloud usando OAuth 2.0
article_id: 8588617184402
translation_id: 12984829399826
locale: es
sidebar_position: 7
created_at: '2023-08-09T16:12:00Z'
updated_at: '2025-10-21T12:18:25Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Disponible para: Jira Cloud incluyendo LDAP-protegido Planes: Starter, Business,
    Enterprise, Education Configurado por: (Enterprise) admin de empresa, o (Todos
    los demás planes) admin de equipo, con privilegios de admin de Jira'
---

:::warning
Si se presentan incidencias técnicas, por favor consulta nuestro artículo sobre [Posibles problemas y cómo resolverlos](https://help.miro.com/hc/articles/360017572654).
:::

:::tip
Aprende más sobre las tarjetas de Jira en los artículos [FAQ de las tarjetas de Jira](https://help.miro.com/hc/articles/360013463739)
:::

## Conectando Jira y Miro

### Cómo instalar la aplicación

1. Para habilitar la integración, en tu [panel](https://help.miro.com/hc/articles/360017571294-What-is-on-your-dashboard) en la esquina superior derecha, haz clic en tu avatar > **Integraciones y aplicaciones**:![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)
   *Gestionando tus aplicaciones*
2. Busca "Tarjetas de Jira" en la línea de **Búsqueda** y haz clic en el botón azul **Conectar** en la esquina inferior derecha del menú emergente.
3. Verás una ventana para **Agregar "tarjetas de Jira"**. Aquí debes confirmar la instalación o seleccionar el equipo en el que quieres instalar la integración (en caso de que seas miembro de varios equipos). Haz clic en **Agregar** para añadir la integración. En la parte superior del panel, verás el mensaje de confirmación de que la **App ha sido instalada:**
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)
   *El mensaje de confirmación*

### Conectar tu perfil de Jira

1. Haz clic en tu avatar en el panel nuevamente y ve a **Configuración > Equipos >** *Nombre de tu equipo* **> Apps & Integraciones > Tarjetas de Jira** y haz clic en **Conectar:
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)***La configuración de la integración*
2. Serás dirigido a la página de Jira para autorizar la conexión. Inicia sesión en Jira y haz clic en **Aceptar**.

### Conectar instancias de Jira a tu equipo de Miro

Con OAuth 2.0, ahora puedes conectar varias de tus instancias de Jira al mismo equipo y a los mismos tableros. Después de autorizar la aplicación en Configuración, verás la opción para **Conectar otra instancia.**

1. Inicia el selector de tarjetas de Jira desde la barra de herramientas de Creación (es posible que debas agregar la aplicación usando el botón **Más aplicaciones +**).
2. En el Selector, haz clic en **Configuración**.
3. Se te llevará a la sección de **Aplicaciones e integraciones** en tu configuración. Busca la opción para **Conectar otra instancia** y selecciona cualquier instancia adicional de Jira que quieras conectar.![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)*Configuración de las tarjetas de Jira en una cuenta de Miro*

Los admins de equipo también pueden ver todas las instancias que los miembros del equipo han conectado:

![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)

:::warning
Ten en cuenta que cada usuario final deberá autenticarse desde los tableros de Miro con cada instancia de Jira conectada si trabajan con las tarjetas de la instancia.
:::

> ✍️ Recuerda que solo una instancia a la vez puede estar activa para que los usuarios puedan extraer tarjetas de ella. Puedes seguir trabajando en las tarjetas existentes de las instancias inactivas en los tableros de Miro.

### Configurar actualizaciones en tiempo real desde Jira

Para obtener los beneficios completos de sincronización bidireccional en tiempo real, debes configurar webhooks para las instancias de Jira que agregues. Esto asegurará que cualquier actualización que realices en Jira se propague a Miro en tiempo real.

1. Inicia el selector de tarjetas de Jira desde la barra de herramientas de Creación (es posible que debas agregar la aplicación usando el botón **Más aplicaciones +**).
2. En el Selector, haz clic en **Configuración**.
3. Serás dirigido a la sección de **Aplicaciones e integraciones** de tu configuración.
4. En la sección de **Instancias conectadas** deberías ver una lista de las instancias que hayas agregado previamente.
5. Junto a cada instancia hay un botón para **Agregar webhook.** Al hacer clic en esto, se configurarán actualizaciones en tiempo real de Jira a Miro para esa instancia.
6. Si en el futuro deseas eliminar los webhooks de esta instancia, puedes seguir los pasos anteriores y hacer clic en el botón **Eliminar webhook** que se encuentra junto a las instancias conectadas para las cuales has agregado un webhook.

:::note
Ten en cuenta que debes ser admin en Miro *y* Jira para poder agregar webhooks a tus instancias.
:::

¡Después de eso, estás listo! Ahora puedes agregar tareas de Jira como tarjetas en la pizarra. Todos los cambios hechos en Jira se reflejan en las tarjetas de Jira en el tablero y viceversa.

## Desinstalar el complemento

Ve a **Configuración de equipo > Apps & Integraciones > Tarjetas de Jira** y haz clic en **Desinstalar para el equipo.**

:::tip
¡No olvides echar un vistazo al artículo principal sobre [cómo usar las tarjetas de Jira](https://help.miro.com/hc/articles/360017572434)!
:::
