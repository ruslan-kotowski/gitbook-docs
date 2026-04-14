---
title: Chips inteligentes y capturas inteligentes para Google
article_id: 11845494577554
translation_id: 11845494577554
locale: es
sidebar_position: 11
created_at: '2023-06-06T12:19:20Z'
updated_at: '2025-08-15T13:44:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-workspace-smart-chips
availability:
  notes: 'Personas: Todos los usuarios Planes: Todos los planes Plataformas: Escritorio,
    navegador (cuando se usa Google Docs, Hojas de cálculo, Presentaciones)'
---

Google ofrece potentes capacidades de colaboración con su lienzo inteligente, que utiliza componentes básicos interactivos llamados chips inteligentes. Con el chip inteligente de Miro para Google, puedes agregar un acceso directo a un tablero de Miro directamente en tu Documento de Google, Diapositivas de Google o Hojas de Cálculo de Google, mejorando tus capacidades de colaboración.

Además, Miro ofrece capturas inteligentes, que te permiten pegar tableros y widgets de Miro directamente como imágenes en Documentos de Google, Diapositivas de Google y Hojas de Cálculo de Google con una funcionalidad mejorada para mantener el contenido sincronizado.

![Miro smart chip board preview in Google Docs](../../../../../../docs/integrations-apps/google/images/21017516136210_miro_smart_chip_board_preview.png)
*El complemento para el chip inteligente de Miro en Google Docs*

## Configurar los chips inteligentes de Miro

Sigue estos pasos para integrar enlaces de tableros de Miro como chips inteligentes en tu Documento de Google, Diapositivas de Google o Hojas de Cálculo de Google.

:::note
Es posible que el administrador de tu Google Workspace deba instalar el complemento de Miro para tu organización o equipo. Si no está disponible, consúltalo con tu administrador. [Obtén más información](https://support.google.com/a/topic/1056395?hl=en&ref_topic=27380).
:::

1. Dentro de tu documento de Google, pega un enlace a tu tablero de Miro y luego presiona **Tab**. Google verificará si el enlace contiene un chip.
2. A continuación, Google comprobará si ya tienes instalado el complemento de Google Workspace para Miro. Luego, se ejecutará una de estas dos opciones:
   1. Si ya tienes el complemento de Google Workspace instalado, no es necesario instalar chips inteligentes; ya los tienes. Verás una vista previa de tu tablero cuando hagas clic en el enlace.
   2. Si no has instalado el complemento, se te pedirá que lo instales desde el Marketplace de Google Workspace.

      > ✏️ Quizás necesites que el administrador de Google instale el complemento por ti.
3. A continuación, Google te pedirá que te conectes a tu cuenta de Miro. Esto es necesario para mostrar cierta información del tablero y determinar si tienes acceso al tablero al que te estás vinculando. Haz clic en **Conectar a Miro**.

   ![Connect Miro to Google Workspaces dialog](../../../../../../docs/integrations-apps/google/images/21017529158034_Google%20Smart%20Chips%20connect.png)
*Conectando Miro a Google Workspaces*
4. Luego, se ejecutará una de estas dos opciones:
   1. Si ya estás autorizado para acceder a este tablero, verás el chip con una vista previa del tablero y metadatos como el propietario del tablero y la última fecha de modificación.
   2. Si necesitas que te autoricen, verás un botón de **Solicitar acceso**. Haz clic en el botón para enviar la solicitud al propietario del tablero.

      ![Miro smart chip request access to board button](../../../../../../docs/integrations-apps/google/images/21017529156882_miro_smart_chip_request_access_to_board.png)*Solicitar acceso a un tablero privado*
5. Una vez que el acceso se haya aprobado, verás el chip con una vista previa del tablero. Si no ves la vista previa, actualiza tu documento.
6. Tu tablero ahora se ha agregado al documento y, al hacer clic en él, irás al tablero de Miro. Cualquier persona con acceso al tablero puede crear un chip inteligente en su documento de Google.

   ![Connected Miro smart chip board link in Google Docs](../../../../../../docs/integrations-apps/google/images/21017516138642_Connecting%20Google%20Smart%20Chip.gif)
*Conectar un enlace de tablero con chip inteligente de Miro a Google Workspaces*

## Usa capturas inteligentes de Miro

La integración del panel lateral de Miro te permite insertar contenido de tableros de Miro directamente en Documentos, Diapositivas o Hojas de cálculo de Google sin salir de tu documento. Esta función ofrece acceso sin problemas a tus tableros de Miro y te permite insertar contenido visual con funcionalidad mejorada.

### Panel lateral de Miro

El panel lateral de Miro en Documentos, diapositivas o Hojas de cálculo de Google incluye las siguientes capacidades:

- **Acceso directo al tablero:** Accede a tus tableros de Miro directamente desde Documentos, diapositivas o Hojas de cálculo de Google sin cambiar de aplicación.
- **Selección de tablero:** Elige entre tus tableros de Miro disponibles usando el botón "Seleccionar tablero de Miro para insertar".
- **Vista previa interactiva:** Ve y selecciona contenido específico de tu tablero de Miro antes de insertarlo.
- **Colocación precisa:** Inserta el contenido exactamente donde esté el cursor en el documento.
- **Funcionalidad inteligente:** El contenido insertado mantiene la conexión con el tablero original de Miro.

### Cómo usar el panel lateral de Miro

1. En tus Documentos, diapositivas o Hojas de cálculo de Google, coloca el cursor en el documento donde desees insertar el contenido de Miro.
2. Abre el panel derecho haciendo clic en el ícono de integración de Miro.
   ![Screenshot 2025-07-11 at 11.05.03.png](../../../../../../docs/integrations-apps/google/images/28006926984466_Screenshot%202025-07-11%20at%2011.05.03.png)
3. Haz clic en **Seleccionar tablero de Miro para insertar** para elegir entre tus tableros de Miro disponibles.
   ![Screenshot 2025-07-11 at 11.09.05.png](../../../../../../docs/integrations-apps/google/images/28006941150482_Screenshot%202025-07-11%20at%2011.09.05.png)
4. Busca y selecciona el área, marco o contenido específico que deseas insertar desde la vista previa del tablero.
   ![Screenshot 2025-07-11 at 11.10.17.png](../../../../../../docs/integrations-apps/google/images/28006926986130_Screenshot%202025-07-11%20at%2011.10.17.png)
5. Usa cualquier opción del menú desplegable disponible para elegir diferentes configuraciones de visualización o selecciones.
6. Haz clic en **Confirmar** para insertar el contenido en la posición de tu cursor.

El contenido insertado aparecerá como una captura de pantalla en tu documento con una conexión de smart chip al tablero original de Miro.

:::note
**Nota:** El panel lateral de Miro requiere que el complemento de Miro para Google Workspace esté instalado. La función funciona con Documentos de Google, Diapositivas de Google y Hojas de cálculo de Google.
:::

## Gestiona el complemento como administrador.

Revisa estos puntos si eres un administrador de Google Workspace que gestiona el complemento de Miro:

1. El complemento Google Workspace se puede instalar o eliminar solo desde Google.
2. Si quieres restringir el acceso a los chips inteligentes de Google, esto debe hacerse desde Google; Miro no tiene control sobre qué usuarios instalan y usan los chips inteligentes.

## Preguntas frecuentes

Estas son las respuestas a las preguntas comunes sobre los chips inteligentes de Miro para Google.

¿Cuál es la diferencia entre los chips inteligentes y el panel lateral de Miro?

Los chips inteligentes crean enlaces clicables a tableros de Miro dentro de tus documentos de Google, mientras que el panel lateral de Miro te permite insertar contenido visual de tus tableros de Miro directamente en Documentos y diapositivas de Google. El panel lateral proporciona una manera integrada de seleccionar e insertar contenido específico del tablero sin salir de tu documento.

¿Qué aplicaciones de Google Workspace admiten integración con Miro?

Los chips inteligentes funcionan con Documentos de Google y el panel lateral de Miro funciona tanto con Documentos como con diapositivas de Google. El soporte para Hojas de cálculo de Google está determinado por Google. Por favor, vuelve a consultar el Centro de Ayuda para conocer las actualizaciones.

¿Con qué tipo de enlaces funcionan los chips inteligentes?

El chip inteligente de Miro para Google admite enlaces a tableros y objetos de tableros de Miro.

¿Cómo se mantienen actualizados los elementos de tableros de Miro insertados?

El contenido insertado a través del panel lateral de Miro mantiene una conexión con el tablero original de Miro. Aunque no se sincroniza automáticamente, puedes actualizar el contenido insertado para asegurarte de que refleje la última versión de tu tablero de Miro.

¿Cómo funciona el panel lateral de Documentos de Google?

El panel lateral de Documentos de Google proporciona acceso directo a tus tableros de Miro sin salir de tu documento. Haz clic en el icono de integración de Miro para abrir el panel lateral derecho, luego usa "Seleccionar tablero de Miro para insertar" para elegir entre tus tableros disponibles. El panel te permite previsualizar y seleccionar áreas o marcos específicos antes de insertarlos en tu documento en la posición de tu cursor.
