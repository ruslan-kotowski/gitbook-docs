---
title: Cómo permitir o limitar la copia y la exportación de tableros y contenido
article_id: 360018350399
translation_id: 360018350399
locale: es
sidebar_position: 14
created_at: '2020-12-14T06:10:03Z'
updated_at: '2026-01-22T14:23:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  notes: 'Quién puede hacerlo: Miembros del equipo, (Configuración) admins de equipo,
    (Configuración) admins de la empresa Qué planes: Starter, Business, Enterprise,
    Educación Qué plataformas: Navegador, Escritorio, Móvil'
---

Los admins de empresa y de equipo pueden especificar si los miembros del equipo y los que no pertenecen al equipo pueden copiar el contenido del tablero, y establecer la configuración de copia predeterminada para nuevos tableros.

Los propietarios y copropietarios de tableros pueden especificar la configuración de copia para otros miembros del equipo en un tablero dado. Si los admins permiten que los miembros externos al equipo copien tableros, incluidos visitantes e invitados, entonces los propietarios y copropietarios de tableros pueden permitir que lo hagan.

Si los admins no permiten que los miembros externos al equipo copien el contenido, se elimina la opción de tablero para permitir la copia del tablero por parte de miembros externos.

:::note
En los planes Free, la copia de tableros está habilitada por defecto y no puede modificarse.
:::

## Cómo configurar permisos de copia de tableros para un equipo

Para un equipo determinado, un admin de empresa o un admin de equipo puede especificar si los miembros ajenos al equipo pueden copiar y exportar tableros y contenido, y establecer los permisos de copia predeterminados para los tableros recién creados.

Sigue estos pasos:

1. Ve a **Admin Console**.
2. Haz clic en **Equipos**.
3. Haz clic en la fila para **\{Team name\}**.
   Se abrirá el panel de **\{Team name\}**.
4. Haz clic para abrir la pestaña **Configuración**.
5. Desplázate hasta **Seguridad de contenido**.
6. Para **Copiar contenido**, especifica si solo los miembros del equipo o cualquier persona en la organización puede copiar el contenido del tablero.
7. Especifica la **configuración predeterminada para copiar contenido**. Los propietarios de tableros pueden modificar esta configuración para tableros individuales.
   Tus configuraciones se guardan automáticamente.

:::note
Si no se permite copiar el contenido del tablero para personas ajenas al equipo, entonces la opción **Cualquier persona con acceso al tablero** se elimina de la configuración del tablero. Por ejemplo, los visitantes y los invitados tienen prohibido copiar contenido.
:::

:::note
No es posible copiar imágenes entre tableros privados conectados a diferentes equipos. Habla con tu admin de empresa de Miro para obtener permiso para acceder al otro tablero y copiar imágenes.
:::

## Cómo establecer permisos de copia para un tablero

Para un tablero concreto, un propietario o copropietario del tablero puede especificar quién puede copiar el tablero.

Sigue estos pasos:

1. En un tablero que poseas, compartas la propiedad o hayas creado, haz clic en la parte superior derecha en **Compartir**.
   Se abre el modal de compartir.
2. En la parte inferior derecha, haz clic en **Configuración de compartir**.
3. En **Quién puede copiar contenido del tablero**, selecciona una opción.

   > ✏️ Si tu admin de empresa o admin de equipo deshabilita la opción **Cualquiera con acceso al tablero**, entonces esta opción no estará disponible.
4. Haz clic en **Hecho**.
   Tus cambios se guardan automáticamente y se aplican a todas las personas con acceso al tablero.

## Opciones de copia del tablero según el tipo de usuario

Suponiendo que **cualquier persona con acceso al tablero** puede copiar contenido, la siguiente tabla muestra los permisos por tipo de usuario.

|  | Guardar tablero como plantilla | Copiar contenido del tablero | Exportar | Duplicar | Descargar archivos del tablero |
| --- | --- | --- | --- | --- | --- |
| Miembros del equipo | ✔ | ✔ | ✔ | ✔ | ✔ |
| Invitados | ✘ | ✔ | ✔ | ✔ | ✔ |
| Visitantes con cuenta de Miro | ✘ | ✔ | ✔ | ✔ | ✔ |
| Visitantes sin una cuenta de Miro | ✘ | (Con acceso de edición) ✔ | ✘ | ✘ | ✔ |

:::note
(Enterprise) Si [no está permitido mover tableros entre equipos](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md), entonces la opción para duplicar un tablero no está disponible.
:::

:::note
Ten en cuenta que algunas opciones no están disponibles para ciertas categorías de usuarios, incluso si el propietario del tablero permite que cualquier persona con el enlace copie el contenido del tablero.
:::

## Preguntas frecuentes

*¿Por qué no puedo copiar y pegar contenido en un tablero de Miro?*

Es posible que el propietario o copropietario del tablero no permita copiar para tu rol. Puedes ver tu rol en la barra de colaboración, en la esquina superior derecha de un tablero de Miro. Contacta al propietario o copropietario del tablero para solicitar permisos de copia para tu rol.

También querrás asegurarte de haber iniciado sesión en Miro. Si tu rol tiene permisos para copiar y has iniciado sesión, inicia sesión y abre el tablero en otro navegador e intenta copiar.

*¿Por qué no aparece la opción de **Cualquiera con acceso al tablero** disponible para mí?*

El admin de empresa o el admin de equipo han deshabilitado esta opción. Si eres un admin de empresa o de equipo, consulta Cómo establecer permisos de copia de tableros para un equipo.

*¿Cómo puedo permitir que los visitantes descarguen archivos mientras restringo su capacidad de copiar o duplicar el tablero?*

Crea un tablero separado solo con los archivos, luego habilita la opción de copiar el contenido del tablero para cualquiera con el enlace al tablero. Comparte el enlace del tablero con los visitantes.

Alternativamente, puedes insertar el nuevo tablero con los archivos, y habilitar la copia para cualquiera con el enlace, en el tablero original. Para más información sobre cómo insertar, [Inserta un tablero de Miro](../import-and-export/export/02-embed-a-miro-board.md).

*¿Por qué no puedo encontrar **Permisos** en el menú de **Compartir** del tablero?*

(De pago) Solo el propietario y el copropietario del tablero pueden especificar los permisos de contenido. (Free) Los permisos de contenido no se pueden modificar de su configuración predeterminada, que permite copiar para todos los usuarios.

*¿Puedo especificar quién puede cargar contenido en mi tablero?*

Cualquiera con derechos de **Puedes editar** puede cargar contenido en tu tablero.
