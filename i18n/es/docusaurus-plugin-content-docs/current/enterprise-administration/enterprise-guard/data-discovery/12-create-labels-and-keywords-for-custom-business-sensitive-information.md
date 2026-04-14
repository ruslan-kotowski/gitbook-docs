---
title: "Crear etiquetas y palabras clave para informaci\xF3n sensible de la empresa"
article_id: 21626517022610
translation_id: 21626517022610
locale: es
sidebar_position: 11
created_at: '2024-09-26T21:36:45Z'
updated_at: '2026-03-04T22:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Crea etiquetas para definir condiciones, como palabras clave o widgets, que desees identificar y localizar en los tableros de Miro. Puedes crear hasta 100 etiquetas personalizadas para información sensible de la empresa. Para crear una etiqueta, realiza los siguientes pasos:

:::note
Para crear etiquetas personalizadas, debes tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.
:::

1. Ve a tus [ajustes de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, bajo **Enterprise Guard,** haz clic en **Descubrimiento de datos**.
3. En la página de **Descubrimiento de datos**, haz clic en la pestaña **Configuración**.
4. En la sección de **Datos sensibles de la empresa**, haz clic en el botón **Crear**.
5. En la página de **Definir etiqueta personalizada**, agrega los detalles de la etiqueta.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | **Nombre de la etiqueta** | **Longitud máxima:** 80 caracteres  Nombre descriptivo para la etiqueta personalizada. Puedes usar un nombre de proyecto interno de la empresa, ya que esta etiqueta no aparece en los registros.  **Nota:** El nombre de la etiqueta no es visible en los registros de auditoría. Si deseas buscar/ver los registros de auditoría asociados con esta etiqueta, puedes usar el ID de la etiqueta. |
   | **Nombre corto** | **Longitud máxima:** 10 caracteres alfanuméricos  Versión corta del nombre de la etiqueta. El nombre corto se usa para referirse a esta etiqueta personalizada en el descubrimiento de datos, el explorador de contenido y la clasificación de datos. **Nota:** El nombre corto no es visible en los registros de auditoría. Si deseas ver/buscar registros de auditoría asociados con esta etiqueta, puedes usar el ID de la etiqueta. |
   | **Descripción** | **Longitud máxima:** 500 caracteres  Descripción de la información que esta etiqueta está detectando. Esta información es útil para otros admins. |
   | **Condiciones** | Agrega palabras clave y tipos de widgets que quieras detectar y a los que se añadirá esta etiqueta al momento de la detección en un tablero de Miro. Debes añadir al menos una condición.  Si solo agregas palabras clave y no seleccionas ninguna casilla de widget, el descubrimiento de datos detecta todos los tableros que contienen coincidencias exactas de las palabras clave que proporcionaste para todos los widgets compatibles. La versión actual admite los siguientes elementos de tablero para la detección de palabras clave: Sticky, Tarjeta, Tarjeta de Jira, Bloque de código, Comentarios, Marco, Tabla, Conector/línea, Forma, Bloque de texto, Tablero Kanban, Mapa de historia del usuario.  También puedes elegir detectar solo bloques de código, tarjetas de Jira, tarjetas de Azure o pantallas de prototipado, sin agregar palabras clave. El descubrimiento de datos entonces detecta todos los tableros que contienen esos widgets.  Si agregas tanto palabras clave como widgets como condiciones, se deben cumplir ambos criterios, de palabra clave y widget, para que el descubrimiento de datos detecte el tablero. Esto te permite refinar tu búsqueda y apuntar a tableros de manera más precisa usando etiquetas personalizadas.  **Ejemplos:**  - Si deseas restringir la detección de tableros para identificar específicamente los tableros relacionados con el desarrollo de productos, pero no los relacionados con marketing, y el tablero debe contener el nombre del proyecto *Enterprise* *Guard*, y además quieres encontrar solo los tableros que también contengan una tarjeta de Jira (ya que está relacionada con el desarrollo de productos), debes configurar esta etiqueta para que contenga la palabra clave *Enterprise* *Guard* y seleccionar la casilla de verificación de la tarjeta de Jira. El descubrimiento de datos encuentra entonces los tableros que contienen la palabra clave Enterprise Guard y una tarjeta de Jira. El descubrimiento de datos también encuentra tableros que contienen tarjetas de Jira con la palabra clave Enterprise Guard en su título o descripción. Si un tablero contiene solo la palabra clave *Enterprise* *Guard* pero no contiene una tarjeta de Jira, el tablero no se detecta ya que no cumple con ambas condiciones especificadas.  - Si deseas detectar todos los tableros que contengan la palabra *Enterprise* *Guard* para todos los tipos de widgets admitidos, sin importar los tipos de widgets que el tablero contenga, en la sección **Añadir palabras clave**, agrega la palabra clave **Enterprise** **Guard**. No necesitas agregar ningún tipo de widget para este ejemplo.  - Si deseas detectar todos los tableros con tarjetas de Jira sin importar el contenido específico, en la sección **Añadir tipo de widget**, selecciona la casilla de **tarjeta de Jira**. No necesitas agregar ninguna palabra clave para este ejemplo.    **Para añadir una palabra clave:**  1. Haz clic en **Añadir palabras clave**.  2. Ingresa o pega palabras clave separadas por comas. **Notas:**  - Las palabras clave admiten caracteres alfanuméricos y Unicode. - Puedes añadir hasta 100 palabras clave o frases. - Los espacios al inicio y al final son ignorados en las palabras clave. - El descubrimiento de datos detecta coincidencias exactas de las palabras clave que proporciones, sin importar la sensibilidad a mayúsculas y minúsculas. - Si añades un espacio antes de una palabra clave, el descubrimiento de datos también encuentra coincidencias exactas que tienen un espacio antes de la palabra clave. - La versión actual admite los siguientes elementos del tablero para la detección de palabras clave: Nota adhesiva, Tarjeta, Tarjeta de Jira, Bloque de código, Marco, Tabla, Conector/línea, Forma, Bloque de texto, Tablero Kanban, Mapa de historia del usuario. Las notas y los comentarios actualmente no están incluidos en los escaneos de descubrimiento de datos. Estamos trabajando para incluir notas y comentarios en futuros lanzamientos de mejoras de funciones.  **Ejemplo:** Para identificar y etiquetar tableros que contengan las palabras clave *confidencial* o *interno*, añade las siguientes palabras clave: *confidencial, interno* (utiliza una coma para separar cada palabra clave). El descubrimiento de datos encuentra entonces todos los tableros que incluyan cualquiera de estas palabras clave.  **Para agregar un tipo de widget:**  1. Haz clic en **Agregar tipo de widget**.  2. Selecciona la casilla de verificación para el tipo de widget que deseas detectar en los tableros de Miro.  **Ejemplo:** Si deseas detectar y etiquetar tableros que contengan una tarjeta de Jira, selecciona la casilla de verificación **tarjeta de Jira**. |
6. Haz clic en **Siguiente**.
7. Revisa los detalles de la etiqueta personalizada.

   Si quieres editar los detalles de la etiqueta personalizada, haz clic en el botón **Anterior**.

   Si los detalles de la etiqueta personalizada son correctos, haz clic en el botón **Crear etiqueta personalizada**.

   Una vez que creas la etiqueta, el primer escaneo comienza automáticamente. Los resultados que coinciden con las condiciones seleccionadas estarán disponibles después de unos minutos u horas, dependiendo del número de tableros de Miro en tu organización.
