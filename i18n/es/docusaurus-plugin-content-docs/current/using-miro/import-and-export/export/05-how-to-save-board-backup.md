---
title: Cómo guardar una copia de seguridad del tablero
article_id: 360017572774
translation_id: 360017572774
locale: es
sidebar_position: 5
created_at: '2019-02-11T10:14:51Z'
updated_at: '2025-12-02T10:14:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  notes: 'Quién puede hacerlo: Propietarios de tableros, copropietarios de tableros,
    admins de empresa con [permisos de admin de contenido](../../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)
    en el [plan Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md)
    Planes: Starter, Business, Enterprise, Education Plataformas: Navegador, Desktop'
---

Crea copias archivadas de tus tableros guardando copias de seguridad de los tableros. Las copias de seguridad te permiten garantizar la seguridad de tu contenido y compartir copias de tus tableros con otros usuarios de Miro.

## Guardar una copia de seguridad del tablero

Para crear una copia de seguridad:

1. Abre el tablero y haz clic en el ícono de **tres puntos verticales** (![icon-main.svg](../../../../../../../docs/using-miro/import-and-export/export/images/27743904151698_icon-main.svg)).
2. Selecciona el submenú **Tablero**.
3. Luego selecciona el submenú **Exportar**.
4. Elige la opción **Descargar copia de seguridad del tablero** y sigue las instrucciones en pantalla.

![backup-entry-point.png](../../../../../../../docs/using-miro/import-and-export/export/images/21537453245330_backup-entry-point.png)
*Descargando la copia de seguridad del tablero*

También puedes guardar una copia de seguridad desde tu panel. Abre el menú del tablero haciendo clic en el icono de **tres puntos** (**...**) y selecciona **Descargar copia de seguridad del tablero** de las opciones.

El archivo *.rtb* se guardará en tu dispositivo.

:::warning
Ten en cuenta que **solo los propietarios** y copropietarios pueden descargar copias de seguridad de tableros ubicados en equipos **de pago**. Si esta opción aparece desactivada en el menú de Exportación, por favor verifica si esta funcionalidad está [disponible en tu plan](../../../plans-billing/miro-plans/02-plans-and-features-available.md) y si eres el [propietario del tablero](../../sharing-boards/01-board-access-rights.md) o [copropietario del tablero](../../sharing-boards/06-co-owners-of-boards-and-spaces.md).
:::

## Restaurar un tablero desde una copia de seguridad

La opción de cargar una copia de seguridad de un tablero está disponible para cualquier usuario en equipos de pago. Puedes enviar una copia archivada de tu tablero a otro usuario de Miro para que pueda recrear la copia del tablero en su equipo de pago.

Para restaurar un tablero desde una copia de seguridad:

1. Desde el [panel](https://miro.com/app/dashboard/), haz click en **Crear Nuevo**.
2. Selecciona **Importar**.
3. Luego selecciona **Importar copia de seguridad**.
   Se abrirá un cuadro de diálogo.
4. Elige tu archivo de copia de seguridad del tablero **.rtb*.
5. Después de confirmar tu elección, se creará un tablero nuevo con el mismo contenido en el equipo. El título del tablero incluirá **Restaurado**.

Después de restaurar el tablero, también tienes la funcionalidad de mover el tablero a un espacio diferente dentro de tu equipo.

![backup-import.png](../../../../../../../docs/using-miro/import-and-export/export/images/21537453249938_backup-import.png)
*Restauración de un tablero desde una copia de seguridad*

## Resolución de problemas

Ten en cuenta que tanto las descargas como las cargas de copias de seguridad de tableros son limitadas. Para las descargas, hay un límite de **1 GB**. Si tu tablero es más grande que eso, necesitarás dividirlo en tableros más pequeños o confiar en las [versiones del tablero](../../managing-boards/12-board-history-versions.md) en lugar de las copias de seguridad descargadas del tablero.

En cuanto a las cargas, la interfaz de Miro puede subir copias de seguridad de tableros de un máximo de **1 GB**. Para cargar archivos de copia de seguridad más grandes, por favor contacta al equipo de Soporte de Miro:

1. Inicia sesión en Miro y envía tu solicitud [utilizando el formulario de asistencia](../../tools/troubleshooting/06-contacting-miro-support.md).
2. Adjunta tu archivo de copia de seguridad a tu solicitud o cárgalo a cualquier almacenamiento en la nube y envíanos el enlace a este (asegúrate de permitir que cualquier persona con el enlace pueda descargar el archivo).
3. Si tu archivo de copia de seguridad es de menos de 1 GB y de todos modos tienes problemas para cargarlo, consulta los pasos de resolución de problemas [en esta página](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

Si aparece el mensaje de error: **No se puede encontrar el duplicado del recurso existente para el recurso optimizado 0** cuando intentes cargar una copia de seguridad, significa que la copia de seguridad del tablero contiene un recurso que necesita ser eliminado. Puedes [enviar el archivo *rtb* al servicio de Soporte de Miro](../../tools/troubleshooting/06-contacting-miro-support.md) para que podamos eliminar los datos del recurso y asegurar la carga exitosa de la copia de seguridad.

:::note
Si tienes problemas para guardar una copia de seguridad, intenta con los pasos de solución indicados en [este artículo](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).
:::

## Preguntas frecuentes

**No tengo la opción de descargar la copia de seguridad del tablero. ¿Por qué?**

Ten en cuenta que solo los propietarios o copropietarios de tableros en equipos de pago o los admins de empresa con [permisos de admin de contenido](../../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md) en el [plan Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md) pueden guardar copias de seguridad de tableros.

**¿Qué hacer si mi tablero ha sido eliminado?**

Revisa esta guía: [Cómo restaurar un tablero eliminado](../../managing-boards/08-how-to-restore-a-deleted-board.md).

**¿Puedo hacer copias de seguridad de varios tableros de forma masiva?**

Esto no es posible actualmente. Tendrás que hacer la copia de seguridad de cada tablero individualmente.
