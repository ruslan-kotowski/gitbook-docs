---
title: Editar una etiqueta personalizada
article_id: 21690361870354
translation_id: 21690361870354
locale: es
sidebar_position: 18
created_at: '2024-09-30T13:43:27Z'
updated_at: '2026-03-04T23:02:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

:::note
Recomendamos editar las etiquetas solo antes de asociarlas con un nivel de clasificación.
:::

Edita las etiquetas para actualizar condiciones, como palabras clave o widgets, que quieras identificar y localizar en los tableros de Miro. Para editar una etiqueta, realiza los siguientes pasos:

:::note
Para editar etiquetas personalizadas, debes tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.
:::

1. Ve a tu [configuración de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, bajo **Enterprise Guard,** haz clic en **Descubrimiento de datos**.
3. En la página **Vista general** del **descubrimiento de datos**, haz clic en los tres puntos en la fila de la etiqueta que deseas editar y luego haz clic en **Editar etiqueta**.
4. En la página de **Editar etiqueta personalizada**, edita los detalles de la etiqueta.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | **Nombre de la etiqueta** | **Longitud máxima:** 80 caracteres  Nombre descriptivo para la etiqueta personalizada. Puedes usar un nombre de proyecto interno de la empresa ya que esta etiqueta no aparece en los registros.  **Nota:** El nombre de la etiqueta no es visible en los registros de auditoría. Si quieres buscar/ver registros de auditoría asociados con esta etiqueta, puedes usar el ID de la etiqueta. |
   | **Nombre corto** | **Longitud máxima:** 10 caracteres alfanuméricos  Versión corta del nombre de la etiqueta. El nombre corto se utiliza para referirse a esta etiqueta personalizada en el descubrimiento de datos y el explorador de contenido. **Nota:** El nombre corto no es visible en los registros de auditoría. Si deseas buscar o ver los registros de auditoría asociados con esta etiqueta, puedes usar el ID de la etiqueta. |
   | **Descripción** | **Longitud máxima:** 500 caracteres  Descripción de la información que esta etiqueta está detectando. Esta información es útil para otros admins. |
   | **Condiciones** | Agrega palabras clave y tipos de widgets que quieras detectar y a los que quieras añadir esta etiqueta al ser detectados en un tablero de Miro. Debes agregar al menos una condición.  Si solo agregas palabras clave y no seleccionas ningún checkbox de widgets, el descubrimiento de datos detecta todos los tableros que contienen coincidencias exactas de las palabras clave que proporcionaste para todos los widgets compatibles. La versión actual admite los siguientes elementos de tablero para la detección de palabras clave: nota adhesiva, tarjeta, tarjeta de Jira, bloque de código, comentarios, marco, tabla, conector/línea, forma, bloque de texto, tablero Kanban, mapa de historia del usuario.  También puedes seleccionar detectar solo bloques de código, tarjetas de Jira, tarjetas de Azure o pantallas de prototipos, sin agregar palabras clave. El descubrimiento de datos entonces detecta todos los tableros que contienen esos widgets.  Si añades tanto palabras clave como widgets como condiciones, se deben cumplir tanto el criterio de palabra clave como el de widget para que el descubrimiento de datos detecte el tablero. Esto te permite refinar tu búsqueda y dirigir los tableros con más precisión usando etiquetas personalizadas.  **Ejemplos:**  - Si deseas restringir la detección de tableros para identificar específicamente tableros relacionados con el desarrollo de productos, pero no relacionados con el marketing, y el tablero debe contener el nombre del proyecto *Enterprise* *Guard*, y quieres encontrar solo los tableros que también contienen una tarjeta de Jira (ya que está relacionado con el desarrollo de productos), configurarás esta etiqueta para que contenga la palabra clave *Enterprise* *Guard* y seleccionarás la casilla de tarjeta de Jira. El descubrimiento de datos encontrará entonces tableros que contengan la palabra clave Enterprise Guard y una tarjeta de Jira. El descubrimiento de datos también encontrará tableros que contengan tarjetas de Jira con la palabra clave Enterprise Guard en su título o descripción. Si un tablero solamente contiene la palabra clave *Enterprise* *Guard* pero no contiene una tarjeta de Jira, el tablero no es detectado ya que no cumple con ambas condiciones especificadas.  - Si deseas detectar todos los tableros con la palabra *Enterprise* *Guard* en ellos para todos los tipos de widgets admitidos, independientemente de los tipos de widgets que contenga el tablero, en la sección **Agregar palabras clave**, añade la palabra clave **Enterprise** **Guard**. No necesitas agregar ningún tipo de widget para este ejemplo.  - Si deseas detectar todos los tableros con tarjetas de Jira, independientemente de cualquier contenido específico, en la sección **Agregar tipo de widget**, selecciona la casilla de **tarjeta de Jira**. No necesitas agregar ninguna palabra clave para este ejemplo.    **Para agregar una palabra clave:**  1. Haz clic en **Agregar palabras clave**.  2. Ingresa o pega palabras clave separadas por comas. **Notas:**  - Las palabras clave admiten caracteres alfanuméricos y Unicode.  - Puedes agregar hasta 100 palabras clave o frases. - El descubrimiento de datos detecta coincidencias exactas para las palabras clave que proporcionas, sin importar la sensibilidad de mayúsculas o minúsculas. - La versión actual soporta los siguientes elementos de tablero para la detección de palabras clave: notas adhesivas, tarjeta, tarjeta de Jira, bloque de código, marco, tabla, conector/línea, forma, bloque de texto, tablero Kanban, mapa de historia del usuario. Notas y comentarios actualmente no están incluidos en los escaneos de descubrimiento de datos. Estamos trabajando para incluir notas y comentarios en lanzamientos futuros de mejoras de funciones.  **Ejemplo:** Para identificar y etiquetar tableros que contengan las palabras clave *confidencial* o *interno*, agrega las siguientes palabras clave: *confidencial, interno* (usa una coma para separar cada palabra clave). El descubrimiento de datos luego encuentra todos los tableros que incluyen cualquiera de estas palabras clave.  **Para agregar un tipo de widget:**  1. Haz clic en **Añadir tipo de widget**.  2. Selecciona la casilla para el tipo de widget que quieres detectar en los tableros de Miro.  **Ejemplo:** Si quieres detectar y etiquetar tableros que contengan una tarjeta de Jira, selecciona la casilla de **tarjeta de Jira**. |
5. Haz clic en **Siguiente**.
6. Revisa los detalles de la etiqueta personalizada.

   Si deseas actualizar los detalles de la etiqueta personalizada, haz clic en el botón **Anterior**.

   Si los detalles de la etiqueta personalizada son correctos, haz clic en el botón **Actualizar etiqueta personalizada**.

   Después de actualizar la etiqueta personalizada, el escaneo comienza automáticamente. Los resultados que coincidan con las condiciones seleccionadas estarán disponibles después de unos minutos u horas, dependiendo del número de tableros de Miro en tu organización.
