---
title: Cómo instalar aplicaciones
article_id: 360017731093
translation_id: 360017731093
locale: es
sidebar_position: 4
created_at: '2019-02-11T10:12:46Z'
updated_at: '2025-08-05T07:54:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Personas: Todos los usuarios Planes: Todos los planes Plataformas: Navegador,
    aplicación de escritorio Los admins de equipo pueden restringir la instalación
    para los que no son admins. Los admins de empresa en el plan Enterprise pueden
    restringir aún más a solo aplicaciones aprobadas.'
---

Puedes ampliar la funcionalidad de Miro instalando aplicaciones desde el Marketplace de Miro. Este artículo te guía para instalar y desinstalar aplicaciones, entender los permisos de las aplicaciones y ofrece una visión general de la creación de integraciones personalizadas.

## Instalar aplicaciones desde el Marketplace de Miro

El [Marketplace de Miro](https://miro.com/marketplace/) es tu centro principal para descubrir y agregar aplicaciones para mejorar tu experiencia en Miro. Puedes instalar aplicaciones directamente desde tu tablero o visitando el sitio web del Marketplace.

![Miro_marketplace.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021611044242_Miro%20marketplace.jpg)*Marketplace de Miro*

Hay dos maneras principales para que los usuarios agreguen aplicaciones:

1. **Desde tu tablero:** Haz clic en el icono de **Herramientas, Medios e Integraciones (+)** en la barra de herramientas de creación, luego usa el cuadro de búsqueda "Buscar integraciones" en la pestaña del Marketplace. Si ves que tu aplicación ya está en la lista, solo haz clic para agregarla. También puedes explorar las aplicaciones disponibles desde este panel.
   ![marketplace-add-apps.png](../../../../../../docs/integrations-apps/integrations-basics/images/21260776452626_marketplace-add-apps.png)*Marketplace en la barra de herramientas de creación*
2. **Desde el sitio web del Marketplace:** También puedes ir directamente al sitio web del [Marketplace de Miro](https://miro.com/marketplace/) para explorar e instalar aplicaciones desde sus respectivas listas.

**Para los admins de empresa:**
Los admins de empresa en los planes aplicables también pueden instalar aplicaciones para todo su equipo a través de la configuración del equipo. Para hacer esto, navega a **Configuración de equipo** > **Aplicaciones e integraciones** > **Instalar aplicaciones**. Esta sección permite la gestión y el despliegue centralizados de aplicaciones a través del equipo.

![apps_and_integrations_page.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021832338450_apps%20and%20integrations%20page.jpg)*Sección de aplicaciones instaladas en la configuración de equipo para admins*

## Desinstalar aplicaciones

Puedes gestionar y desinstalar aplicaciones desde la configuración de tu equipo. Ten en cuenta que los usuarios que no son admins pueden tener restricciones para desinstalar aplicaciones, dependiendo de la configuración del equipo.

:::warning
Los usuarios que no son admins no pueden desinstalar aplicaciones si un admin no les permite instalarlas en la configuración del equipo.
:::

Para gestionar las aplicaciones de tu equipo, navega a **Configuración de equipo > Aplicaciones e integraciones**. Esta página enumera todas las aplicaciones instaladas actualmente para tu equipo o por ti personalmente.

![apps_settings.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021898097682_apps%20settings.jpg)*Aplicaciones e integraciones en la configuración de equipo*

Para desinstalar una aplicación, sigue estos pasos:

1. De la lista de **Aplicaciones e integraciones**, selecciona la aplicación que deseas eliminar.
2. Haz clic en **Desinstalar para el equipo** o **Desinstalar para mí**. La opción disponible dependerá de cómo se instaló la aplicación y de tus derechos administrativos.

![uninstall_an_app.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021797466258_uninstall%20an%20app.jpg)*La opción de desinstalar una aplicación*

## Permisos para la instalación de aplicaciones

Los admins de equipo y de empresa tienen varios controles para gestionar quién puede instalar aplicaciones y qué aplicaciones están disponibles para su organización, garantizando seguridad y cumplimiento.

Los admins de equipo pueden configurar si los miembros del equipo que no son admins tienen permitido instalar aplicaciones. Esta configuración se encuentra en **Configuración de equipo > Aplicaciones e integraciones** bajo las opciones de gestión de aplicaciones.

![allow_non-admins_to_install_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021903025170_allow%20non-admins%20to%20install%20apps.jpg)*Opción "Permitir que quienes no son admins instalen aplicaciones" en la configuración de equipo*

Para usuarios en el [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), los admins de empresa tienen acceso a controles más granulares. Pueden gestionar las **Aplicaciones aprobadas** a través de **Configuración de empresa** > **Aplicaciones**. Esta función permite a los admins crear una lista de aplicaciones aprobadas por la empresa, restringiendo a los usuarios de instalar aplicaciones que no estén en esta lista. [Obtén más información sobre la gestión del descubrimiento e instalación de aplicaciones para planes Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).

![Enterprise_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021890162962_Enterprise%20apps.jpg)*Gestión de aplicaciones aprobadas en la configuración de empresa Enterprise*

## Integraciones personalizadas y plataforma de desarrolladores

Si necesitas funcionalidad específica que no está disponible en el Marketplace de Miro, puedes crear tus propias soluciones personalizadas usando la [Plataforma para Desarrolladores de Miro](https://miro.com/api/). Esta plataforma ofrece herramientas robustas, incluidas API REST, plugins web e insertos, para ayudarte a construir integraciones poderosas adaptadas a tus necesidades.

Aquí hay puntos clave a considerar al desarrollar integraciones personalizadas:

- **Introducción:** Puedes comenzar a construir tu aplicación [creando un equipo de desarrolladores](https://developers.miro.com/). Los equipos de desarrolladores estándar están destinados a fines de desarrollo y pruebas y tienen ciertas limitaciones:
  - Hasta 5 usuarios en el equipo.
  - Hasta 3 tableros en el equipo.
  - Se muestra una marca de agua en los tableros.
  - La funcionalidad de exportación de tableros no está disponible.
- **Desarrolladores del Plan Enterprise:** Si tu organización está en un [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), puedes crear un equipo de desarrolladores como parte de tu suscripción. Estos equipos de desarrolladores no están sujetos a las limitaciones de los estándar y se benefician de todas las funciones de seguridad de nivel Enterprise. [Obtén más información sobre los equipos de desarrolladores para planes Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md).

Para obtener información adicional, asistencia y conectarte con otros desarrolladores, puedes explorar el [Foro de la Plataforma de Desarrolladores](https://community.miro.com/developer-platform-forum-57).
