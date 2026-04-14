---
title: Tablas
article_id: 22760922335506
translation_id: 22760922335506
locale: es
sidebar_position: 11
created_at: '2024-11-20T17:33:53Z'
updated_at: '2026-03-13T12:26:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Las tablas son una herramienta interactiva que te permite estructurar tu contenido en Miro, convirtiendo ideas en planes de acción.

> ***Disponible en:** Todos los dispositivos*
> ***Disponible para:** Todos los planes de Miro*
> ***Quién puede hacerlo:** Propietarios de tableros y editores*

## Funciones principales

Las tablas incluyen las siguientes funciones principales:

- **Crear campos personalizados**
  Organiza y estructura tu información con campos personalizados.
- **Crear registros a partir de tarjetas de Miro**
  Arrastra y suelta tarjetas de Miro en el widget de tablas para crear nuevos registros.
- **Crear registros a partir de notas adhesivas**
  Consulta Agregar una tarjeta de Miro o nota adhesiva a una tabla.
- **Crear registros sincronizados de tarjetas de Jira**
  Consulta Agregar una tarjeta de Jira a una tabla.
- **Capacidades avanzadas de filtrado y ordenamiento**
  Filtra y ordena las tablas para organizar y priorizar registros.
- **Agrupar registros**
  Organiza los registros en una tabla por campo para agrupar la información de manera lógica.
- **Crear tablas sincronizadas en varios tableros**
  Copia y pega una tabla para crear una vista sincronizada de los mismos registros
- **Cronograma**
  Cambia a una vista de cronograma para ver tus datos en un nuevo diseño.
- **Cálculos de columna**
  Calcula agregados como suma, promedio y más para campos numéricos para analizar tus datos de un vistazo.
- **Formato visual de números**
  Da formato a los números como barras de progreso con visualización de porcentaje o moneda y utiliza reglas de formato condicional para resaltar valores que cumplan con criterios específicos. Consulta [Números visuales en Tablas](04-visual-numbers-in-tables.md).
- **Dependencias**
  Mapea y visualiza dependencias entre registros usando campos de "bloqueado por" y "bloqueando" entre proyectos.
- **Acciones en masa**
  Realiza acciones como editar, mover, duplicar y eliminar en múltiples registros al mismo tiempo, o arrastra múltiples registros al lienzo como tarjetas.

## Agrega una tabla a tu tablero

:::warning
Los editores invitados no tienen la capacidad de agregar o editar tablas.
:::

1. Abre un tablero de Miro.
2. Haz clic en el icono de **Herramientas, medios e integraciones** (**+**) en la barra de herramientas de creación.
   Se abre el panel de Herramientas, medios e integraciones.
3. Busca y selecciona **tabla**.
   Tu cursor ahora muestra el icono de la tabla.
4. Haz clic en cualquier parte del tablero de Miro para colocar tu widget de tabla.

## Convertir un archivo de Excel a una tabla

1. Abre un tablero de Miro.
2. Haz clic en el icono de **Herramientas, Medios e Integraciones** (**+**) en la barra de herramientas de creación.
   El panel de Herramientas, Medios e Integraciones se abre.
3. Busca y selecciona **Cargar**.
   El panel de Cargar se abre.
4. Selecciona **Mi dispositivo**.
5. Navega y selecciona el archivo Excel (.xlsx) que deseas cargar.
6. Se abrirá un modal con opciones:
   1. Convertir a tabla.
   2. Convertir a cuadrícula.
   3. Agregar como archivo.
7. Selecciona **Convertir a tabla** y elige si deseas **Usar la primera fila como encabezados**.
8. Haz clic en **Seleccionar**.
9. Se creará una tabla en el tablero con los datos del archivo de Excel.

:::warning
Al cargar un archivo de Excel, hay un límite de 500 filas y 30 columnas.
:::

## Copiar y pegar tablas

Básicamente tienes dos opciones al copiar y pegar tablas, ya sea dentro de un tablero o entre tableros. La primera opción es crear una tabla sincronizada que mostrará actualizaciones en cada ubicación. La segunda opción es crear una tabla no sincronizada, que funciona como una plantilla.

1. Selecciona la tabla que deseas copiar.
2. Haz clic en el menú contextual (![icon-main.svg](../../../../../../docs/using-miro/formats/images/22916604338834_icon-main.svg)) y selecciona Copiar. También puedes usar el atajo de teclado Ctrl + C (en Windows) o Comando + C (en Mac).
3. Navega al lugar en el tablero donde deseas pegar la tabla.
4. Haz clic derecho y selecciona Pegar. También puedes usar el atajo de teclado Ctrl + V (en Windows) o Comando + V (en Mac).
   Aparecerá una ventana emergente.
5. Selecciona si deseas crear una tabla sincronizada o una nueva tabla en la ventana emergente.

## Gestionar permisos para las tablas

Si creas una o más vistas sincronizadas de una tabla en diferentes tableros de Miro, tendrás que gestionar los permisos para asegurarte de que, al añadir una vista sincronizada de una tabla a un nuevo tablero, puedas ver y gestionar quién tiene acceso de edición y visualización a esa tabla. Los permisos para las vistas sincronizadas de tablas son gestionados por el tablero principal—el tablero en el que se creó la tabla original.

Al pegar una tabla en un nuevo tablero como una vista sincronizada, se mostrará un pop-up si no todos los usuarios del tablero tienen permisos de vista o edición para la tabla. Si deseas ver o editar los permisos de la tabla, se te dirigirá al tablero original donde aparece la tabla para realizar cambios.

Si un usuario en un tablero no tiene acceso al tablero principal donde se creó la Tabla original, esta aparecerá en un estado de no acceso para ellos. Si el usuario solo tiene acceso para ver el tablero principal, podrá ver la Tabla en el nuevo tablero, pero no podrá editar ninguno de los registros ni cambiar la vista aplicando filtros, ordenaciones, grupos, etc.

## Interactuar con las tablas

El widget de tablas proporciona flexibilidad para crear el contenido que deseas y estructurarlo y organizarlo de la manera más efectiva para tu caso de uso.

Al crear una nueva tabla en tu tablero de Miro, se proporcionará un conjunto de campos predeterminados que se corresponden con los campos existentes encontrados en las tarjetas de Miro. Puedes eliminar, editar u ocultar estos campos o crear tus propios campos nuevos.

### Crear un campo

Sigue estos pasos para crear un nuevo campo:

1. Haz clic en el icono de + en la parte superior de la columna más a la derecha de la tabla.
   Se abrirá un menú.
   ![tables-adding-fields.png](../../../../../../docs/using-miro/formats/images/25142699942930_tables-adding-fields.png)
   *Agregar un nuevo campo a una tabla*
2. Haz clic en el tipo de campo que quieres crear desde el menú. Hay opciones para campos de Miro y tipos de campo personalizados.
   Se abrirá un cuadro de diálogo de opciones.
3. Ingresa la información del campo (nombre del campo y, en el caso del campo de selección, las opciones para el menú desplegable) en el cuadro de diálogo y haz clic en Guardar.

:::note
El tipo de campo Enlace solo está disponible para los planes Business y Enterprise.
:::

### Editar el nombre de un campo u opciones

1. Pasa el cursor sobre el nombre del campo.
   Un icono de tres puntos (...) aparecerá.
2. Haz clic en el icono de **tres puntos** (**...**).
   Se abrirá un menú.
3. Haz clic en **Editar campo**.
   Se abrirá un cuadro de diálogo con las opciones de edición.
4. Edita el nombre del campo y/o las opciones y haz clic en **Guardar**.

### Borrar un campo

1. Pasa el cursor sobre el nombre del campo.
   Un icono de tres puntos (...) aparecerá.
2. Haz clic en el icono de **tres puntos** (**...**).
   Se abrirá un menú.
3. Haz clic en Borrar.

:::warning
Un campo eliminado no puede deshacerse. Se eliminará del Tabla actual y de todas las versiones sincronizadas inmediatamente.
:::

### Ocultar o mostrar un campo

Sigue estos pasos para ocultar o mostrar un campo individual:

1. Pasa el cursor sobre el nombre del campo.
   Aparecerá un icono de tres puntos (...).
2. Haz clic en el icono de **tres puntos** (**...**).
   Se abrirá un menú.
3. Haz clic en **Ocultar campo**.
   El campo se ocultará.
4. Para mostrar el campo, repite los mismos pasos anteriores pero haz clic en **Mostrar campo**.

También puedes ocultar o mostrar múltiples campos a la vez.

Sigue estos pasos para ocultar o mostrar múltiples campos:

1. Haz clic en el icono de **Ocultar** en la parte superior de la Tabla.
   Aparecerá una lista de campos en la Tabla.
2. Selecciona los campos que deseas ocultar o mostrar de la lista.

### Editar un registro

1. Haz doble clic en el registro que deseas editar.
   El registro se vuelve editable.
2. Edita el registro y presiona Intro.

Para aplicar formato o agregar un enlace al texto dentro de un registro:

1. Haz doble clic en el registro que deseas editar.
   El registro se vuelve editable.
2. Resalta el texto que quieres formatear.
   Aparecerá un menú contextual.
3. Aplica el formato o agrega un enlace al texto desde el menú contextual o utilizando [los atajos de teclado](../working-on-the-board/06-shortcuts-and-hotkeys.md).
4. Presiona Intro para guardar el registro.

El formato de texto también se puede aplicar en el panel lateral al editar un registro.

### Editar varios registros a la vez

1. Pasa el cursor sobre la fila para revelar la casilla de verificación a la izquierda.
2. Selecciona los registros que deseas editar usando las casillas de verificación en cada fila relevante.
   Aparecerá una barra de herramientas con opciones para editar.
3. Edita, mueve o duplica esos registros simultáneamente en la barra de herramientas.

### Eliminar un registro

1. Pasa el cursor sobre el registro que deseas eliminar.
2. Haz clic en el ícono de seis puntos para abrir el menú.
3. Selecciona **Eliminar**.

### Eliminar múltiples registros

1. Pasa el cursor sobre la fila para mostrar la casilla de verificación a la izquierda.
2. Selecciona los registros para editar usando las casillas de verificación de cada fila relevante.
   Una barra de herramientas aparecerá con opciones para editar.
3. Haz clic en el icono **Eliminar** en la barra de herramientas para eliminar todos los registros seleccionados.

### Añadir comentarios a las tablas

Facilita la colaboración agregando comentarios directamente a las partes de una tabla que deseas discutir.

1. Pasa el cursor sobre la fila a la que te gustaría agregar un comentario.
   En el lado derecho de la primera celda aparecerá un icono para agregar comentario.
2. Haz clic en el icono de **Agregar comentario**.
   Un panel lateral se abrirá a la izquierda.
3. En el panel, añade tu comentario y presiona Intro.

Una vez que se hayan agregado nuevos comentarios, aparecerá un conteo de comentarios junto al icono de Agregar comentario en cada fila. Haz clic en el icono para abrir el panel de comentarios.

Desde el panel de comentarios, puedes:

- Responder a comentarios.
- Añadir reacciones a los comentarios.
- Resolver un hilo de comentarios.
- Copiar un enlace al comentario.
- Seguir el hilo de comentarios para recibir notificaciones.
- Eliminar el hilo de comentarios.
- Editar un comentario que hayas dejado.

### Agregar una Tarjeta de Miro o una nota adhesiva a una Tabla

Puedes crear registros en una Tabla usando Tarjetas de Miro o notas adhesivas.

1. Selecciona la tarjeta o nota adhesiva que deseas copiar en la tabla.
2. Arrastra y suelta la tarjeta o nota adhesiva sobre la tabla.
   Aparecerá una línea azul donde se colocará el nuevo registro.
3. Se crea un nuevo registro, con el contenido de la tarjeta asignado a los campos correspondientes.
   En el caso de una nota adhesiva, el contenido se ubicará en el primer campo.

### Añadir una tarjeta de Jira a una tabla

Puedes arrastrar y soltar tarjetas de Jira en una tabla para crear registros sincronizados con Jira. Esto significa que puedes combinar el trabajo de Miro y Jira en una vista de tabla o cronograma para gestionar y seguir el trabajo del equipo completo en un solo lugar.

1. Encuentra la tarjeta de Jira relevante en el lienzo.
2. Arrastra la tarjeta hacia la Tabla.
3. Suelta la tarjeta en la fila objetivo dentro de la Tabla.

Cualquier cambio realizado en Miro se reflejará en Jira y viceversa. Los siguientes campos dentro de la Tabla se sincronizarán con Jira:

- Título
- Descripción
- Estimación
- Fecha de inicio
- Fecha de finalización
- Asignado a (Beta)
- Estado (Beta)

Todos los demás campos en la tabla se almacenan únicamente en Miro y no se sincronizan con Jira.

**Más información:** Consulta [preguntas frecuentes sobre tarjetas de Jira](../../integrations-apps/atlassian/17-jira-cards-faq.md).

### Trabaja con varias tarjetas de Jira a la vez

Al editar en masa registros sincronizados con Jira, solo estarán disponibles las acciones y campos compatibles con la integración de Jira. Las acciones no compatibles se ocultarán o deshabilitarán en el menú de acciones en masa.

### Filtrar una Tabla

Puedes filtrar los contenidos de una Tabla por uno o más campos para ayudar a reducir la vista/los registros con los que deseas trabajar.

1. Haz clic en el **ícono de filtro** en la parte superior de la tabla.
   Se abrirá un diálogo.
2. Selecciona si deseas **Agregar filtro** o **Agregar grupo de filtros**.
   Se abrirá un diálogo.
3. Especifica los parámetros del filtro: el campo en el que basar el filtro, la lógica del filtro y el contenido específico para el filtro.
   La tabla se filtra en tiempo real.
4. Haz clic en cualquier lugar fuera del diálogo de filtro para cerrarlo.

### Ordenar una Tabla

1. Pasa el cursor sobre el nombre del campo.
   Aparecerá un icono de tres puntos (...).
2. Haz clic en el icono de **tres puntos** (**...**).
   Se abrirá un menú.
3. Haz clic en **Ordenar ascendente** o **Ordenar descendente**.

Para eliminar la ordenación en una tabla:

1. Haz clic en el **icono de ordenar** en la parte superior de la tabla.
   Se abrirá un diálogo.
2. Haz clic en **Eliminar orden**.

### Buscar en una tabla

1. Haz clic en el icono de **Buscar** en la barra de herramientas superior de la Tabla.
2. Escribe tu consulta de búsqueda.
3. Los resultados relevantes aparecerán mientras escribes.
4. Puedes navegar por los resultados usando los iconos de flecha en la barra de búsqueda o desplazándote por la Tabla.
5. Haz clic en el icono de **Limpiar** (**X**) para volver a la Tabla completa.

### Agrupar registros por campo

1. Haz clic en el icono de **Agrupar** en la parte superior de la Tabla.
   Se abre un menú.
   ![table-group-records.png](../../../../../../docs/using-miro/formats/images/25142699944338_table-group-records.png)
   *Agrupación de registros en una Tabla*
2. Selecciona el campo por el que deseas agrupar los registros.
   Los registros en la Tabla se agruparán por el campo elegido.

:::note
Cuando arrastras un registro a un grupo existente, el valor del campo correspondiente se actualizará para coincidir con ese grupo.
:::

Para eliminar la agrupación en una Tabla, sigue estos pasos:

1. Haz clic en el icono de **Grupo** en la parte superior de la tabla.
   Se abrirá un menú.
2. Haz clic en **Borrar agrupación**.

### Tarjetas sincronizadas

Puedes arrastrar y soltar registros desde la tabla a tu lienzo para crear una tarjeta sincronizada.

1. Pasa el cursor sobre el registro del que te gustaría crear una tarjeta sincronizada.
   Los iconos aparecerán en el lado izquierdo del registro.
2. Haz clic y mantén presionado el icono de puntos y arrástralo al lienzo.
   Se creará una tarjeta con la información de ese registro.
3. La tarjeta se actualizará siempre que el registro en la tabla se actualice, y viceversa.

Puedes saber si una tarjeta está sincronizada con una Tabla a través de un ícono de base de datos que aparecerá en la esquina inferior derecha de la tarjeta.

Si eliminas un registro, la tarjeta sincronizada correspondiente permanecerá en el tablero, pero ahora aparecerá en blanco.

Si eliminas una tarjeta sincronizada en el lienzo, el registro permanecerá en la Tabla.

Si arrastras una tarjeta sincronizada existente en la Tabla de la que se origina, no funcionará, ya que se trata como un registro único en esa Tabla. Sin embargo, puedes arrastrar una tarjeta sincronizada existente a una nueva Tabla y aparecerá en la Tabla como un nuevo registro no sincronizado.

### Ver una Tabla como un Cronograma

Sigue estos pasos para cambiar a la vista de Cronograma:

1. Haz clic en el icono de **Tabla** en la parte superior de la Tabla.
   Se abrirá un cuadro de diálogo.
2. Selecciona **vista de cronograma** (o vuelve a cambiar a **vista de tabla**).

Cuando cambias a la vista de cronograma, se utilizan la fecha de inicio y la fecha de finalización predeterminadas, si están disponibles, para representar los registros en tu Tabla como barras correspondientes en tu cronograma. El campo de Título y el campo de asignado se usan para mostrar el nombre del registro y el asignado en la barra.

**Más información:** [Cronograma](15-timeline.md)

## Cálculos de columna

> **¿Cuáles planes?:** Business, Enterprise

Los cálculos de columnas te permiten realizar funciones agregadas en campos numéricos en tu Tabla, ayudándote a analizar y resumir tus datos. Puedes calcular suma, promedio, cuenta, mínimo, máximo y valores medianos para cualquier columna numérica.

1. Abre el menú de opciones del campo haciendo clic en el encabezado de la columna que contiene los datos.
2. Selecciona **Mostrar cálculo de columna** del menú.
3. Elige el tipo de cálculo que deseas aplicar:
   1. Suma: Suma todos los valores de la columna
   2. Promedio: Calcula el promedio de todos los valores
   3. Recuento: Cuenta el número de entradas
   4. Min: Muestra el valor más pequeño
   5. Máximo: Muestra el valor más grande
   6. Mediana: Muestra el valor del medio
4. El resultado del cálculo aparecerá en una fila de pie al final de la Tabla.

Para eliminar un cálculo de columna:

1. Haz clic en la opción **Calcular** dentro de la fila de pie de página.
2. Selecciona **Ninguno**.
3. Repite hasta que el último Cálculo haya sido configurado a Ninguno.

:::note
Puedes aplicar un cálculo por columna. Cuando filtras o agrupar tu tabla, los cálculos se actualizan automáticamente para reflejar solo los registros visibles. En vistas agrupadas, los cálculos aparecen para cada grupo, así como un total general.
:::

Los cálculos de columna funcionan perfectamente con el formato visual de números. Cuando aplicas un formato visual a una columna calculada, el resultado se muestra como una barra de progreso siguiendo tus reglas de formato. Ver [Números visuales en tablas](04-visual-numbers-in-tables.md).

## Fórmulas multicolumna

> **Qué planes:** Business, Enterprise

Además de los cálculos por columna, puedes crear campos para fórmulas que involucren múltiples columnas. Los campos de fórmula calculan a través de varias columnas en la misma fila.

Para crear un campo de fórmula:

1. Haz clic en el icono **+** para agregar un nuevo campo.
2. Selecciona el tipo **Fórmula**.
3. Usa el constructor visual de fórmulas para seleccionar campos, constantes y operadores (+, -, ×, ÷, (,)).
4. Tu fórmula se calcula automáticamente para cada fila.

:::note
Los campos de fórmulas actualmente soportan campos numéricos y constantes.
:::

## Relaciones (Dependencias)

> **Para cuáles planes:** Business, Enterprise

Este tipo de campo de relación te permite mapear dependencias entre registros en tu Tabla usando los campos "bloqueado por" y "bloqueando". Esto te ayuda a rastrear las relaciones del proyecto y entender cómo los elementos de trabajo dependen unos de otros.

### Crear campos de dependencia

1. Haz clic en el **icono +** para agregar un nuevo campo.
2. Elige una de las siguientes opciones:
   1. **Bloqueado por** - Para mostrar qué registros deben completarse antes que este.
   2. **Bloqueando** - Para mostrar qué registros están esperando por este.
3. Nombra tu campo y haz clic en Crear.

### Agregar dependencias entre registros

Una vez que hayas creado campos de dependencias, puedes enlazar registros siguiendo estos pasos:

1. Haz clic en una celda en la columna de **Bloqueado por** o **Bloqueando**.
2. Selecciona el o los registros que quieres vincular desde el menú desplegable.
3. Haz clic fuera de la celda para guardar.

:::note
Los registros pueden tener múltiples relaciones de bloqueado por y bloqueando. Las dependencias se sincronizan en todas las tablas sincronizadas, asegurando consistencia en tus vistas y tableros.
:::

:::warning
**Limitaciones actuales (Beta):**

- Las dependencias aún no son compatibles para registros sincronizados con Jira u otras integraciones de terceros
- Los indicadores visuales para dependencias aún no se muestran en las tarjetas sincronizadas
- Los ajustes automáticos de fechas basados en dependencias aún no están disponibles
:::

## Relaciones (Nesting) (BETA)

> **Para qué planes:** Business, Enterprise

El tipo de campo de relación de anidamiento te permite crear una jerarquía entre registros en tu Tabla usando campos de **Padre** e **Hijo**.

### Crear campos jerárquicos

1. Haz clic en el icono **+** para añadir un nuevo campo.
2. Elige entre:
   1. **Padre**: Usa este campo para vincular un registro a su elemento de nivel superior (por ejemplo, una función vinculada a un épico).
   2. **Hijo**: Usa este campo para vincular un registro a sus elementos de nivel inferior (por ejemplo, una iniciativa con sub-tareas).
3. Nombra tu campo y haz clic en **Crear**.

### Vincular registros padre e hijo

1. Haz clic en una celda en la columna de **Padre** o **Hijo**.
2. Selecciona el(los) registro(s) que quieres vincular desde el menú desplegable.
3. Haz clic fuera de la celda para guardar.

### Visualiza tu jerarquía

1. Haz clic en el icono de **Configuración de vista** en el encabezado de tablas.
2. Activa **Anidación**.

Usa el **cheurón** junto a los registros Padre para mostrar u ocultar los registros Hijo.

:::note
*La anidación y jerarquía están ocultas por defecto. Deberás activarlas en estas configuraciones.*
:::

### Otras formas de crear jerarquía

1. Haz clic en **Añadir subregistro** a través del **menú de 6 puntos** a la izquierda en cada fila.
2. El anidamiento se activará por defecto.

   > ✏️ Se crearán campos de Elemento principal e Hijo, pero estarán ocultos. Para mostrar estos campos, ve al menú Ocultar campos en el encabezado de la Tabla.

   > ✏️ Para desactivar el anidamiento, ve a las Configuraciones de vista en el encabezado de las Tablas.
3. Puedes gestionar las jerarquías a través de los campos de Elemento principal e Hijo.
4. Cuando el anidamiento está activado, también puedes arrastrar y soltar para crear jerarquías.

:::warning
*Si eliminas un registro principal, todos los registros secundarios de este también se eliminarán. Usa la función Deshacer para revertir esto si es necesario.*
:::

Si los campos Principal y Secundario no están ocultos, serán visibles en el panel lateral. Puedes cambiar a la vista de Cronograma y observar cómo tu portafolio se despliega con el tiempo.

:::warning
***Limitaciones actuales (Beta):***

- *Máximo de cuatro niveles para la jerarquía.*
- *La anidación aún no es compatible para registros sincronizados con Jira o integraciones de terceros.*
- *Los indicadores visuales para la anidación aún no se muestran en las tarjetas sincronizadas.*
:::

## Modo sin distracciones

Puedes editar y ver tu tabla en modo sin distracciones (pantalla completa). Simplemente haz clic en el **ícono de flecha diagonal** en la parte superior del widget. Las configuraciones como Filtro, Ordenar, Agrupar y Ocultar campos se encuentran en la parte superior derecha.

Para regresar al lienzo, haz clic en **Volver al lienzo** en la parte superior.

## Límites de widget de datos estructurados

Cada tablero de Miro tiene un límite máximo de 250 widgets de datos estructurados, lo que incluye el conteo total combinado de tablas, cronogramas y tarjetas sincronizadas. Cada tabla está limitada a 1,000 filas y 50 columnas. Cuando alcanzas el límite de filas, verás un mensaje que evita que se agreguen más filas.

Para un rendimiento óptimo, recomendamos mantener las tablas con menos de 200 filas cuando se utilizan muchas columnas, ya que operaciones como agrupar, ordenar y filtrar pueden ralentizarse a partir de este punto. Estos límites ayudan a asegurar un rendimiento y fiabilidad óptimos para tus tableros de Miro.

### ¿Qué ocurre cuando alcanzas el límite de widgets de datos?

Cuando un tablero alcanza o excede el límite de 250 widgets de datos estructurados, puedes experimentar:

- Un mensaje de error al intentar añadir más widgets de datos estructurados.
- Carga inconsistente de los widgets de datos existentes.
- Problemas potenciales al guardar cambios.
- Ralentizaciones en el rendimiento.

### Consejos para gestionar los límites de widgets de datos

Si estás alcanzando o ya has superado el límite de widgets de datos estructurados, intenta:

**Distribuir widgets en varios tableros:**

- Agrupar contenido relacionado en tableros separados.
- Usar nombres de tableros significativos para facilitar la navegación.
- Crear un tablero "maestro" con enlaces a todos los tableros relacionados.

**Consolidar datos similares:**

- Combinar tablas con estructuras similares.
- Usar filtros en lugar de crear tablas separadas para diferentes vistas.
