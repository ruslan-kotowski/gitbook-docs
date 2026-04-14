---
title: "Aplicaci\xF3n de escritorio"
article_id: 360017572854
translation_id: 360017572854
locale: es
sidebar_position: 5
created_at: '2019-02-11T10:15:04Z'
updated_at: '2025-11-25T16:00:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
---

Abre la aplicación de Miro de escritorio en segundos desde tu pantalla de inicio y trabaja en tableros sin distracciones. La app admite todas las funciones básicas de la versión de navegador.

:::tip
Descarga la app de Miro desde [nuestro sitio web](https://miro.com/apps/).
:::

## Descargar la app de escritorio de Miro

### Windows

- Windows 64-bit - [descargar la aplicación](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.exe)

:::note
Windows 32-bit está obsoleto y ya no está disponible.
:::

### macOS

- Macs con chips de Apple silicon - [descargar la aplicación](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro.dmg)
- Macs con chips Intel - [descargar la aplicación](https://desktop.miro.com/platforms/darwin/Install-Miro.dmg)

Para averiguar qué tipo de procesador tienes, sigue estos pasos:

1. Haz clic en el ícono de Apple en la esquina superior izquierda de tu Mac.
2. Esto hará aparecer un menú desplegable. Haz clic en la opción **Acerca de esta Mac**.

La ventana te mostrará la información que necesitas, incluyendo el tipo de procesador (Intel o Apple silicon).

## Implementa Miro en múltiples dispositivos

Miro ofrece varias versiones de instalador que los administradores de TI pueden utilizar para implementar Miro en usuarios a través de miles de máquinas. Hay dos formas básicas de hacerlo: instalar por usuario o por máquina. Dentro de cada una de ellas, hay versiones con y sin actualizaciones automáticas. La versión con actualizaciones automáticas permite que tus usuarios reciban la versión actualizada de la app tan pronto se publique. La versión sin actualizaciones automáticas te da más control sobre la versión de Miro que utilizan tus empleados.

### Para Windows

#### Como implementar Miro en Archivos de programa

Miro también puede instalarse en el directorio Archivos de programa, para que esté disponible para todos los usuarios de un dispositivo, manteniendo sus perfiles separados. Una única instalación en una máquina representa una menor huella de disco duro a escala, al tiempo que Miro sigue estando disponible para todos los usuarios de esa máquina. Si optas por la versión con actualizaciones automáticas, ten en cuenta que se necesitan permisos administrativos para instalar una actualización.

- Windows MSI de 64 bits con actualizaciones automáticas - [descargar la aplicación](https://desktop.miro.com/platforms/win-nsis/Miro-setup.msi)
- Windows MSI de 64 bits sin actualizaciones automáticas - [descargar la aplicación](https://desktop.miro.com/platforms/win-nsis/Miro-no-updates.msi)

#### Cómo implementar Miro para un usuario concreto

Miro ofrece varias versiones de instalador que los administradores de TI pueden utilizar para implementar Miro para un solo usuario. Esta versión puede actualizarse sin permisos administrativos y solo se instala para el usuario o usuarios concretos elegidos.

- Windows MSI 64 bit con actualizaciones automáticas - [descargar la aplicación](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.msi)
- Windows MSI 64 bit sin actualizaciones automáticas - [descargar la aplicación](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-no-updates.msi)

### Para MacOS

- Mac con Apple silicon sin actualizaciones automáticas - [descargar la app](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro-no-updates.dmg)
- Mac con Intel sin actualizaciones automáticas - [descargar la app](https://desktop.miro.com/platforms/darwin/Install-Miro-no-updates.dmg)

## Requisitos de sistema de la aplicación

### Para Windows

|  |  |  |
| --- | --- | --- |
|  | **Mínimo** | **Recomendado** |
| **CPU** | 3 GHz (2 núcleos/4 hilos) | 2,8 GHz (4 núcleos/8 hilos) |
| **RAM** | 8 GB | 16 GB (DDR4) |
| **SO** | Windows 10 o superior para la app de Microsoft Store + Microsoft .NET Framework 4.5 (Por favor, nota que la versión ARM de Windows no es compatible) | SO más reciente |
| **Red** | 8 Mb/s o más rápido | 32 Mb/s |

### Para macOS

|  |  |  |
| --- | --- | --- |
|  | **Mínimo** | **Recomendado** |
| **CPU** | Intel de 64 bits o Apple M1 |  |
| **Sistema operativo** | MacOS 12 (Monterey) o superior | Último sistema operativo |
| **Red** | 8 Mb/s o más rápido | 32 Mb/s |

Ten en cuenta que la aplicación tendrá varias instancias en funcionamiento en tu dispositivo:

- Proceso principal
- Proceso de ventana (renderizador de UI)
- Aceleración de hardware
- Gestión de accidentes
- + 1 proceso por cada pestaña abierta (porque cada pestaña tiene una WebView)

Por ejemplo, si tienes tres pestañas abiertas durante tu trabajo, verás siete instancias de Miro.exe. Más información sobre esta arquitectura se puede encontrar [aquí](https://www.electronjs.org/docs/glossary#process) y [aquí](https://www.chromium.org/developers/design-documents/multi-process-architecture).

## Atajos específicos de la aplicación

La aplicación de escritorio tiene atajos adicionales [aquí](../../using-miro/working-on-the-board/06-shortcuts-and-hotkeys.md):

- **Ctrl + R** *(para Windows)* / **Cmd + R** *(para Mac)* para recargar la pestaña
- **Ctrl + W** *(para Windows)* / **Cmd +W** *(para Mac)* para cerrar la pestaña
- **Ctrl + Q** *(para Windows)* / **Cmd + Q** *(para Mac)* para salir de la app
- **Ctrl + Shift + L** *(para Windows)* / **Cmd + Shift + L** *(para Mac)* para copiar el enlace del tablero
- **Ctrl + ~** *(para Windows)* / **Cmd + ~** *(para Mac)* para hacer zoom

## Acciones de la aplicación

La siguiente tabla muestra qué acciones disponibles en la aplicación de escritorio de Miro pueden tener una experiencia diferente en comparación al navegador:

| Acción | **Apps de Win y Mac desde** [**Miro Apps**](https://miro.com/apps/) |
| --- | --- |
| Guardar como imagen (bajo, medio, alto) | ✔ |
| Guardar como imagen (vector) | ✔ |
| Guardar como PDF (bajo) | ✔ |
| Guardar como PDF (vector) | ✔ |
| Exportar a una hoja de cálculo (CSV) | ✔ |
| Videochat | ✔ |
| Pegar desde una hoja de cálculo | ✔ |
| Plugin para Confluence | ✔ |

### Acciones no disponibles

Las siguientes acciones no están disponibles en la aplicación de escritorio de Miro:

- Los visitantes no pueden iniciar sesión.

  > ✏️ Solo los usuarios registrados de Miro pueden iniciar sesión en la aplicación de escritorio.
- Sin opción para copiar/pegar desde Sketch
- Para algunas versiones de Jira Server, no es posible editar las tarjetas de Jira por razones de seguridad.

## Verificación ortográfica

Si quieres desactivar la funcionalidad de verificación ortográfica automática en la aplicación de escritorio, sigue estos pasos:

- Presiona **Alt** (*solo para Windows*)
- Haz clic en **Vista** en la barra de navegación principal en la parte superior
- Desmarca el botón **Mostrar corrector ortográfico**

Ten en cuenta que la opción para deshabilitar la verificación ortográfica no está disponible en la aplicación descargada de Microsoft Store.

## Posibles dificultades y cómo resolverlas

### Cómo restablecer los datos de la aplicación

En varios casos en los que surge un problema (especialmente si tienes dificultades con el procedimiento de inicio de sesión), puede resultar de ayuda **restablecer los datos de la aplicación**, despejando la memoria de la aplicación.

:::tip
Si el problema persiste después de restablecer los datos, también puedes eliminar la aplicación y volver a instalarla [descargando la última versión](https://miro.com/apps/).
:::

#### Para Windows

Presiona **Alt > Help** y elige restablecer los datos de la aplicación como se muestra en la captura de pantalla a continuación:

![reset app data on Windows.png](../../../../../../docs/getting-started/apps-for-devices/images/21016134171922_reset%20app%20data%20on%20Windows.png)
*Restablecer los datos de la app en la app de escritorio para Windows*

Si no puedes encontrar el menú, probablemente estés usando la aplicación descargada desde MS Store. En este caso, para restablecer los datos de la aplicación, abre **Configuración** de Windows > **Aplicaciones** > **Aplicaciones y características** > busca **Miro** en la lista > **Opciones avanzadas** > **Restablecer**.

Si esto no ayuda de inmediato, procede a eliminar todos los archivos de la aplicación de **C:\Users\username\AppData\Roaming\RealtimeBoard** y **C:\Users\username\AppData\Local\Programs\RealtimeBoard**

> **✏️** Si la carpeta **Appdata** está oculta, ve [aquí](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) cómo puedes revelarla.

#### Para macOS

Haz clic en Miro en el menú superior y elige **Restablecer los datos de la aplicación** como se muestra en la captura de pantalla a continuación:

![reset app data on Mac.png](../../../../../../docs/getting-started/apps-for-devices/images/21016120799378_reset%20app%20data%20on%20Mac.png)
*Restablecer los datos de la aplicación en Mac*

Después de eso, intenta iniciar sesión nuevamente en la aplicación y verificar si el problema se resolvió.

Si restablecer la aplicación no ayuda de inmediato, abre una ventana del buscador > presiona **Command + Shift + G** > pega **~/Library/Application Support/RealtimeBoard**y elimina todos los archivos de la aplicación.

Si usas MDM para Mac

Si enfrentas una incidencia cuando la aplicación no puede cargarse y está atascada en un bucle, asegúrate de que tu configuración permite que nuestro actualizador automático se ejecute. `https://github.com/Squirrel/Squirrel.Mac` debe tener permisos para:

- leer, escribir y ejecutar en el directorio "Application".
- leer y escribir en "~/Application Support/Caches/" para trabajar con el directorio "com.electron.realtimeboard.ShipIt" y también opera con el directorio temporal "private/var/folders".

Si algo sale mal durante el proceso de actualización, Squirrel crea "ShipIt_stderr.log" en "~/Application Support/Caches/com.electron.realtimeboard.ShipIt". Se puede encontrar más información sobre el problema allí.
Ten en cuenta que Skype y Slack usan un proceso de actualización similar, por lo que si ya has configurado MDM para ellos, puedes aplicar los mismos ajustes para la aplicación de escritorio de Miro.

## Preguntas frecuentes

1. *¿Dónde puedo descargar la aplicación de escritorio?*
   - Descárgala desde [nuestro sitio web](https://miro.com/apps/).
2. *¿Cómo puedo eliminar la ventana emergente para abrir la aplicación de escritorio cuando inicio Miro en un navegador?*
   - Prueba siguiendo los pasos de [este artículo](../../using-miro/troubleshooting-technical-questions/technical-guidelines/04-how-to-disable-miro-desktop-app-pop-up-in-your-browser.md).
3. *¿Tienes una versión de la aplicación de escritorio para Linux?*
   - No, por el momento, no tenemos esa versión.
4. *¿Cómo puedo copiar un enlace de un tablero abierto en la aplicación de escritorio?*
   - Puedes abrir el menú de **Compartir** del tablero y copiar el enlace desde allí. Otra manera es hacer clic en **Archivo** en la esquina superior derecha > **Copiar enlace del tablero**. También puedes usar el atajo **Ctrl + Shift + L** *(para Windows) /* **Cmd + Shift + L** *(para Mac).*
5. *Si presiono **Alt** mientras estoy en mi aplicación de escritorio de Windows, el menú no aparece. ¿Cómo puedo solucionarlo?*
   - Ten en cuenta que el menú no es compatible con la app descargada de Microsoft Store. Puedes restablecer los datos de la app a través de la configuración de Windows (**Sistema > Aplicaciones > Buscar Miro > Opciones avanzadas > Restablecer**) o [instalar la versión original de la aplicación](https://miro.com/apps/).
6. *Si elimino la aplicación de escritorio, ¿mis tableros se eliminarán?*
   - No, tu contenido está vinculado a tu perfil de Miro. Puedes acceder a él en un navegador, [aplicación para tabletas](11-tablet-app.md), [aplicación móvil](08-mobile-app.md) también.
