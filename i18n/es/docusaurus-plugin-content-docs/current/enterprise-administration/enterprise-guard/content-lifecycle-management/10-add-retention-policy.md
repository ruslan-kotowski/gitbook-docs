---
title: "A\xF1adir pol\xEDtica de retenci\xF3n"
article_id: 19205113739282
translation_id: 19205113739282
locale: es
sidebar_position: 10
created_at: '2024-05-28T18:00:55Z'
updated_at: '2025-12-08T16:05:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Para añadir políticas de retención, debes tener el [rol de admin de gobernanza de datos](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de gobernanza de datos, ponte en contacto con el admin de empresa.
:::

Para añadir una política de retención, realiza los siguientes pasos:

1. Ve a tus [ajustes de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, bajo **Enterprise Guard,** haz clic en **Ciclo de vida del contenido**.
3. Haz clic en la pestaña **Retención**.
   Aparecerá la página de **Políticas de retención**.
4. Haz clic en **Agregar política de retención**.
   Aparecerá la página **Definir criterios**.
5. Añade o selecciona la información adecuada para cada campo. La tabla siguiente enumera cada campo y su descripción.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | **Nombre**  **(requerido)** | Nombre de la política de retención.  Longitud máxima: 60 caracteres. |
   | **Descripción**  **(opcional)** | Descripción de esta política de retención.  Longitud máxima: 300 caracteres. |
   | **Período de retención**  **(obligatorio)** | Evita que los tableros sean eliminados de forma permanente por un período específico basado en uno de los siguientes criterios: **Último acceso**, **Última modificación** o **Creado en**. Selecciona un número, elige **Meses** o **Años**, y luego elige desde qué evento se calcula el período de retención.  Si especificas el período de retención en meses, debes seleccionar un período de retención entre 1 y 120 meses.  Si especificas el período de retención en años, debes seleccionar un período de retención entre 1 y 10 años. |
   | **Alcance**  **(obligatorio)** | Selecciona el alcance de esta política de retención. El alcance indica los tableros a los que se aplica esta política de retención. Puedes establecer el alcance de una política de retención para todos los tableros de una organización o para determinados niveles de clasificación de tableros.  **Configurar la política de retención para todos los tableros de la organización** Si deseas establecer el alcance de la política de retención para todos los tableros de la organización, en la lista **Alcance**, selecciona **Todos los tableros en la organización**.  **Configurar la política de retención para uno o más equipos en la organización** Si deseas establecer el alcance de la política de retención para uno o más equipos en la organización, realiza los siguientes pasos:  1. En la lista de **Ámbito**, selecciona **Equipo**. 2. Haz clic en el cuadro Intro de equipo y selecciona cada equipo al que deseas aplicar la política de retención. Aparecerá una marca de verificación junto al equipo que seleccionaste para asociar con la política de retención.   ✏️ - Puedes seleccionar varios equipos para una política de retención. Sin embargo, cualquier equipo solo puede asociarse con una política de retención a la vez.  - Puedes seleccionar cualquier equipo, incluidos los equipos eliminados, como un ámbito al configurar la política de retención.   - Un equipo que se seleccione como el ámbito de una política de retención no puede eliminarse permanentemente hasta que se elimine ese equipo del ámbito.  **Configurar la política de retención para un nivel de clasificación de tablero**  ✏️ Para establecer el alcance de la política de retención en un nivel específico de clasificación de tableros, debes asegurarte de que la función de Clasificación de Datos esté activada. Una vez que una política de retención utiliza un nivel de clasificación de tableros, no puedes desactivar la función de Clasificación de Datos. Para más información, consulta la documentación sobre [Clasificación de Datos](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Si deseas establecer el alcance de la política de retención para un nivel de clasificación específico del tablero, realiza los siguientes pasos:  1. En la lista de **Alcance**, selecciona **Clasificación**. 2. Haz clic en la lista situada junto a la lista de **Clasificación** y, a continuación, selecciona los niveles de clasificación a los que deseas aplicar la política de retención. También puedes buscar los niveles de Clasificación y seleccionarlos.  Aparece una marca de verificación junto a los niveles de clasificación que seleccionaste para asociarlos a la política de retención.  ✏️ **Notas:** - Puedes seleccionar varios niveles de clasificación a la vez. - No puedes establecer el mismo nivel de clasificación para distintas políticas de retención. Si un nivel de clasificación específico ya está asociado a una política de retención, el nivel de clasificación aparecerá en gris.  - Una vez que una política de retención utiliza un nivel de clasificación de tableros, no puedes desactivar la función de Clasificación de Datos.  -Una vez que un nivel de clasificación está asociado a una política de retención, no puedes eliminar ese nivel de clasificación específico. - Cuando un tablero está gobernado por una política de retención tanto de todos los tableros en el ámbito de la organización como de ámbito de clasificación, la política con el período de retención más largo es la que se aplica. |
6. Haz clic en **Siguiente**.
   La **página de revisión del impacto** aparece.
7. Revisa el impacto de la política de retención. La página de revisar impacto proporciona la siguiente información:
   - **Resumen:** configuración de la política de retención, como el nombre de la política, el periodo de retención y el alcance.
   - **Impacto de la política:** número de tableros que se regirán por esta política. La política de retención también es aplicable a los tableros en la papelera y se incluyen en el cálculo del impacto de la revisión.

   > ✏️ Cuando un tablero está gobernado tanto por una política de retención basada en tiempo como por una basada en clasificación, se aplica la política con el periodo de retención más largo.
8. Para guardar la configuración y aplicar la política de retención, haz clic en **Publicar**.

:::note
La creación, actualización o eliminación de una política activa el proceso de políticas de retención, que puede tardar hasta 24 horas en completarse. Sin embargo, la actualización del nombre o la descripción de una política se produce inmediatamente, ya que estas acciones no activan el proceso de las políticas de retención.
:::

#
