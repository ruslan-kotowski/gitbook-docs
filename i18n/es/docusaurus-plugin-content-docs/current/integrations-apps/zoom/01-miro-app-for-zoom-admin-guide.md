---
title: "Aplicaci\xF3n de Miro para Zoom (gu\xEDa del admin)"
article_id: 360022039379
translation_id: 360022039379
locale: es
sidebar_position: 1
created_at: '2021-05-28T04:43:09Z'
updated_at: '2025-02-26T11:51:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: zoom
---

La aplicación de Miro para Zoom permite que los equipos organicen una sala de reuniones digital integral y que colaboren de manera eficaz durante las reuniones y los talleres con Miro desde Zoom.  La aplicación ofrece las capacidades de colaboración en Miro desde Zoom y simplifica especialmente la incorporación de invitados. Para quienes son nuevos en Miro, ofrecemos pizarras virtuales con acceso sin registro.

Los Admins de Zoom y Miro pueden usar esta guía a fin de habilitar la experiencia para sus usuarios.

:::note
Consulta la [Guía del usuario de la aplicación de Miro para Zoom](02-miro-app-for-zoom-user-guide.md).
:::

> **Disponible para:** todos los planes Miro, todos los planes Zoom
> *Para los planes Business y Enterprise de Zoom, es posible que el admins tenga que aprobar previamente la app Miro
> **Disponible en**: versión de escritorio

## Cómo habilitar la experiencia de la aplicación en Zoom

### Habilitar el descubrimiento de aplicaciones

1. Inicia sesión en el portal web de Zoom como admin con el privilegio de editar los ajustes de la cuenta.
2. En el panel de navegación, haz clic en **Account Management** (Administración de cuenta) y, luego, en **Account Settings** (Ajustes de cuenta).
3. Haz clic en la pestaña **Zoom Apps** (Aplicaciones de Zoom).
4. Verifica que el **botón Zoom Apps Quick Launch** (Inicio rápido de aplicaciones en Zoom) esté habilitado.  Esto permite a los usuarios de tu cuenta ver el botón Zoom Apps ![mceclip0.png](../../../../../../docs/integrations-apps/zoom/images/21017682787474_mceclip0.png) en el cliente de escritorio.
5. Si el ajuste está deshabilitado, haz clic en el conmutador para habilitarlo. Si aparece un cuadro de diálogo de verificación, haz clic en **Activar** para verificar el cambio.

Además, Zoom tiene documentación adicional sobre cómo habilitar las aplicaciones de Zoom solo para grupos de usuarios específicos.  Para obtener más información, visita el centro de ayuda de Zoom aquí/span>[.](https://support.zoom.us/hc/articles/360061555152)

inicio_rápido_de_aplicaciones_de_Zoom.jpg
Habilitación del botón de inicio rápido de aplicaciones de Zoom

Esto habilitará las aplicaciones de Zoom en la barra superior del cliente principal de Zoom y en la barra inferior de los clientes de reuniones para los usuarios de tu cuenta.

### Cómo preaprobar la aplicación en Zoom

Si eres un admin de Zoom de un plan Zoom Business o Enterprise, es posible que tengas que preaprobar la aplicación de Miro [aquí](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) para que los usuarios tengan acceso a ella.

![pre-aprobar_aplic.miro.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653155474_pre-approve%20Miro%20app.jpg)*Preaprobar la app Miro*

### Seleccionar los usuarios en la cuenta que pueden instalar la aplicación

Además de preaprobar la aplicación de Miro, puedes seleccionar qué usuarios o grupos pueden instalarla.

autorizar_usuarios_para_instalar_la_aplicación.jpg
/span>Seleccionar usuarios y grupos que pueden instalar la aplicación de Miro

Una vez que apruebes la aplicación de Miro y la instales en la cuenta de la empresa, los usuarios podrán acceder a ella e instalarla desde el cliente de Zoom.

Consulta la [documentación de Zoom](https://support.zoom.us/hc/articles/360061555152) para obtener más información.

## Cómo habilitar la experiencia de la aplicación en Miro

> **Configurado por:** Admins de empresa en plan Enterprise

Si estás en [un plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) y limitaste la instalación solo a las aplicaciones aprobadas, asegúrate de incluir la aplicación de Miro para Zoom en tu lista de apps aprobadas. Puedes hacerlo en **Company settings (ajustes de empresa) > Apps (aplicaciones) > Manage apps (gestionar aplicaciones**). Puedes hacer esto si pegas la identificación de cliente 3074457354625507111 en la búsqueda y habilitas la aplicación para la instalación.

aprobar_Zoom_en_el_plan_Enterprise.jpg
Aplicaciones aprobadas en los ajustes de empresa

## Cómo los usuarios pueden instalar la aplicación

Los usuarios pueden encontrar la aplicación de Miro para Zoom en el [Zoom Marketplace](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) o el [Miro Marketplace](https://miro.com/marketplace/zoom-app/).

El primer paso del proceso de instalación es autorizar la aplicación de Miro para Zoom.

instalar_aplicación_miro_para_Zoom.jpg
Permitir que Miro acceda a tu cuenta de Zoom/span>

Una vez autorizada, la app redirigirá a los usuarios a su app de escritorio Zoom y mostrará la app Miro recién instalada. **Ten en cuenta que tendrán que iniciar sesión en su cuenta de Zoom para añadir la app**.

Los usuarios de Miro tendrán que **iniciar sesión** para ver sus tableros.  Esto los redireccionará al navegador de su sistema, en el que se les pide que inicien sesión en Miro o que autoricen directamente la aplicación en Miro. Pueden optar por instalar la aplicación para cualquier equipo al cual tengan acceso.

instalar_Zoom_para_un_equipo_de_Miro.jpg
Instala la aplicación para uno de tus equipos de Miro/span>

Luego, redirigiremos a los usuarios a la aplicación de escritorio de Zoom, en la que verán su panel de Miro, incluidos todos sus equipos y tableros existentes.

![Miro_tablero_en_Zoom.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653159442_Miro%20dashboard%20in%20Zoom.jpg)*Los usuarios podrán seleccionar un tablero de su panel y abrirlo dentro de Zoom*

## Comprensión de los ajustes de acceso para compartir tableros

Los usuarios pueden definir los permisos apropiados para compartir un tablero en una reunión de Zoom.  Pueden elegir entre cuatro opciones: **Cualquiera en Zoom puede editar/comentar/ver** o **Privado** (lo que significa que la configuración para compartir será la misma que la establecida en el lado de Miro).

ajustes_uso_compartido_inserciones_tablero.jpg

*Configuración de ajustes de acceso para tu tablero*

Las opciones de ajustes de acceso seguirán los controles de acceso para toda la organización.  Si tienes la función de compartir enlaces públicos restringida para inserciones de tableros en el [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), esa opción no estará disponible para los usuarios. Más información: [Cómo administrar la política de uso compartido de Enterprise respecto de las integraciones insertadas](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)./span>

edición_pública_desactivada.jpg
/span>El admin de empresa desactivó la edición pública

## Preguntas frecuentes

1. *¿A qué datos accede la app Miro para Zoom?*
   - La app Miro para Zoom solicita información sobre el perfil del usuario para asociar un tablero a un usuario determinado. Nuestra aplicación **no** accede al contenido de las reuniones, como archivos de vídeo, audio, chat o reuniones y, por lo tanto, no aparece en el notificador de aplicaciones activas de Zoom.
2. *¿Se puede instalar la app en tabletas o dispositivos móviles?*
   - No, la app Miro para Zoom sólo está disponible para escritorio.
3. *¿Para qué sistema operativo funciona Zoom Apps?*
   - Mac OS y Windows.
4. *¿Qué versión de Zoom es necesaria para utilizar las apps de Zoom?*
   Versión: 5.7.3.
