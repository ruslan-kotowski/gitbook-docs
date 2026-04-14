---
title: Miro para Confluence
article_id: 360020712594
translation_id: 7618394363410
locale: es
sidebar_position: 3
created_at: '2022-09-13T18:17:36Z'
updated_at: '2026-03-12T09:15:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Disponible para: todos los planes de Miro; Confluence Cloud (inserción en
    Miro), Confluence Cloud/Servidor/DC (inserción en Confluence) Quién puede hacerlo:
    admin de Confluence'
---

Miro y Confluence trabajan juntos con la sincronización bidireccional para garantizar que obtengas el contenido más actualizado de ambas plataformas, donde sea que trabajes.

## Cómo funciona Miro con Confluence

Inserta tableros de Miro y documentos de Confluence, y haz un seguimiento de los cambios con la sincronización instantánea. Puedes establecer niveles de acceso de inserción para que los usuarios correctos tengan acceso a la información adecuada en todo momento.

Insertar documentos de Confluence en tableros de Miro

Insertar tableros de Miro en documentos de Confluence

## Insertar documentos de Confluence en tableros de Miro

Puedes insertar documentos de Confluence en Miro simplemente pegando un enlace en el tablero de Miro. Ten en cuenta que **para insertar documentos de Confluence en Miro es necesario usar Confluence Cloud.**

Cuando pegas un enlace de Confluence en un tablero de Miro, aparece como un [enlace inteligente de Miro](https://help.miro.com/hc/articles/360017730993). Cuando pegues un enlace de Confluence por primera vez, deberás hacer clic en **Conectar** para autorizar el acceso de Confluence.

:::warning
Por motivos de seguridad, no mostramos los detalles de un enlace de Confluence en tableros públicos de Miro, y los usuarios solo pueden ver el título de un enlace de Confluence en tableros privados. Los usuarios solo verán el título de la página cuando autoricen su cuenta de Confluence, luego de lo cual podrán expandir y editar el documento de Confluence (según los permisos de nivel de acceso proporcionados).
:::

![Connect_Confluence.png](../../../../../../docs/integrations-apps/atlassian/images/21019693898258_Connect%20Confluence.png)*Conectar la página de Confluence en Miro*

Una vez que Confluence esté autorizado, los usuarios que acceden al tablero podrán ver el título del documento, el ícono del proveedor y la fuente del enlace. Los usuarios también podrán expandir el enlace inteligente de Miro al modo de pantalla completa.

:::tip
Los títulos de enlace inteligente de Miro se extraen de la URL. Si editas el título del documento de Confluence, deberás volver a pegar el enlace para ver el título actualizado en tu enlace inteligente de Miro.
:::

![Connected_Confluence_card.png](../../../../../../docs/integrations-apps/atlassian/images/21019704985746_Connected%20Confluence%20card.png)*Una página de Confluence conectada como enlace inteligente de Miro*

Cuando los usuarios hagan clic en el ícono de expandir, se les pedirá que autoricen su propia cuenta de Confluence antes de que puedan ver y editar el documento dentro de Miro.

![Expanded_Confluence_card.png](https://help.miro.com/hc/article_attachments/21019705042578)*El documento de Confluence expandido*

## Insertar tableros de Miro en documentos de Confluence

Puedes insertar tableros de Miro en documentos de Confluence con el Complemento de Miro para Confluence o directamente a través de Atlassian Smart Links. Puedes hacerlo con Confluence Cloud, Server o DC.

### Paso 1: Configura el Complemento de Miro

Primero, instala la [aplicación de Miro para Confluence](https://marketplace.atlassian.com/apps/1217530/miro-for-confluence?tab=reviews&hosting=cloud) desde Atlassian Marketplace.

**Cómo instalar la aplicación de Miro para Confluence**

> **Quién puede hacerlo**: admin de Confluence

1. Inicia sesión en tu instancia de Confluence como admin
2. Haz clic en el menú desplegable de administrador y elige **Complementos (Aplicaciones)**
3. Selecciona **Buscar nuevas aplicaciones** o **Buscar nuevos complementos**
4. Busca **Miro para Confluence**
5. Haz clic en **Obtener aplicación**

![Miro_for_Confluence.png](https://help.miro.com/hc/article_attachments/21019705044882)*La aplicación de Miro para Confluence*

Verás el siguiente mensaje cuando la aplicación se haya instalado correctamente:

![success_message.jpg](https://help.miro.com/hc/article_attachments/22249929764882)
*La aplicación se instaló correctamente*

### Paso 2: inserta un tablero en la página de Confluence

Hay tres maneras de insertar un tablero de Miro en una página de Confluence:

1. Escribir **/miro** directamente en el documento de Confluence.
   ![Typing_miro_on_the_doc.png](https://help.miro.com/hc/article_attachments/22249929770514)
   *Escribir /miro en la página de Confluence para insertar un tablero*
2. Buscando Miro desde la barra de herramientas de la aplicación. Desde el documento de Confluence, haz clic en **Insertar** y selecciona **Miro** de la lista de aplicaciones.
   ![Miro_plugin.jpg](https://help.miro.com/hc/article_attachments/22249903480210)
   *Seleccionando Miro de la lista de aplicaciones para insertar un tablero*
3. Pegando un enlace de Miro directamente en Confluence con Atlassian Smart Links.

### Paso 3: selecciona un tablero del selector de tableros

El selector de tableros se abrirá. Selecciona el tablero que deseas insertar desde el menú desplegable o busca un tablero. Los usuarios solo verán los tableros disponibles en Miro y solo podrán insertar tableros si tienen acceso de editor a esos tableros.

![Board_picker.png](https://help.miro.com/hc/article_attachments/21019705050258)*Elegir un tablero para insertar desde el selector de tableros*

Selecciona la **vista inicial** para el tablero insertado.

![Set-the-starting-view-for-your-embed.png](../../../../../../docs/integrations-apps/atlassian/images/21019693917842_Set-the-starting-view-for-your-embed.png)*Configurando la vista inicial para el tablero de Miro insertado*

Elige el nivel de acceso para **Todos los visitantes** de la página de Confluence.

- **Pueden ver:** Permite que cualquier visitante de la página de Confluence pueda ver el tablero.
- **Requiere acceso:** Limita la visualización a quienes tienen acceso al tablero en Miro.

![Access-level-for-embed.png](../../../../../../docs/integrations-apps/atlassian/images/21019693915666_Access-level-for-embed.png)*Configurando el nivel de acceso al tablero de Miro en la página de Confluence*

### Paso 4: Insertar el tablero

Una vez que hagas clic en **Insertar tablero**, el tablero de Miro se insertará en la página de Confluence como iFrame. Los usuarios pueden ver y navegar por el tablero.

:::note
Para los usuarios del plan Enterprise, los niveles de acceso seguirán la configuración de acceso de toda la organización, y por lo tanto, algunos permisos pueden estar restringidos. Aprende más sobre [la gestión de tableros insertados para el plan Enterprise](https://help.miro.com/hc/articles/4405088016274).
:::

![Miro-board-embedded-in-confluence.png](../../../../../../docs/integrations-apps/atlassian/images/21019705017874_Miro-board-embedded-in-confluence.png)*Tablero de Miro insertado en una página de Confluence*

Para abrir el tablero directamente en Miro, haz clic en el logo de Miro.

![Open-embedded-board-in-miro.png](../../../../../../docs/integrations-apps/atlassian/images/21019693937554_Open-embedded-board-in-miro.png)
*La opción para abrir el tablero en Miro*

#### **Experiencia del usuario en Confluence Cloud vs. Confluence Server**

El menú de tamaño de la ventana para los tableros insertados es diferente en Confluence Cloud y Confluence Server.

En Confluence Cloud, verás el siguiente menú de tamaño de ventana con la opción **Usar ancho completo**:

![Go-full-width-Miro-board-confluence.png](../../../../../../docs/integrations-apps/atlassian/images/21019693943826_Go-full-width-Miro-board-confluence.png)
*Menú de tamaño de ventana en el navegador de Confluence*

En Confluence Server, verás un menú con la opción para seleccionar un tamaño de ventana pequeño, mediano o grande (**S/M/L**):

![Miro_in_Confluence_Server.jpg](../../../../../../docs/integrations-apps/atlassian/images/21019705005330_832eb85b-5925-4545-8cea-321d3b55d7ed.png)*Menú de tamaño de la ventana en la aplicación de Confluence*

## Insertar tableros de Miro a través de Atlassian Smart Links

También puedes insertar tableros de Miro en Confluence utilizando la función de Atlassian Smart Links. La función te permite insertar automáticamente un tablero sin necesidad de instalar una aplicación.

Ve a una página de Confluence y simplemente pega un enlace de tablero, o escribe **/link** para insertar. Si usas la función por primera vez, se te pedirá que conectes un equipo de Miro. Haz clic en **Connect to preview**, autoriza en Miro y elige un equipo desde el cual insertarás tus tableros.

:::note
Solo los usuarios que tengan acceso al tablero insertado en Miro podrán trabajar con la vista previa del tablero insertado después de conectar sus cuentas de Atlassian y Miro. Si quieres que la vista previa del tablero esté disponible para todos los usuarios de Confluence, puedes usar la aplicación de Miro.
:::

![install_Atllassian_links.jpg](https://help.miro.com/hc/article_attachments/22249903483666)
*Elegir un equipo desde el cual insertar los tableros*

Cuando pegas el enlace de un tablero de Miro en una página de Confluence, este se convierte en un widget de forma automática. Haz clic en el enlace para ver las opciones de visualización. Puedes elegir mostrar el tablero de Miro como un **URL**, texto **en línea**, una **tarjeta** o una**inserción**.

![Confluence_widget.png](../../../../../../docs/integrations-apps/atlassian/images/21019704980370_Confluence%20widget.png)*Widget del tablero de Miro en Confluence*

Si eliges mostrar el tablero como elemento insertado, puedes cambiar el tamaño del elemento arrastrando sus lados.

![changing_embed_size.gif](https://help.miro.com/hc/article_attachments/22249903488402)
*Cambiar el tamaño del elemento insertado de Miro en Confluence*

:::warning
Si las cookies de terceros están bloqueadas en tu navegador, puede haber problemas inesperados cuando se muestran los tableros insertados.
:::

## Deshabilitar la aplicación de Miro para Confluence

Para deshabilitar la aplicación, ve a **Atlassian Marketplace** > **Manage apps** > **Miro for Confluence Cloud** > **Uninstall.**

*![Uninstall_Confluence_plugin.jpg](https://help.miro.com/hc/article_attachments/22249903494034)*
*La aplicación de Miro para Confluence en la lista de las aplicaciones de Atlassian instaladas*

## Migración y su impacto en los tableros de Confluence

Ya sea que estés migrando de una instancia local a una en la nube, o de nube a nube, el plugin de Miro no requiere pasos de migración dedicados. Confluence muestra los tableros de Miro a través de iFrames, que son inserciones basadas en URL, lo que significa que Confluence solo almacena el enlace del tablero, mientras que el tablero permanece en Miro.
