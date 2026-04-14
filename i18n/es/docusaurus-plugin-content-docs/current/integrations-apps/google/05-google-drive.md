---
title: Google Drive
article_id: 360017731253
translation_id: 360017731253
locale: es
sidebar_position: 6
created_at: '2019-02-11T10:14:01Z'
updated_at: '2025-01-13T14:51:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

**Google Drive** te permite almacenar archivos en línea de forma segura, acceder a ellos desde cualquier lugar y colaborar con otras personas. Con la integración de Google Drive, te facilitamos centrarte en tus tareas y rastrear tus documentos directamente en el tablero.

Google_Drive_on_the_Upload_menu.jpg

> Configurada **por:** cada usuario por separado (los admins pueden restringir la instalación de la app a usuarios que no sean admins)
> **Disponible en:** versión para navegador, [app de escritorio](../../getting-started/apps-for-devices/05-desktop-app.md) (funcionalidad completa y edición de archivos); [app para tableta](../../getting-started/apps-for-devices/11-tablet-app.md), [app móvil](../../getting-started/apps-for-devices/08-mobile-app.md) (funcionalidad limitada, no se admite la edición).

### Cómo habilitar Google Drive

Para empezar a agregar archivos de Google Drive, deberás instalar el plugin y conectar tu Google Drive a Miro.

Instalar la aplicación de [marketplace de Miro](https://miro.com/marketplace/google-drive/?backUrl=%2Fmarketplace%2F). Tras hacer clic en **Obtener app**, se te sugerirá que elijas un equipo para el que instalar el plugin.![install_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016134562450_install%20Google%20Drive.jpg)*Elegir un equipo al instalar el complemento de Google Drive*

También puedes instalar el plugin desde un tablero. En la barra de creación, selecciona **Herramientas, Medios e integraciones****(+**). Se abre un panel. En la pestaña **Herramientas**, busca Google Drive. Selecciona **Cargar** y, a continuación, selecciona **Google Drive**.

Google_Drive_on_the_toolbar.jpg

Luego, conecta Google Drive a Miro. Hay 2 formas sencillas.

1.  Desde la configuración de tu perfil. En la barra de tableros, selecciona el icono de la hamburguesa. Se abre la barra lateral. Selecciona tu avatar y, a continuación, selecciona **Configuración**. La configuración de tu perfil se abre en una nueva ventana. Selecciona la pestaña **Integraciones** . Para **Google Drive**, selecciona **Conectar**.

![conectar_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016121228306_connect%20Google%20Drive.jpg)*Google Drive en la página de integraciones*

2. 2. Conecta tu perfil de Miro a **Google Drive** desde el tablero al hacer clic en Google Drive en el menú **Upload (Cargar)** en la barra de herramientas:

![Google_Drive_en_el_menú_de_carga.jpg](../../../../../../docs/integrations-apps/google/images/21016121222546_Google%20Drive%20on%20the%20Upload%20menu.jpg)*El icono de Google Drive en la barra de herramientas*

Confirma la autorización para la cuenta de Google necesaria y **permite** que la aplicación acceda a tus archivos:

permissions.jpg
Permisos de Google Drive

Ten en cuenta que estos son los permisos estándar para Google Drive.

- **Consulta y descarga todos tus archivos de Google Drive** para un seleccionador de archivos de Google Drive en un tablero. Permite importar documentos de Google Drive a Miro

-- **Ver, editar, crear y eliminar solo los archivos de Google Drive específicos que usas con esta aplicació**n para tener la capacidad de guardar un tablero de Miro en Google Drive.

La aplicación de Google Drive solo administra los archivos que creamos en el Drive (enlaces a tableros, etc.).  Miro no tiene la oportunidad de administrar ningún contenido en tu Google Drive. Para implementar la integración, usamos la **API v3 de Google Drive**. En esta API, los alcances se agrupan de tal manera que no se puede solicitar permisos de acceso de escritura por separado de los permisos de acceso al disco completo. Si quisieras echar un vistazo, consulta los permisos en el artículo de Google, [Alcances para las API de Google](https://developers.google.com/identity/protocols/googlescopes).

Si necesitas cambiar la cuenta de Google conectada a Miro, ve a **Ajustes de perfil** > **Integraciones**, haz clic en **Cerrar sesión** junto a **Google Drive** y conecta otra cuenta

![Google_Drive_logout_en_configuracion.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*Conexión a Google Drive en la configuración del perfil*

### Cómo añadir archivos de Google Drive y unidades compartidas

> **Disponible en:** versión de navegador, [aplicación de escritorio](../../getting-started/apps-for-devices/05-desktop-app.md), [aplicación para tabletas](../../getting-started/apps-for-devices/11-tablet-app.md), [aplicación móvil](../../getting-started/apps-for-devices/08-mobile-app.md) (funcionalidad limitada)

:::warning
Cualquier persona con acceso a un tablero de Miro puede extraer sus documentos importados, incluso si está restringida por Google. Para proteger tus archivos, es importante que evites compartir el tablero con personas que no deben tener acceso a los documentos.
:::

Para añadir un archivo de Google Drive:

1. Pega la URL del documento en el tablero (ten en cuenta que pegar una URL en una [forma](../../using-miro/essential-tools/11-shapes.md) o en una [nota adhesiva](../../using-miro/essential-tools/14-sticky-notes.md) no insertará tu documento en el tablero, pero añadirá el enlace como texto simple). Cuando copias un enlace a una hoja concreta desde las hojas de cálculo de Google y lo pegas en el tablero de Miro, la hoja de cálculo pegada seguirá empezando desde la primera página en Miro.

   o/span>
2. Haz clic en el botón **Cargar** en la barra de herramientas (que se muestra en la captura de pantalla anterior) y elige **Google Drive**. Luego, verás el menú del seleccionador. Selecciona todos los documentos que te gustaría añadir y haz clic en **Seleccionar**. También puedes usar la barra de búsqueda para encontrar documentos en tu Google Drive.

> Para añadir un documento de Google Drive en un tablero en la [aplicación móvi](../../getting-started/apps-for-devices/08-mobile-app.md)l, pega la URL del documento mediante el menú Cargar.

![seleccionar_un_archivo_en_Google_Drive.gif](../../../../../../docs/integrations-apps/google/images/21016121231122_select%20a%20file%20in%20Google%20Drive.gif)*Seleccionar un documento en Google Drive*

Añade documentos de **unidades compartidas**: cambia a la pestaña y elige archivos.

![team_drive.jpg](../../../../../../docs/integrations-apps/google/images/21016134572434_team%20drive.jpg)*Team Drive en el selector de Google Drive*

### Cómo editar documentos de Google

> **Disponible en:** versión de navegador, [aplicación de escritorio](../../getting-started/apps-for-devices/05-desktop-app.md)

Puedes insertar documentos, hojas de cálculo y diapositivas de Google en el tablero, moverlos y cambiar el tamaño, y también deslizar las páginas de los documentos.

Haz clic en el documento y verás un menú contextual con las opciones para cambiar páginas, **fijar** una página, **extraer páginas**, **editar** contenido, **volver a cargar**, **actualizar** o ir a la **fuente**.

Para comenzar a editar el documento, haz clic en el ícono de la pluma en el menú contextual o haz doble clic en el documento. El documento se abre en una ventana emergente y puedes editarlo como si estuviera en tu Google Drive. Haz clic en **Cerrar** o en el área gris para terminar de editar. Todos los cambios se guardan automáticamente y están visibles en el tablero y en los documentos de Google.

![google_drive_editar_docs.gif](../../../../../../docs/integrations-apps/google/images/21016121248274_google_drive_edit_docs.gif)*Editar un Documento de Google insertado*

Si prefieres también puedes hacer clic en el botón **fuente** y el documento se abrirá para editar en la siguiente pestaña.

Si hiciste cualquier edición directamente desde tu Google Drive (especialmente, cuando trabajabas sin conexión), actualiza lo insertado en el tablero usando el botón **Actualizar** en el menú contextual. Los archivos de Google Drive insertados no se actualizan automáticamente en los tableros de Miro (a menos que el archivo se edite desde Miro).

![botón_actualizar.jpg](../../../../../../docs/integrations-apps/google/images/21016121232274_update%20button.jpg)*Botón de actualización*

### Cómo administrar los derechos de acceso

Ten en cuenta que los derechos de acceso en Google Drive y Miro se establecen *por separado*. Significa que para permitir que alguien edite un documento de Google en el tablero, debes compartir el documento con él en Google Drive con los derechos *del editor* y también [invitarlo como *editor* al tablero](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

Si permites que alguien edite el documento en Google, pero lo invitas al tablero solo con [los derechos de visualización o comentarios](../../using-miro/sharing-boards/01-board-access-rights.md), no podrá activar el modo de edición del documento. Y viceversa, si invitas a una persona al tablero como editor, pero no compartes el documento con ellos en Google Drive, Google no les permitirá editarlo.

Asegúrate de que tú y los miembros de tu equipo reciban el nivel de acceso necesario para tener una colaboración exitosa.

### Cómo guardar un tablero en Google Drive

> **Configurado por:** propietarios del tablero

En la barra de tableros, selecciona los tres puntos verticales. Se abre el menú **principal**. Selecciona **Tablero** > **Exportar** > **Guardar en Google Drive**.

En Google Drive, ahora puedes hacer clic en el tablero guardado y se abrirá en una pestaña del navegador separada.  Si eliminas el tablero de Google Drive, seguirá estando disponible en Miro. Sin embargo, si eliminas el tablero en Miro, ya no podrás acceder a él desde Google Drive./span>

:::warning
Si no eres el propietario del tablero, recibirás el mensaje de error como se muestra a continuación.
:::

![Google_Drive_error.jpg](../../../../../../docs/integrations-apps/google/images/21016121236882_Google%20Drive%20error.jpg)*Mensaje de error de derechos de almacenamiento insuficientes*

### Cómo desinstalar el plugin

Para desinstalar el plugin para un equipo, encuéntralo en la sección **Aplicaciones e integraciones** de los ajustes del equipo y haz clic en **Desinstalar para el equipo**.

![desinstalar_app_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016134575122_uninstall%20Google%20Drive%20app.jpg)*Desinstalar Google Drive para un equipo*

Para desconectar Miro de Google Drive, abre la página **Integrations** (Integraciones) en Profile settings (Ajustes de perfil) y haz clic en**Log out** (Cerrar sesión) cerca del icono de Google Drive.

![Google_Drive_logout_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*Desconectar Google Drive de Miro*

### Características no disponibles para los archivos integrados de Google Drive

**General**

- Página de inicio de Google Drive
- Cómo mover archivos entre carpetas
- Cómo compartir
- Búsqueda de ayuda

**Presentaciones de Google**

- Modo de presentación

### Posibles dificultades y cómo resolverlas

**Error de carga**

Si recibes el mensaje de error **Lo sentimos, parece que no tienes derechos para cargar este archivo o el archivo se eliminó.** Consulta el derecho de acceso e intenta nuevamente cuando intentes cargar un archivo de Google Drive a un tablero de Miro, pídele a tu administrador de Google que permita que los usuarios accedan a Google Drive con la API del SDK de Drive:

1. Inicia sesión en la [consola de administración de Google.](https://admin.google.com/)
2. Haz clic en **Inicio > Aplicaciones > Espacio de trabajo de Google**. Asegúrate de que el Drive y los documentos estén **ACTIVADOS para todos.**
3. Haz clic en **Drive y Docs > Features and Applications (Características y aplicaciones**). En la sección delSDK de Drive, asegúrate de **permitir que los usuarios accedan a Google Drive cuando el API del SDK de Drive** esté **ACTIVADO**.

no_se_pudo_subir.png
Mensaje de advertencia de que no se pudo subir

**Problema de autorización**

Si no puedes conectar tu Google Drive a Miro, asegúrate de conceder acceso a Miro para **Ver y descargar todos tus archivos de Google Drive** y **Ver, editar, crear y eliminar solo los archivos específicos de Google Drive que usas con esta aplicación** cuando conectes tu Google Drive. Para esto, ve a Miro Profile settings (Ajustes de perfil de Miro) > Integrations (Integraciones), elimina la conexión con Google Drive y vuelve a configurarla.

Permisos.png
Acceso de Miro a la cuenta de Google Drive

### Preguntas frecuentes

1. *¿Puedo abrir un archivo insertado en Google Drive?*
   - Sí, selecciona el documento y haz clic en el botón **Fuente** del menú contextual.
2. *¿Puedo pegar el contenido del tablero de Miro en un archivo de Google Drive?*
   - Puedes [copiar el contenido del tablero como texto o como imagen](../../using-miro/working-on-the-board/09-copy-as-text-or-as-an-image.md) y pegarlo en un archivo de Google Drive.
