---
title: "Gesti\xF3n de aplicaciones"
article_id: 4404659741458
translation_id: 4404659741458
locale: es
sidebar_position: 2
created_at: '2021-08-03T15:46:50Z'
updated_at: '2026-01-29T10:00:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: apps-management
---

Aprende a gestionar aplicaciones y permisos en organizaciones y equipos.

> **Relevante para:** plan Business, plan Enterprise
> **¿Quién puede hacerlo?:** admins de equipo, admins de empresa

### ¿Quién puede gestionar las aplicaciones?

La gestión de aplicaciones a nivel organizacional solo está disponible en el plan Enterprise para admins de empresa. La gestión de aplicaciones del equipo está disponible en los planes Business y Enterprise para admins de equipo y de empresa.

### Añadir aplicaciones para una organización o para equipos específicos

Agrega y autoriza aplicaciones para todos los usuarios de una organización o para equipos específicos dentro de tu organización desde los controles de gestión de aplicaciones.
Ve a **Configuración de la empresa** > **Aplicaciones e integraciones** > **Aplicaciones**. Desde esta sección, los admins de empresa pueden agregar aplicaciones para todos los equipos o equipos específicos.

![apps-access.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803476626_apps-access.png)*Control de la gestión de aplicaciones en la Configuración de la empresa*

Ingresa el nombre de una aplicación o la ID del cliente en la barra de búsqueda. Selecciona una aplicación de la lista desplegable y haz clic en **Agregar**.

![add-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780909714_add-app.png)*Agregando una aplicación desde la Configuración de la empresa*

Puedes añadir la aplicación para todos los equipos de la organización o elegir equipos específicos. Si una aplicación ya se añadió para algunos equipos, verás la etiqueta correspondiente. Si vuelves a añadir la aplicación para un equipo, los miembros del equipo necesitarán volver a autorizar la aplicación. Haz clic en **Añadir** para terminar.

![add-apps-where.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780917010_add-apps-where.png)
*Seleccionar equipos para los que se instalará la aplicación de Google Drive*

Si añades una aplicación para todos los equipos, también se agregará a los equipos recién creados.

### Aplicaciones predeterminadas

Algunas aplicaciones se agregaron de forma predeterminada para los usuarios. Pueden requerir autorización adicional o inicio de sesión individual. Estas aplicaciones predeterminadas son: [Box](../../integrations-apps/more-integrations/05-box-legacy.md), [Dropbox](../../integrations-apps/more-integrations/06-dropbox.md), [Google Drive](../../integrations-apps/google/05-google-drive.md), [OneDrive](../../integrations-apps/microsoft/06-onedrive.md), [Smartsheet](../../integrations-apps/more-integrations/15-smartsheet-app-for-miro.md), [Azure Cards](../../integrations-apps/microsoft/03-azure-cards.md), [Jira Cards](../../integrations-apps/atlassian/03-jira-cards.md),[Brandfetch](https://miro.com/marketplace/brandfetch/), [Google Images](../../integrations-apps/google/06-google-images.md), [Slack](../../integrations-apps/more-integrations/14-slack.md). Estas aplicaciones no se agregarán previamente si no están en la lista aprobada por la empresa. Puedes gestionar esta lista si eres admin de empresa.

### Preautorizar las aplicaciones para una organización

Si añades una aplicación, también puedes autorizarla previamente al mismo tiempo. Si un admin agrega y autoriza previamente una aplicación, los usuarios de la organización podrán comenzar a usarla de inmediato. Es posible que de igual forma se requiera el inicio de sesión individual en un servicio de terceros en ciertas aplicaciones.

Esta función está disponible solo para las aplicaciones creadas con el Miro Web SDK. El SDK web de Miro permite extender la funcionalidad de Miro. Es una caja de herramientas para crear aplicaciones potentes que se ejecutan en un tablero de Miro.

### Aprobar aplicaciones para la gestión de usuarios individuales

De forma predeterminada, los usuarios pueden agregar cualquier aplicación para su equipo. Los admins de empresa pueden restringir la gestión de aplicaciones del usuario para permitir que sus equipos agreguen solo algunas apps.

Los admins de empresa pueden habilitar o limitar la posibilidad de agregar ciertas aplicaciones para sus usuarios yendo a **Configuración de la empresa** > **Aplicaciones e integraciones** > **Aplicaciones** > **Administrar aplicaciones** y activar la opción **Permitir que los miembros agreguen solo aplicaciones de la siguiente lista**.

![manage-apps.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780921490_manage-apps.png)*Limitar la adición de aplicaciones aprobadas en el plan Enterprise*

Si se activa la limitación, los usuarios de Enterprise solo pueden agregar las aplicaciones que hayan sido aprobadas. Para aprobar una aplicación para los usuarios, habilítala desde el control junto a ella o pega una ID de cliente en el campo correspondiente a fin de aprobar una aplicación desarrollada de forma interna.

Para restringir una aplicación agregada previamente, encuentra la aplicación en la lista y asegúrate de que el control junto a ella esté deshabilitado. Ten en cuenta que los usuarios de todos los equipos de Enterprise no podrán usar la aplicación si está restringida.

Si una aplicación está restringida en tu organización, los usuarios podrán enviar [solicitudes de uso de aplicación a los admins de empresa](03-app-request-flow.md).

Los usuarios pueden ver las aplicaciones aprobadas en el Marketplace de los tableros de Miro almacenados en el plan Enterprise.

### Permitir o restringir la instalación de aplicaciones en los equipos

Los admins de empresa y de equipo también pueden gestionar el uso de aplicaciones a nivel de equipo: pueden permitir o restringir a los miembros del equipo para que agreguen nuevas aplicaciones para el equipo. La configuración se realiza para cada equipo por separado.

![add-apps-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780928914_add-apps-team.png)*Aplicaciones e integraciones en la configuración del equipo*

Aprende más sobre [las aplicaciones e integraciones de Miro.](../../integrations-apps/integrations-basics)
