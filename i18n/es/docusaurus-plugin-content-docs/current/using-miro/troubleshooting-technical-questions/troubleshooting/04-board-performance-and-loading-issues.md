---
title: Problemas de rendimiento y carga del tablero
article_id: 360013588560
translation_id: 360013588560
locale: es
sidebar_position: 4
created_at: '2020-05-06T08:17:24Z'
updated_at: '2025-04-01T16:57:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Explora consejos para mejorar el rendimiento de los tableros durante las sesiones colaborativas y en tableros grandes y para solucionar problemas como el rendimiento y la navegación lentos, el congelamiento de los tableros y las cargas interminables.

## Cómo mejorar el rendimiento del tablero

El rendimiento del tablero puede ser más lento durante **las sesiones colaborativas** con un gran número de usuarios, así como en **los tableros grandes** que tienen mucho contenido.

Consejos para las sesiones colaborativas Consejos para tableros grandes

El número creciente de usuarios de un tablero y su intensiva actividad pueden afectar el rendimiento de los tableros.  Los usuarios con dispositivos más antiguos y menos potentes tienen un mayor riesgo de sufrir retrasos en el rendimiento.

**Si estás participando de una sesión colaborativa, asegúrate de hacer lo siguiente:**

- cierra o minimiza todas las pestañas y ventanas redundantes, si trabajas en un navegador de escritorio [navegador](../technical-guidelines/02-supported-browsers-browser-restrictions.md)
- ocultar los cursores de los colaboradores y cerrar todas las barras laterales
- tratar de no seleccionar y cambiar múltiples objetos del tablero al mismo tiempo;
- Minimizar la navegación en el tablero.
- Si accedes a Miro desde una laptop, asegúrate de estar en el modo de alto rendimiento en lugar de en el modo de ahorro de energía.

**Si estás planificando una sesión colaborativa en Miro, esto es lo que debes hacer:**

- Invita a los usuarios que no necesitan acceso de edición como visualizadores.  Aprende cómo configurar [los derechos de acceso al tablero](../../sharing-boards/01-board-access-rights.md)/span>
- Asegúrate de mantener el contenido del tablero ordenado: para saber cómo lograrlo, consulta nuestros **Consejos para tableros grandes**, en la segunda pestaña de arriba.

La cantidad máxima de objetos que puedes agregar en un tablero es 100 000.  Sin embargo, el rendimiento puede verse afectado a partir de los 1000 objetos. Para tener una mejor experiencia, recomendamos mantener el número de objetos en cada tablero por debajo de los 5000. /span>
Para encontrar la cantidad de objetos en el tablero:

- Selecciona todos los objetos del tablero (ctrl-A en Windows, cmd-A en Mac o crea un cuadro de selección alrededor de todos los objetos).
- El menú contextual aparecerá donde verás la cantidad total de objetos
- Haz clic **en Filtrar** para ver la cantidad de objetos por tipo

![número-de-objetos.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/25736281544466_number-of-objects.gif)
*Medir el número de objetos de un tablero*

Junto con el número de objetos, los objetos más pesados o complejos (especialmente los archivos y documentos cargados) también pueden ralentizar tu tablero.

Para acelerar un tablero grande, manténlo en orden:

- Elimina el contenido innecesario, especialmente los archivos y documentos grandes cargados (por ejemplo, PDF de vectores con muchos detalles o imágenes de alta resolución)
- Convierte los PDF y las imágenes pesadas en alta resolución a archivos PNG/JPG y vuelve a subirlos al tablero
- Reduce la escala del contenido del tablero si se ve demasiado grande con un zoom del 100%:
  - Ve al mapa en la esquina inferior derecha y establece el zoom al 100%
  - Si con este nivel de zoom tu contenido se ve demasiado grande, selecciónalo usando **Ctrl + A** (en Windows) o **Cmd + A** (en Mac) y reduce la escala
  - considera también la posibilidad de reducir la escala de las imágenes grandes
    **![redimensionar-objetos-tablero.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/25736308553874_resize-board-objects.gif)**
    *Reducción del contenido*
- [resolver comentarios](../../facilitation-tools/asynchronous-tools/01-comments.md)
- Convertir [la](../../essential-tools/10-pen.md) escritura a mano en imágenes:
  - Haz una captura de pantalla de un dibujo.
  - Súbelo al tablero.
  - Elimina el dibujo.
- Si es posible, divide el tablero en un par de tableros:
  - Copia una parte del contenido del tablero seleccionándolo y presionando **Ctrl + C** (para Windows) o **Cmd + C** (para Mac)
  - [Crea un nuevo tablero](../../../getting-started/start-here/your-first-board/01-create-a-miro-board.md) y pega el contenido en el tablero.
  - Elimina el contenido que copiaste del tablero original.

## Cómo resolver problemas de bajo rendimiento o cargas interminables

Tu dispositivo, conexión a internet, navegador y otros factores pueden influir en el rendimiento y la velocidad de carga del tablero.  Si experimentas un rendimiento deficiente en el tablero o tu panel no carga en un navegador, aplicación de escritorio, en una tableta o dispositivo móvil, intenta resolver el problema dando los siguientes pasos.

:::warning
Antes de explorar las soluciones a continuación, consulta la [página de estado de Miro](https://status.miro.com/) para obtener los informes de degradación del rendimiento.
:::

Navegador Aplicación de escritorio Tableta, móvil

1. 1. Abre Miro en modo incógnito/span> [(privado)](https://support.google.com/chrome/answer/95464) **y en un** navegador diferenteSi Miro funciona en el modo de incógnito o en un navegador diferente, limpia el caché y las cookies de tu navegador.

**Cómo limpiar los datos del sitio web de Miro en Chrome**

1. 2. Ve a /span>`https://miro.com/` y abre las **herramientas de desarrolladores** de Chrome (**Command + Option + J** *en Mac*, **Ctrl + Mayús + J** *en Windows*)2. Elige la pestaña Application (Aplicación) > Storage (Almacenamiento). Haz clic en **Borrar datos del sitio.**​ Esto debería eliminar cualquier dato de Miro guardado en tu navegador Chrome, y podrás iniciar una nueva sesión. Ten en cuenta que se cerrará la sesión de tu perfil de Miro.![borrar_datos_del_sitio.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)*La opción de borrar los datos del sitio en Chrome*

Además, quizás debas actualizar el navegador a la última versión o deshabilitar ciertas extensiones. Consulta la lista de [navegadores compatibles](../technical-guidelines/02-supported-browsers-browser-restrictions.md).

2. Verifica tu **conexión a Internet**. Si el ancho de banda de la red no alcanza el mínimo de 8 Mb/s, cambia a otra red, preferiblemente, más rápida./span>

3. Asegúrate de que el dispositivo cumpla los [requisitos del sistema](../technical-guidelines/01-system-requirements.md)/span>:

- CPU: 3 GHz (2 núcleos/4 subprocesos)
- Memoria RAM: 8 GB

4. 4. Si accedes a Miro desde una laptop, asegúrate de estar **en el modo de alto rendimiento/span> en lugar de en el modo de ahorro de energía**.

5. 5. Si experimentas un problema con tableros específicos, intenta [duplicarlos](../../managing-boards/03-how-to-duplicate-a-board.md)/span> **y corrobora si el problema persiste en el tablero copiado.**Para los usuarios que no pueden cargar ni acceder a Miro:

6. Comprueba si tu conexión soporta **WebSockets. Obtén más información sobre WebSockets y los pasos de resolución de problemas en Cómo añadir Miro a las aplicaciones permitidas**/strong>

7. Comprueba si tu navegador soporta **WebAssembly**. Miro utiliza WebAssembly para representar el contenido del tablero. Si tu navegador, extensiones o configuración de seguridad bloquean WebAssembly, es posible que los tableros no se carguen. Para comprobar si tu navegador soporta WebAssembly, prueba a abrir [esta página de prueba](https://wasm.joway.io/). Si no es así, consulta con tu equipo informático o revisa la configuración de tu navegador para asegurarte de que WebAssembly está **permitido**.

8. Consulta con el departamento de TI si tu empresa usa firewalls/span> o un **proxy** que pueda bloquear a Miro. Sigue las directrices para colocar a Miro en la lista de permisos o proporcionar una alternativa en Cómo añadir Miro a las aplicaciones permitidas

Si el problema persiste, [comunícate con el servicio de soporte de Miro](../../tools/troubleshooting/06-contacting-miro-support.md) y envíanos [los registros de la consola del navegador](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Consulta si experimentas bajo rendimiento o cargas interminables cuando usas una [**versión web**](https://miro.com/app/dashboard/).  Si no puedes acceder a Miro desde la versión web, prueba la guía de resolución de problemas para el navegador/span>
2. Si no experimentas ningún problema en el navegador, **restablece los datos de la aplicación.**

   **Cómo restablecer los datos de la aplicación en Windows**

   Presiona Alt, haz clic en **Help** (Ayuda) en la esquina superior derecha y elige **Reset application data** (restablecer datos de la aplicación):

   reset_app_data_on_Windows.jpg
   Cómo restablecer los datos de la aplicación en la aplicación para escritorio para Windows

   Si no puedes encontrar el menú, probablemente estés usando la aplicación descargada desde MS Store. En este caso, para restablecer los datos de la aplicación, abre Windows **Configuración** > **Apps** > **Aplicaciones y funciones** > Encuentra **Miro** en la lista > **Opciones avanzadas** > **Restablecer.**

   **Cómo restablecer los datos de la aplicación para macOS**

   Cuando estés en la aplicación de Miro, haz clic en **Help** (ayuda) en el menú superior y selecciona **Reset application data** (restablecer datos de aplicación):

   restablecer_datos_aplicación_Mac.jpg
   *Restablecer los datos de la aplicación en Mac*
3. Si el problema persiste, elimina la aplicación y [**vuelve a instalarla**](https://miro.com/apps/).

Si los problemas persisten, [comunícate con el soporte de Miro](../../tools/troubleshooting/06-contacting-miro-support.md) y envía [los registros de consola de la aplicación](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Verifica tu **conexión a Internet**.  Si el ancho de banda de la red no alcanza el mínimo de 8 Mb/s, cambia a otra red, preferiblemente, más rápida.
2. Asegúrate de que el dispositivo cumpla los **requisitos técnicos**:

- Para Miro en tabletas:- RAM de 6 GB- iOS 12.0 o superior, Android 6.0 o superior, Windows 10 versión 1607 o superior- Resolución de pantalla de 768 × 1024 píxeles o superior
- Para Miro en dispositivos móviles:- OS 12.0 o superior- Android 6.0 o superior

Eliminar y **volver a instalar la aplicación** en el dispositivo

**Para usuarios de iPad:**ten en cuenta que la degradación en el rendimiento del tablero en el iPad puede estar causada por las limitaciones de la RAM del dispositivo. Intenta lo siguiente:

1. Cierra todas las aplicaciones en segundo plano que no necesites antes de usar Miro; esto debería mejorar el rendimiento.
2. Trabaja en tableros cuyo tamaño sea más pequeño; esto debería hacer que la carga de la aplicación en el sistema sea más liviana.
3. Cambia a otro dispositivo (laptop o computadora) con mejor RAM y usa la versión de navegador de Miro.

## Cómo solucionar problemas típicos

Sincronizando...  Espera unos segundos Conexión restablecida/span>

Notificación emergente **Sincronizando...** Espera unos segundos por lo general significa que se está procesando una carga pesada y que el proceso no tiene la potencia necesaria para completarse en el tiempo esperado. Así que el mensaje puede aparecer si estás trabajando en un tablero extremadamente pesado si mueves muchos objetos a granel, por ejemplo, o si hay pérdida de paquetes. Ten en cuenta que incluso si tu tablero se ve relativamente simple, para Miro los objetos pesados son las imágenes de alta resolución, los archivos PDF o los dibujos de Pen (porque son gráficos vectoriales difíciles de renderizar) o las tablas; estos pueden ocasionar una degradación en el rendimiento que dispara el mensaje.

Intenta dividir tu tablero en varios más pequeños copiando y pegando el contenido en un tablero nuevo y observa si el problema persiste.  Si eso no ayuda:

- Asegúrate de que tu dispositivo cumpla los requisitos mínimos del sistema y de que tu navegador esté actualizado a la útlima versión.
- Si tienes muchas pestañas abiertas en el navegador, intenta cerrarlas o congelarlas antes de trabajar en Miro de modo que tu navegador pueda dirigir toda su potencia de procesamiento a la aplicación de Miro sin dividirla entre otras pestañas.
- Prueba Miro en el modo de incógnito (privado) (para impedir que las extensiones del navegador interfieran) y en otro navegador. Si es necesario, cierra todas las pestañas y aplicaciones del navegador que se estén ejecutando en segundo plano.
- Elimina la caché y las cookies de tu navegador, reinicia tu navegador y actualiza la página haciendo clic en F5 (o Ctrl / Cmd + R) varias veces.
- Si experimentas problemas con tableros específicos, duplícalos y comprueba si el problema persiste en las copias. También puedes probar abriendo un tablero con menos elementos o un tablero más pequeño para ver si sigue habiendo problemas.
- Si usas VPN, comprueba si el problema persiste cuando lo desactivas.
- Intenta duplicar el tablero y comprueba si el error se reproduce en el nuevo.

Por lo general, los errores **Reconectando...**, **Conexión restablecida** pueden aparecer en los siguientes casos:

- Cuando hay problemas de conectividad de tu lado.  Asegúrate de que tu conexión de red cumpla con los requisitos mínimos. Si es posible, intenta cambiar a una red más rápida.
- Cuando estás trabajando en varios tableros pesados abiertos en el mismo navegador.  Si este es tu caso, cierra todas las pestañas y aplicaciones adicionales en ejecución en tu navegador y actualiza la página.

También vale la pena comprobar tu conexión con WebSocket (especialmente si tienes problemas con todos los tableros, incluso con los más pequeños).  Comunícate con tu departamento de TI y pídeles que habiliten las conexiones de WebSocket en los puertos 80 y 443 (SSL) y [comprueba si la causa puede ser otra](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)/span>.

## Preguntas frecuentes

*¿El rendimiento del tablero depende del plan que esté usando (gratis/de pago)?*

No, el plan que tengas no afecta el rendimiento del tablero.

*¿Los ajustes de uso compartido de mi tablero pueden afectar el rendimiento?*

La configuración de compartir no debería afectar al rendimiento del tablero, pero el número de usuarios de tu tablero puede influir en él. Puedes utilizar los consejos anteriores para las sesiones de colaboración.
