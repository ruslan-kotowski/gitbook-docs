---
title: "Clasificaci\xF3n de datos"
article_id: 4417739162258
translation_id: 4417739162258
locale: es
sidebar_position: 2
created_at: '2022-02-07T10:01:21Z'
updated_at: '2025-02-26T12:17:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

La clasificación de datos permite a los usuarios del plan Enterprise asignar etiquetas a sus tableros para especificar el nivel de sensibilidad del contenido del tablero.

> **Disponible para: plan Enterprise
> **Disponible en**: escritorio, tableta
> **Quién puede hacerlo:** admins de empresa**

Puedes encontrar la configuración de la clasificación de datos en la consola de admins de la empresa. Ve a **Configuración** y selecciona **Clasificación**.

:::note
Para los clientes con Enterprise Guard, puedes encontrar la **clasificación** en la consola de admin, en **Enterprise Guard**. Ve a **Configuración** > **Enterprise Guard** > Clasificación.
:::

Asegúrate de que comprendes los siguientes puntos clave sobre la clasificación de datos:

- La clasificación de datos es una etiqueta interna de y no tiene ningún impacto en la configuración para compartir tableros, lo que significa que los tableros pueden compartirse más allá de su clasificación.
- Los tableros que se crearon antes de que la función se habilitara se marcarán como no clasificados.
- [Duplicar un tablero](../../../using-miro/managing-boards/03-how-to-duplicate-a-board.md) copiará la etiqueta de clasificación de datos actual en la nueva copia del tablero.
- Las etiquetas no se muestran actualmente en el [modo de presentación](https://help.miro.com/hc/articles/360017731073), en el [modo de reuniones inteligentes](https://help.miro.com/hc/articles/4408834812690) ni en el móvil.

## Cómo configurar las etiquetas de clasificación

En **Configuración**, selecciona **Clasificación**. Para activar las etiquetas de clasificación de tu organización empresarial, selecciona **Configurar clasificación.**

## Cómo añadir nuevas etiquetas de clasificación

Los admins de empresa pueden crear y personalizar hasta 30 etiquetas de clasificación, y establecer una etiqueta por defecto para todos los tableros nuevos de la organización.

En Configuración de **la clasificación**, ya están creadas cuatro etiquetas, que puedes personalizar. También puedes crear nuevas etiquetas que se adapten a tus necesidades organizativas.

Para crear una nueva clasificación:

1. Selecciona **Editar niveles de clasificación**.
2. Haz clic en **Añadir nivel**.
3. **Establece el **Nivel** de clasificación, agrega un **Nombre**, una **Descripción** y cambia el color de la Insignia.**
4. **Si quieres agregar una referencia para los usuarios del tablero, agrega un enlace a los lineamientos.**
5. (Opcional) Selecciona **Vista previa** para ver cómo aparecerá tu etiqueta en producción.
6. Selecciona **Hecho.**
7. (Opcional) Para reordenar tus etiquetas de clasificación, haz clic en las flechas hacia arriba**(Ʌ)** o hacia abajo**(V**).
8. **Haz clic en Publicar para finalizar y guardar los cambios.**

:::note
Cuando creas o editas una etiqueta de clasificación, tus cambios se guardan como borrador y no se publican hasta que hagas clic en el botón **Publicar**. Esto significa que puedes salir de la configuración de la clasificación y volver a ella en cualquier momento.
:::

También puedes agregar un enlace a las directrices de clasificación de tu empresa en la que los colaboradores pueden recibir más información sobre las políticas de clasificación de datos existentes.

![](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921802487570_image.png)

*Enlace a las directrices de clasificación*

## Cómo personalizar los borradores de clasificación

Para editar una clasificación **sin** un borrador guardado:

1. Haz clic en el botón **Editar niveles de clasificación** .
2. Haz clic en el icono del lápiz **Editar**.
3. Haz los cambios y pulsa **Hecho**.
4. **Haz clic en Publicar para finalizar y guardar los cambios.**

Para editar una clasificación **con** un borrador guardado:

1. En el panel Clasificación de datos, haz clic en **Reanudar configuración**.
2. Haz clic en el icono del lápiz **Editar**.
3. Haz los cambios y pulsa **Hecho**.
4. **Haz clic en Publicar para finalizar y guardar los cambios.**

## Cómo eliminar una etiqueta de clasificación

Para eliminar una etiqueta, haz clic en el icono de la papelera. Ten en cuenta que no puedes eliminar la etiqueta predeterminada.

![datos_clasificacion_borrar_etiqueta.pngBorrar](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017013528978_data_classification_delete_label.png)
*una etiqueta*

### Agregar la etiqueta predeterminada en la empresa

Elige una etiqueta de clasificación por defecto para los tableros recién creados. A cada nuevo tablero que se crea en la organización Empresa se le asigna la etiqueta por defecto.

Para establecer una etiqueta predeterminada para tu organización, marca **Etiqueta de clasificación predeterminada** cuando añadas o edites una etiqueta de clasificación.

![Configurar la etiqueta por defecto de clasificación de datos](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921802487570_image.png)

Establecer la etiqueta de clasificación predeterminada

### Añadir la etiqueta predeterminada en el equipo

> **Configurado por: admins de empresa, admins de equipo**

Los admins de empresa y de equipo pueden habilitar la función **Anular la etiqueta predeterminada** y establecer una etiqueta predeterminada en el ámbito de equipo: cada nuevo tablero que se cree en el equipo recibirá esta nueva etiqueta predeterminada que anulará la etiqueta predeterminada establecida en la empresa.

Para habilitar esta configuración, navega a los Ajustes de equipo > **Permisos** y desliza hacia abajo.

Ten en cuenta que puedes establecer la función para anular la etiqueta del equipo solo si los ajustes de clasificación de datos están habilitados en la empresa.

Para [los equipos recién creados,](../../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md) este ajuste está deshabilitado si elijes los ajustes predeterminados cuando se crea un equipo.

### Añadir etiquetas de clasificación a los tableros

> **Establecido por:** propietarios del [tablero](../../../using-miro/sharing-boards/01-board-access-rights.md), [copropietarios del tablero](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md), editores que sean miembros del equipo, admins de empresa con [permisos de admins de contenido](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md)

Si la clasificación de datos está habilitada en tu Configuración de la empresa, los usuarios pueden ver y cambiar las etiquetas del tablero. La etiqueta de clasificación de datos aparece como una insignia junto al nombre del tablero. Cuando pases el mouse sobre la insignia, los colaboradores verán el nombre y la descripción de la etiqueta.

[El propietario del tablero,](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) [los copropietarios del tablero](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), los editores miembros del equipo y los admins de empresa con permisos de admins de contenido pueden actualizar la etiqueta de clasificación haciendo clic en la insignia de clasificación o desde los detalles del tablero. Selecciona una etiqueta y haz clic en Actualizar. Si el administrador de la empresa añadió un enlace a los lineamientos en los ajustes, el usuario puede seguir ese enlace en la ventana emergente para conocer más detalles.

![clasificacion_datos_añadir_etiquetas_a_tableros.gifCambiar](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017043043090_data_classification_adding_labels_to_boards.gif)
*la etiqueta de clasificación de datos en el tablero*

### Filtro de clasificación de datos en el panel

Los usuarios del plan Enterprise con clasificación de datos habilitada pueden filtrar sus tableros por etiquetas en el panel. **Cualquier clasificación** está seleccionada de forma predeterminada.

![filtro_clasificacion_datos.pngFiltro](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017043043986_data_classification_classification_filter.png)
*de clasificación en el panel de control*
