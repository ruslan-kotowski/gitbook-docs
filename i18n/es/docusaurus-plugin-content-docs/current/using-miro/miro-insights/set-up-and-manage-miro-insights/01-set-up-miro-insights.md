---
title: "Configuraci\xF3n de Miro Insights"
article_id: 30122381753106
translation_id: 30122381753106
locale: es
sidebar_position: 0
created_at: '2025-10-10T10:26:28Z'
updated_at: '2025-11-25T15:54:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Conectar tus herramientas a Miro Insights es un primer paso crucial para obtener un valor real. Las integraciones permiten que Miro Insights extraiga automáticamente comentarios de clientes y datos relevantes de todos tus sistemas. Esta guía es para los admins de empresa que habilitarán estas conexiones.

Si eres un integrante del equipo que busca usar Miro Insights después de su configuración, consulta el artículo sobre [Uso de Miro Insights](../../miro-insights/use-miro-insights).

## Requisitos previos

Para configurar las integraciones de Miro Insights necesitas cumplir con los siguientes requisitos:

- Debes ser un **admin de empresa en Miro**.
- Debes tener **acceso de administrador o API en la plataforma externa** a la que te estás conectando.

:::note
Asegúrate de que tu **plan de Miro incluya Miro Insights**. Si Miro Insights es un complemento o está en lanzamiento limitado, tu cuenta debe ser elegible. Además, algunas integraciones pueden requerir ediciones específicas del software externo. Por ejemplo, cierto acceso a la API de CRM está disponible en planes de nivel superior.
:::

## Prepara tus fuentes de datos

Antes de conectar tus fuentes de datos a Miro Insights, es importante preparar tus datos y establecer una taxonomía clara. Esta preparación garantizará que obtengas los insights más precisos y accionables desde la plataforma.

### Limpia y optimiza tus datos

Antes de sincronizar datos con Miro Insights, limpia y optimiza tus fuentes de datos:

- Elimina duplicados y elementos obsoletos.
- Limpia opiniones inconsistentes o irrelevantes.
- Asegura la calidad de los datos en tus sistemas de origen.
- Aborda las principales inconsistencias o vacíos de datos con anticipación.

### Establece tu taxonomía

Aunque Miro Insights incluye categorías básicas generadas por inteligencia artificial, se recomienda definir tu propia taxonomía estandarizada antes del lanzamiento. Esto garantiza la consistencia y mejora la calidad de las ideas desde el inicio.

Considera incluir estas categorías estándar:

- Solicitudes de funciones
- Errores
- Puntos problemáticos de UX
- Segmentos de clientes
- Niveles de prioridad
- Unidades de negocio
- Iniciativas estratégicas

Prácticas recomendadas para la taxonomía:

- Usa terminología que coincida con el lenguaje de tu equipo.
- Crea directrices claras sobre cómo y cuándo usar cada categoría.
- Comparte la taxonomía con tu equipo para asegurar un uso consistente.
- Revisa y refina las categorías regularmente según sea necesario.
- Considera mapear hacia tus iniciativas estratégicas y OKRs.

:::tip
Comunícate con el soporte de Miro Insights para obtener ayuda en la definición de tu taxonomía. Ellos pueden proporcionar ejemplos y mejores prácticas basadas en otros clientes de tu industria.
:::

## Conectar una integración

Cuando tus datos estén listos, puedes conectar tus integraciones. Miro Insights es compatible con una variedad de herramientas populares en CRM, asistencia, llamadas de Ventas, gestión de proyectos y plataformas de chat.

En la pestaña de **Integraciones y Automatizaciones** de configuración, puedes ver y gestionar todas tus integraciones conectadas. Cada integración se enumera con su estado de conexión y opciones para configurar o desconectar.

Para conectar una integración:

1. Desde la aplicación de **Miro Insights**, selecciona el ícono de **Configuración** en la parte superior de la barra lateral izquierda.
2. En el panel de **Configuración**, ve a la pestaña de **Integraciones y Automatizaciones**.
3. Selecciona **Conectar** junto a la integración que deseas añadir.
4. **Autorizar acceso**. Se abrirá una ventana emergente que te pedirá autorizar a Miro Insights para acceder a esa herramienta.
   Esto normalmente implica iniciar sesión en el servicio externo y otorgar permisos. Por ejemplo, al conectar Salesforce, debes iniciar sesión con tu cuenta de admin de Salesforce y aprobar la integración. Para Slack, selecciona un espacio de trabajo y autoriza la aplicación de Slack de Miro Insights. Sigue las instrucciones en pantalla para cada uno.
5. **Configurar ajustes de importación**. Una vez conectado, la integración aparecerá como "Conectado" con opciones adicionales de configuración. Aquí puedes establecer:
   - **Importar conversaciones desde**: Para fuentes basadas en conversaciones como Gong o Zendesk, puedes elegir una fecha. Esto evita traer datos antiguos a menos que los necesites.
   - **Reglas de importación automática**: Activa o desactiva si los nuevos ítems deben ser importados automáticamente. Puedes habilitar esta opción para que las nuevas llamadas o tickets ingresen de forma continua. Si la dejas desactivada, podrás importar ítems manualmente o selectivamente.
   - **Si la IA detecta solicitudes con**: Algunas fuentes te permiten filtrar por confianza en la detección por IA.
   - **Detectar incidencias**: Habilita Miro Insights para identificar y extraer automáticamente incidencias de los comentarios de los clientes. Estas incidencias pueden incluir desafíos de usabilidad, problemas de rendimiento, preocupaciones de seguridad, etc.

Otras opciones pueden variar según la integración. Por ejemplo, en Jira, puedes seleccionar de qué proyecto(s) extraer las funciones o mapear campos personalizados.

### Filtrado por IA

Algunas integraciones te permiten **filtrar por detección de IA**. Esto significa que Insights escaneará la transcripción de una llamada y solo creará un ítem de comentarios si está razonablemente seguro de que se mencionó una solicitud de producto. Esto reduce el ruido de conversaciones no relacionadas. Puedes ajustar el umbral de confianza o desactivar esta opción para importar todo.

### Filtros por etiqueta o campo

En herramientas como Zendesk, puedes especificar una etiqueta. Por ejemplo, "feature_request", y así solo se procesarán los tickets que tengan esa etiqueta. En Jira, puedes seleccionar un proyecto específico o tipo de incidencia para importar como funciones.

### Sincronización de incidencias

Para herramientas de proyectos como Jira, puedes tener opciones para mapear campos. La captura de pantalla de arriba muestra un ejemplo "Enviar el valor en dólares de la función a un campo personalizado" – podrías seleccionar un campo personalizado en Jira para completar con el impacto económico calculado de Miro Insights, cerrando el ciclo de nuevo a ingeniería. Este paso es opcional pero puede ser poderoso.

Conecta todos los sistemas que sean relevantes. Recomendamos como mínimo conectar un CRM y una fuente de soporte o comentarios para comenzar, así obtienes tanto contexto de cuenta como retroalimentación cruda. Siempre puedes añadir más después.

Una vez hecho esto, habrás conectado exitosamente tus integraciones a Miro Insights. El sistema comenzará a sincronizar los datos. La sincronización inicial puede tardar un poco si hay muchos datos históricos (verás las marcas de tiempo de la última sincronización junto a cada integración). Puedes monitorear el estado de la sincronización en la lista de Integraciones: muestra la hora de la última sincronización y ofrece una opción para desconectar si es necesario.

## Importar elementos manualmente

También puedes importar funciones y elementos de comentarios manualmente usando un archivo CSV. Esto es útil para importaciones únicas o si tienes una lista de solicitudes de funciones o comentarios de otra fuente.

Para importar funciones a través de CSV:

1. En Miro Insights, ve a la vista de **Backlog**.
2. Haz clic en el botón **Importar** en la parte superior derecha.
3. Selecciona **Cargar CSV**.
4. Selecciona la columna en tu fuente de datos CSV que mejor coincida con las propiedades de Miro Insights.
5. Selecciona **Importar función** para completar el proceso.

Tus funciones importadas ahora aparecerán en la sección de [Backlog](../../tools/use-miro-insights/05-backlog.md).

Para importar elementos de comentarios a través de CSV:

1. En Miro Insights, ve a la vista de **Comentarios**.
2. Haz clic en el botón **Importar** en la parte superior derecha.
3. Selecciona **Cargar CSV**.
4. Mapea las columnas de tu CSV a las propiedades de comentarios de Miro Insights (por ejemplo, título, descripción, fuente).
5. Selecciona **Importar comentarios** para completar el proceso.

Tus comentarios importados ahora aparecerán en la sección de [Comentarios](../../tools/use-miro-insights/07-feedback.md).

## Conectar herramientas no compatibles usando Zapier

Si tienes una herramienta que no es compatible directamente, a menudo puedes utilizar [Zapier](http://zapier.com/) para dirigir los datos a Miro Insights. Por ejemplo, podrías crear el siguiente flujo de trabajo con Zapier. Cuando se envía un Google Form o aparece una nueva entrada en una base de datos personalizada, crea un comentario en Miro Insights.

Para obtener los pasos detallados, consulta el artículo sobre [Uso de Zapier con Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/03-connect-tools-with-zapier.md).

## Pasos adicionales

Después de conectar tus integraciones, puedes realizar algunos pasos opcionales para asegurarte de que todo esté configurado correctamente:

### Importar o verificar funciones

Si conectaste un rastreador de tareas como Jira, revisa el Backlog en Miro Insights para ver si tus funciones o épicas existentes han aparecido. Si no es así, podrías usar el botón de Importar en la vista de Backlog para cargar un archivo CSV o activar una extracción desde Jira. Asegúrate de que cada función importada tenga un título y una descripción claros; la IA depende de ese texto para coincidir con los comentarios relevantes.

### Configura comandos de Slack o reenvío de correos electrónicos

Si agregaste Slack, informa a tu equipo cómo enviar mensajes a Insights. Por ejemplo, haz clic con el botón derecho en un mensaje > "Enviar a Miro Insights".

Para correo electrónico u otros canales, podrías configurar el reenvío. Algunos equipos configuran una dirección de correo específica que reenvía automáticamente a una herramienta como Intercom o un hook de Zapier para la ingesta.

> **Consejo**: Es recomendable revisar periódicamente tus ajustes de integración. Por ejemplo, si notas que recibes demasiadas opiniones triviales de una fuente, ajusta los filtros o incrementa el umbral de confianza de la IA. Por el contrario, si falta información que esperabas, verifica que la integración esté conectada con el alcance correcto (por ejemplo, el proyecto o la etiqueta adecuada). Una configuración bien ajustada de integración mantiene señales altas y ruido bajo en tus insights.

## Desconectar una integración

Si alguna vez necesitas desconectar una integración:

1. Ve a **Ajustes** > **Integraciones y Automatizaciones**.
2. Encuentra la integración que deseas eliminar.
3. Selecciona **Desconectar** al lado de ella.
4. Confirma la desconexión en la instrucción emergente.

Esto detendrá cualquier futura sincronización de datos desde esa fuente.

> **Importante**: En algunos casos, por ejemplo Gong, desconectar también podría eliminar elementos de comentarios importados previamente. En otros casos, como Jira, las funciones existentes pueden permanecer, pero no recibirán actualizaciones. Revisa el comportamiento específico de cada integración en la documentación o contacta al soporte si tienes dudas.

Asegúrate de comunicarte con tu equipo si desconectas una fuente principal, ya que puede afectar la integridad del backlog y los comentarios en Miro Insights.

## ¿Qué sigue?

Al conectar integraciones, has sentado las bases para que Miro Insights entregue perspicaces y continuos conocimientos sobre el producto. Los datos comenzarán a fluir y la inteligencia artificial empezará a hacer conexiones.

Ahora puedes proceder a [usar Miro Insights](../../miro-insights/use-miro-insights) o aprender más sobre las tareas administrativas en curso, incluidas las configuraciones generales, la gestión de equipos, las notificaciones y el acceso a la API en la [guía de administración de Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/02-manage-miro-insights.md).
