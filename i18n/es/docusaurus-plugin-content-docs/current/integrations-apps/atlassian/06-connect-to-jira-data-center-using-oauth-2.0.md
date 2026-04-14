---
title: Conectar al Centro de Datos de Jira usando OAuth 2.0
article_id: 25753304280466
translation_id: 26513394914962
locale: es
sidebar_position: 8
created_at: '2025-05-06T09:05:53Z'
updated_at: '2025-05-21T09:27:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quién puede hacerlo: Admins de empresa con permisos de administrador del
    sistema Jira ¿Qué planes?: Enterprise ¿Qué plataformas: navegador, escritorio'
---

> La conexión al Jira Data Center usando OAuth 2.0 solo está habilitada a nivel organizacional.

## Requisitos previos

- Asegúrate de tener los siguientes permisos:
  - Permisos de admin del sistema Jira
  - Admin de empresa de Miro
- Crea un enlace de la aplicación OAuth 2.0 en Jira Data Center. Para aprender cómo, consulta (Externo) [Soporte para aplicaciones de Atlassian Jira](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Create%20an%20incoming%20link%20using%20application%20links).
  - Usa la siguiente URL de redirección cuando se te indique:
    https://integrations.miro.com/api/external-auth/oauth2/callback
  - Para usar webhooks automáticos, asegúrate de seleccionar **Administrador** para tu alcance.

## Conecta Miro con el Centro de datos de Jira usando OAuth 2.0

1. Desde tu panel de Miro, selecciona tu avatar en la esquina superior derecha y ve a (Enterprise) **Consola de administración**, o(Starter y Business) **Configuración**.
2. En la barra lateral izquierda, ve a **Aplicaciones e integraciones ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Aplicaciones** > **Administrar aplicaciones**  pestaña.
3. Asegúrate de que **Permitir solo aplicaciones de la siguiente lista** esté habilitado.
4. En la columna **App**, para **Jira Cards**, selecciona **Ajustes**.
5. Selecciona **Agregar nueva conexión**.
6. En **la configuración de Jira**, selecciona **Centro de datos de Jira**.
7. En **Método de autenticación**, selecciona **OAuth 2.0**.
8. Para **URL de Jira**, ingresa la URL de tu instancia de Jira.
9. (Opcional) Para hacer de esta conexión la conexión predeterminada para todos los equipos de tu organización, haz clic en **Establecer como predeterminada**.
10. Ingresa el **ID de Cliente** de Jira.
    **Más información**: Ver (Externo) [Configurar un enlace entrante](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
11. Ingresa el **secreto de cliente** de Jira.
    **Más información**: Ver (Externo) [Configurar un enlace entrante](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
12. Elige tu alcance.
    Para usar webhooks automáticos, elige **Admin** o **Administrador de sistema**.
13. (Opcional) Para obtener actualizaciones en tiempo real de Jira en Miro, marca **Crear webhook automáticamente**.
    > ✏️ Opcionalmente, puedes agregar el webhook manualmente más tarde.
14. Selecciona **Conectar**.
    > La primera vez que un usuario intenta realizar una acción relacionada con Jira, se le solicita autenticar. No necesitan autenticarse de nuevo.

## ¿Qué sigue?

Para ver y administrar tus instancias conectadas de Jira, ve a **Admin Console** | **Configuración** > **Aplicaciones e integraciones ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Administrar aplicaciones**. Luego, en la columna de **App**, para **Jira Cards** selecciona **Ajustes**.

Para aprender cómo conectar tus equipos a la instancia predeterminada de Jira, consulta [Conectar equipos de la organización a los ajustes predeterminados de Jira.](https://help.miro.com/hc/articles/26438407676434)

## Preguntas frecuentes

**¿Elegir Admin para el alcance requiere que todos los usuarios tengan privilegios de admin en Jira?**

No. El alcance del Admin significa que el admin es el nivel más alto que un usuario puede tener en Miro. El alcance está de todos modos limitado por usuario, dependiendo de sus permisos en Jira.

**¿Puedo conectar Jira Data Center con OAuth 2.0 a nivel del equipo?**

No. Solo a nivel de la organización.
