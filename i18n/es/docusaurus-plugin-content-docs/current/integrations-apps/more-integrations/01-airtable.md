---
title: Airtable
article_id: 360012807619
translation_id: 360012807619
locale: es
sidebar_position: 1
created_at: '2020-03-24T12:09:00Z'
updated_at: '2025-08-05T07:33:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Personas: Todos los usuarios de Miro, usuarios con planes de pago de Airtable
    Planes de Miro: Todos los planes Plataformas: Navegador'
---

¡Lleva el poder de la visualización de pizarras a tu trabajo con Airtable! Puedes exportar los datos de Miro a Airtable e insertar tableros de Miro en las bases de Airtable para verlos, comentarlos y editarlos directamente desde Airtable.

## Exportar datos de tableros de Miro a Airtable

La integración de Airtable Sync te permite exportar datos (por ejemplo, notas adhesivas, tarjetas) de tus tableros de Miro y organizarlos en Airtable. Para obtener más información sobre cómo configurar y usar esta función, visita la [documentación oficial de Airtable](https://support.airtable.com/docs/airtable-sync-integration-miro).

## Insertar tableros de Miro en las bases de Airtable

### Instalar la aplicación de Miro en Airtable

:::warning
La aplicación de Miro para Airtable **no** está disponible en el navegador **Safari**.
:::

Los editores de bases en Airtable pueden instalar la aplicación de Miro. Para hacerlo:

1. Abre tu base de Airtable y haz clic en **Extensiones** en la esquina superior derecha.

   ![Airtable extensions button in the top right corner.](../../../../../../docs/integrations-apps/more-integrations/images/21017651877394_Airtable%20extensions.jpg)
   *Botón de extensiones en la esquina superior derecha de una base de Airtable.*
2. Haz clic en **Añadir una extensión**.

   ![Add an extension option in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647938834_add%20an%20extension.jpg)
   *La opción para añadir una nueva extensión.*
3. Busca "Miro" en el Marketplace de Airtable y haz clic en **Añadir**.

   ![Miro app in Airtable Marketplace.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933714_Miro%20in%20Airtable.jpg)
   *Aplicación de Miro en el Marketplace de Airtable.*

### Agregar tableros existentes de Miro a las bases de Airtable

Una vez que la aplicación de Miro esté añadida a tu base de Airtable, haz clic en **Añadir un tablero** en la sección de la aplicación de Miro que aparece en tu panel de extensiones.

![Add a Miro board button in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651876498_add%20a%20Miro%20board.jpg)
*Agregando un tablero de Miro a través de la aplicación de Miro en Airtable.*

Aparecerá un selector de tableros de Miro. Si aún no has iniciado sesión en Miro en tu navegador, se te pedirá que te registres o crees una cuenta de Miro.

Después de seleccionar un tablero, establece los permisos para compartir cómo aparecerá en Airtable mediante el menú desplegable. Tienes tres opciones:

- **Cualquiera puede ver:** Cualquiera en Airtable puede [ver](../../using-miro/sharing-boards/01-board-access-rights.md) el contenido del tablero insertado.
- **Cualquiera puede comentar:** Cualquiera en Airtable puede [hacer comentarios](../../using-miro/sharing-boards/01-board-access-rights.md) en el tablero insertado. (Nota: Esta opción no está disponible para tableros almacenados en Miro [plan Free](../../plans-billing/miro-plans/09-free-plan.md).
- **Privado:** El tablero se ajustará a su configuración de uso compartido existente tal como se haya configurado en Miro.

  > ✏️ Para los usuarios del [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) de Miro, tu configuración de acceso respetará los controles de acceso de toda la organización, lo que podría implicar que algunas opciones para compartir estén restringidas. Más información: [Gestión de la política de uso compartido del plan Enterprise para integraciones insertadas](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).

![Sharing settings options when adding a Miro board to Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651879826_board%20access%20in%20Airtable.jpg)
*Ajustes de uso compartido cuando se añade un tablero de Miro a Airtable.*

El tablero de Miro insertado aparecerá entonces en tu base de Airtable, donde podrás verlo, comentarlo o editarlo según los permisos configurados.

![Embedded Miro board within an Airtable base.](../../../../../../docs/integrations-apps/more-integrations/images/21017651872402_Miro%20board%20in%20Airtable.jpg)
*Un tablero de Miro insertado en Airtable.*

Para reemplazar un tablero insertado por otro diferente, haz clic en el icono de engranaje (**Configuración**) de la aplicación de Miro en Airtable, selecciona **Elegir un tablero** y elige otro tablero del selector de Miro.

![Replacing an embedded Miro board in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647932690_replacing%20a%20board.jpg)
*Reemplazando un tablero de Miro insertado en Airtable.*

### Crear nuevos tableros de Miro desde Airtable

Para crear un nuevo tablero de Miro directamente desde Airtable:

1. En la sección de la aplicación Miro dentro de Airtable, haz clic en **Añadir tablero** (o **Elegir un tablero** si ya hay uno insertado y lo estás reemplazando).
2. En el seleccionador de Miro, selecciona la opción para crear un **Nuevo tablero**.

![Creating a new Miro board from the picker within Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651880466_add%20a%20new%20board%20to%20Airtable.jpg)
*Creando un nuevo tablero de Miro desde el selector en Airtable.*

El nuevo tablero se creará en tu cuenta de Miro y se insertará en tu base de Airtable.

### Eliminar tableros de Miro de Airtable

Para eliminar un tablero de Miro insertado de tu base de Airtable, necesitas eliminar o reconfigurar la extensión de la aplicación de Miro dentro de esa base. Haz clic en el menú desplegable de la aplicación de Miro en el panel de extensiones y elige eliminar o gestionar la extensión.

![Deleting the Miro app from Airtable extensions panel.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933074_deleting%20the%20app.jpg)
*Eliminación de la aplicación de Miro del panel de extensiones de Airtable.*
