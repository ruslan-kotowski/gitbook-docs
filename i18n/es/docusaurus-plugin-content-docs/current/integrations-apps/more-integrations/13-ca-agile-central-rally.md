---
title: CA Agile Central (Rally)
article_id: 360017731133
translation_id: 360017731133
locale: es
sidebar_position: 4
created_at: '2019-02-11T10:13:34Z'
updated_at: '2025-11-25T16:02:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: rally-cards
---

Aprovecha el software y la metodología líderes de CA Agile directamente en el tablero. Convierte tus tareas de CA Agile Central en tarjetas prácticas y disfruta de la priorización de tareas pendientes, la creación de mapas de historias y otras actividades de equipo que ayudan a tu equipo de manera consistente, y desarrolla proyectos de alta calidad rápidamente.

> **Disponible para:** [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)

## Conectar CA Agile

La autorización de CA Agile se realiza a través del protocolo OAuth 2.0 (concesión de código de autorización) y todas las solicitudes se envían a través de SSL. Hay dos niveles de conexión de tus datos de Miro y tu cuenta de CA Agile Central: el nivel del perfil de usuario y el nivel del equipo.

Es importante tener en cuenta que la conexión con CA Agile es unidireccional: CA Agile --> Miro. Puedes importar las tarjetas a un tablero de Miro y editarlas mediante el botón Origen, como se describe más adelante en la sección Editar tarjetas. No puedes editar directamente las tarjetas de CA Agile en Miro.

### Nivel del equipo

> **Configurado por:** admins de equipo

:::warning
Ten en cuenta que tendrás que usar cuentas de usuario de Rally diferentes en cada equipo de Miro para conectar la misma instancia de Rally.
:::

Para establecer la conexión a nivel del equipo, el admin de equipo deberá buscar la aplicación **CA Agile** en el [Marketplace de Miro](https://miro.com/marketplace/) e instalarla para el equipo: haz clic en **Obtener aplicación** y, a continuación, selecciona un equipo y haz clic en **Instalar y autorizar**.

![install_Rally_for_a_team.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416392594_install%20Rally%20for%20a%20team.jpg)
*Instalar Rally para un equipo*

También puedes instalar la aplicación desde un tablero:

1. En la barra Creación, selecciona **Herramientas, medios e integraciones** (**+**).Se abrirá el panel **Herramientas, medios e integraciones**.
2. En la pestaña **Herramientas**, busca y selecciona CA Agile.
   Se abrirá el panel **CA Agile**.

![ca-agile-entry-point.png](../../../../../../docs/integrations-apps/more-integrations/images/21537455155858_ca-agile-entry-point.png)
*Instalar la aplicación desde un tablero*

A continuación, abre la **configuración del equipo > Aplicaciones e integraciones** y **conecta** la integración desde allí. Si no tienes autorización en Rally, se te pedirá que inicies sesión en tu cuenta de Rally.

![connect_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416393874_connect%20Rally.jpg)
*Conectar la integración a nivel del equipo*

Durante esta configuración, se crea un webhook en el extremo de Rally que luego envía actualizaciones a Miro para las tarjetas importadas.

Cuando la integración se configura a nivel del equipo, cualquier miembro puede ver las tarjetas de Rally importadas por otros participantes en los tableros y el estado actual de estas.

Ten en cuenta que la cuenta de Rally que se usa al configurar la integración a nivel del equipo debe tener acceso a todos los proyectos de Rally desde los cuales se importarán las tarjetas. Si esta cuenta de Rally no podrá acceder a algún proyecto de Rally, las tarjetas importadas desde dicho proyecto no se actualizarán en el tablero y se mostrarán como congeladas para todos los usuarios del equipo.

### Nivel del perfil

> **Configurado por:** cada usuario

:::warning
Antes de conectar la integración, asegúrate de iniciar sesión en Rally en una pestaña del navegador separada.
:::

Si un usuario requiere la opción de importar tarjetas de Rally en el tablero mismo, entonces también tendrá que configurar la integración a nivel del perfil. Para conectar tu perfil de Miro, abre la [configuración del perfil](https://miro.com/app/account/profile/), cambia a **Integraciones**, busca **CA Agile Central (Rally)** y haz clic en **Conectar**:

![connect_Rally_on_profile_level.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429433746_connect%20Rally%20on%20profile%20level.jpg)
*Conectar la integración a nivel del perfil*

Cuando se establezca la conexión a nivel del perfil, el usuario podrá usar el ícono de Rally en su barra de herramientas y abrir el selector de biblioteca de Rally. Allí el usuario puede ver todos los elementos de Rally (historias de usuarios, tareas, defectos) disponibles para la cuenta de Rally que se utilizan para configurar la integración a nivel del perfil. En otras palabras, con el selector de Rally, el usuario podrá importar solo los elementos que tiene a su disposición en Rally.

## Agregar tarjetas de CA Agile al tablero

Para agregar una tarjeta al tablero, simplemente copia la dirección URL de la tarea y pégala en el tablero (también funcionan las [combinaciones de teclas](https://help.realtimeboard.com/support/solutions/articles/1000206698-shortcuts-hotkeys) estándar).

Para filtrar tareas o agregar tarjetas de forma masiva, elige **CA Agile** en la barra de herramientas Creación.

Verás el selector de CA Agile Central, donde puedes configurar los filtros de búsqueda, como proyecto, tipo, iteración, versión, etc. Elige una o varias y haz clic en **Exportar**:

![Rally_picker.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416397714_Rally%20picker.jpg)
*Selector de CA Agile Central*

Las tareas se agregarán automáticamente al tablero. Si el nombre de la tarea es largo, arrastra la parte inferior de la tarjeta para verlo completo.

*![Rally_cards_on_the_board.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398482_Rally%20cards%20on%20the%20board.jpg)
Tarjetas de Rally en el tablero*

> Ten en cuenta que la integración de Rally en Miro no ofrece la capacidad de crear o editar directamente tarjetas de Rally en Miro.

## Cómo editar tarjetas

Para editar el contenido de una tarjeta, haz clic en el enlace de origen en la tarjeta:

![Rally_card_source.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398866_Rally%20card%20source.jpg)
*El ícono de edición en la tarjeta*

La tarea de origen se abrirá en una pestaña nueva en la que se la puede editar. Todos los cambios se aplican a la tarjeta al instante.

## Deshabilitar la integración

Para eliminar la conexión a tus iteraciones de Rally, tendrás que **Deshabilitar** la integración y **Desinstalarla** en la **configuración del equipo > Aplicaciones e integraciones**.

![uninstall_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429436562_uninstall%20Rally.jpg)
*La opción para deshabilitar la integración*

## Posibles problemas y cómo resolverlos

1. *El selector de Miro-Rally no muestra algunos de mis proyectos*
   - Nuestra integración de Rally usa el [selector de SDK de Rally](https://rally1.rallydev.com/docs/saas/apps/2.1/doc/index.html#!/api/Rally.ui.picker.project.ProjectPicker) para rellenar los datos, solo funciona con proyectos en estado Abierto y, desafortunadamente, no es personalizable. Para mostrar un proyecto en el extremo de Miro, cambia su estado a Abierto.
2. *Las actualizaciones de las tarjetas o los campos en algunas tarjetas no se envían a Miro*- Si estás usando la integración de tarjetas de Rally con varios equipos de Miro, comprueba que todos los equipos estén conectados a tu instancia de Rally con una cuenta de usuario de Rally *diferente*. Es posible que el problema con las actualizaciones en el equipo elegido se deba a que las credenciales de conexión ya se usen en otro equipo de Miro. Vuelve a conectar la integración con un conjunto diferente de credenciales de usuario de Rally si es necesario.
3. *Al intentar abrir el selector de Rally en Miro, nunca termina de cargarse.*- Sigue los pasos de solución de problemas que se indican a continuación.

   1. Abre el menú Suscripción (`https://rally1.rallydev.com/#/subscription`).

   2. Haz clic en el menú desplegable **Acciones** y elige **Editar**.

   3. Desplázate hacia abajo hasta el campo **Orígenes permitidos de CORS**.

   4. Ingresa `https://miro.com,https://*.miro.com` (`http://miro.com`) en el campo.

   5. Haz clic en **Guardar y cerrar**.
