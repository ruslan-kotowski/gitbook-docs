---
title: "Editar la pol\xEDtica de eliminaci\xF3n"
article_id: 19551033354002
translation_id: 19551033354002
locale: es
sidebar_position: 18
created_at: '2024-06-14T19:50:51Z'
updated_at: '2025-12-08T16:14:46Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Para editar políticas de eliminación, debes tener el [rol de admin de gobernanza de datos](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de gobernanza de datos, ponte en contacto con el admin de empresa.
:::

Para editar una política de eliminación, realiza los siguientes pasos:

1. Ve a tus [parámetros de configuración de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, bajo **Enterprise Guard**, haz clic en **Ciclo de vida del contenido**.
3. Haz clic en la pestaña de **Eliminación**.
   Aparece la página de **Políticas de eliminación**.
4. En la página de **Políticas de eliminación**, haz clic en la política de eliminación que quieras editar.
   Aparece la página que muestra la información relacionada con la política.
5. Haz clic en **Editar** en la parte superior derecha de la página y, a continuación, edita los campos requeridos. La tabla siguiente enumera cada campo y su descripción.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | **Nombre**  **(obligatorio)** | Nombre de la política de eliminación.  Longitud máxima: 60 caracteres. |
   | **Descripción**  **(opcional)** | Descripción de esta política de eliminación.  Longitud máxima: 300 caracteres. |
   | **Período de eliminación**  **(requerido)** | Especifica cuándo los tableros se mueven automáticamente a la papelera. Elige un número, selecciona **Meses** o **Años**, y luego elige si el período se calcula desde la **última modificación** del tablero o desde su **último acceso**.  Si especificas el periodo de eliminación en Meses, debes seleccionar un periodo de eliminación entre 1 y 120 meses.  Si especificas el periodo de eliminación en Años, debes seleccionar un periodo de eliminación entre 1 y 10 años.  Por ejemplo, si quieres que los tableros se muevan a la papelera cuando no se hayan modificado durante un año, puedes seleccionar 1 año y elegir **Última modificación**. |
   | **Alcance**  **(obligatorio)** | Selecciona el alcance para esta política de eliminación. El alcance indica los tableros a los que se aplica esta política de eliminación. Puedes establecer el alcance de una política de eliminación para todos los tableros de una organización o para determinados niveles de clasificación de tableros.  **Establecer la política de eliminación para todos los tableros de la organización** Si deseas establecer el alcance de la política de eliminación para todos los tableros de la organización, en la lista de **Alcance**, selecciona **Todos los tableros en la organización**.  **Configura la política de eliminación para uno o más equipos en la organización** Si deseas establecer el alcance de la política de eliminación para uno o más equipos en la organización, realiza los siguientes pasos:  1. En la lista de **Alcance**, selecciona **Equipo**. 2. Haz clic en el cuadro **Ingresar equipo** y selecciona cada equipo al que quieres aplicar la política de eliminación. Un símbolo de verificación aparece junto al equipo que seleccionaste para asociar con la política de eliminación.   ✏️ - Puedes seleccionar múltiples equipos para una política de eliminación. Sin embargo, cualquier equipo solo puede estar asociado con una política de eliminación a la vez.  - Puedes seleccionar cualquier equipo, incluyendo equipos eliminados, como un alcance al establecer la política de eliminación.   - Un equipo seleccionado como alcance para una política de eliminación no puede ser eliminado permanentemente hasta que se retire del alcance.  **Establecer la política de eliminación para un nivel de clasificación de tablero**  ✏️ Para establecer el alcance de la política de eliminación en un determinado nivel de clasificación de tableros, debes asegurarte de que la función Clasificación de Datos está activada. Una vez que una política de eliminación utiliza un nivel de clasificación de tableros, no puedes desactivar la función de Clasificación de Datos. Para más información, consulta la documentación sobre [Clasificación de Datos](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Si quieres establecer el alcance de la política de eliminación para un determinado nivel de clasificación de tableros, sigue estos pasos:  1. En la lista de **Alcance**, selecciona **Clasificación**. 2. Haz clic en la lista situada junto a la lista de **Clasificación** y luego selecciona los niveles de clasificación para los que deseas aplicar la política de eliminación. También puedes buscar los niveles de Clasificación y luego seleccionar los niveles de Clasificación.  Aparece una marca de verificación junto a los niveles de clasificación que seleccionaste para asociar a la política de eliminación.  ✏️ **Notas:** - Puedes seleccionar varios niveles de clasificación a la vez. - No puedes establecer el mismo nivel de clasificación para diferentes políticas de eliminación. Si un nivel de clasificación específico ya está asociado a una política de eliminación, el nivel de clasificación aparece en gris.  - Una vez que una política de eliminación utiliza un nivel de clasificación de tableros, no puedes desactivar la función de Clasificación de Datos.  -Una vez que se asocia un nivel de clasificación con una política de eliminación, no puedes eliminar ese nivel de clasificación específico. - Cuando un tablero está regido tanto por políticas de eliminación de alcance de todos los tableros en la organización como de alcance de clasificación, se aplica la política con el período de eliminación más largo. |
6. Haz clic en **Siguiente**.
   La **página de revisión de impacto** aparece.
7. Revisa el impacto de la política de eliminación. La página de revisar impacto proporciona la siguiente información:
   - **Resumen:** configuración de la política de eliminación, como el nombre de la política, el periodo de eliminación y el alcance.
   - **Impacto de la política:** número de tableros que se regirán por esta política.
8. Para guardar la configuración y aplicar la política de eliminación, haz clic en **Publicar**.
   Si no tienes habilitadas las notificaciones de eliminación, aparece el cuadro de diálogo de **Habilitar notificaciones de eliminación**.

**Notificaciones de eliminación** permiten a los usuarios recibir alertas anticipadas antes de que un tablero se mueva automáticamente a la papelera debido a inactividad. Estas alertas ayudan a los usuarios a tomar medidas si desean conservar su contenido.

Si deseas habilitar las notificaciones de eliminación:

a. Haz clic en **Notificar**.

b. Configura cuántos días antes se debe enviar la notificación — cualquier valor entre **1 y 30 días**.

Si habilitar las notificaciones resulta en **algunos tableros siendo movidos inmediatamente a la Papelera** (porque ya están por encima del umbral), se te preguntará si deseas notificar a los usuarios sobre esos tableros específicos. Puedes elegir:

- **Sí** – para notificar a los propietarios y copropietarios del tablero incluso si el tablero se está moviendo a la Papelera de inmediato.

- **No** – para mover los tableros sin enviar una notificación para esta acción inmediata.

Una vez habilitadas, los usuarios con tableros bajo el alcance de cualquier política de eliminación con notificaciones activadas:

- Recibirán una notificación en su Miro **feed de notificaciones** durante la ventana de inspección configurada.

- Podrán abrir el tablero directamente desde la notificación.

- Verán un **banner** en el tablero advirtiendo sobre el auto-borrado inminente, con una opción para **Mantener tablero** si desean conservarlo.

:::note
La creación, actualización o eliminación de una política activa el proceso de políticas de eliminación, que puede tardar hasta 24 horas en completarse. Sin embargo, la actualización del nombre o la descripción de una política se produce inmediatamente, ya que estas acciones no activan el proceso de políticas de eliminación.
:::

#
