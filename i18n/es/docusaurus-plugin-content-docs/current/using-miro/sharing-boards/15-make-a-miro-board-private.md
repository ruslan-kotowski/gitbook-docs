---
title: Hacer que un tablero de Miro sea privado
article_id: 360021095159
translation_id: 360021095159
locale: es
sidebar_position: 15
created_at: '2021-04-15T11:55:31Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  notes: 'Quién puede hacerlo: Propietarios del tablero ¿Qué planes: Starter, Business,
    Enterprise y Education ¿Qué plataformas?: Navegador, escritorio, móvil'
---

Si vas a empezar un proyecto individual o quieres trabajar en un tablero antes de compartirlo con tu equipo, puedes crear un tablero de Miro privado o hacer privado un tablero compartido existente.

## Comprender los tableros privados

Los tableros privados son tableros que no se comparten con nadie y solo son accesibles por el propietario del tablero. Esta función está disponible en los planes Starter, Education, Business y Enterprise.

En el plan Free, todos los tableros creados dentro de un equipo son visibles para todos los miembros del equipo. Puedes ver quién está en tu equipo en [Configuración de equipo](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md) en la pestaña **Usuarios activos**. Si deseas un tablero privado en un plan Free, debes ser el único miembro de ese equipo.

## Administrar la privacidad del tablero

Puedes crear un nuevo tablero con acceso privado desde el principio o cambiar la configuración de un tablero existente para hacerlo privado.

### Crear un nuevo tablero privado

Para asegurarte de que un tablero nuevo sea privado desde el momento de su creación, sigue estos pasos.

1. **Para administradores: Establecer ajustes para compartir predeterminados (opcional).** Si eres admin de equipo o de empresa en un plan Starter, Business, Enterprise o Education, puedes configurar todos los nuevos tableros para que sean privados por defecto.
   1. Ve a **Configuración de equipo** > **Permisos** > **Configuración de uso compartido**.
   2. Bajo **Configuración predeterminada para el uso compartido de tableros**, elige **Solo el propietario del tablero puede acceder**.
      ![Configuración predeterminada para compartir en Miro.](images/22298483629074_default sharing settings.jpg)
      *Ajustes para compartir predeterminados*
2. **Verifica la ubicación del tablero.** Antes de crear tu tablero, asegúrate de estar en la sección **Tableros en este equipo** de tu panel. Si creas un tablero dentro de un [espacio](../spaces/01-spaces.md) compartido, el tablero se compartirá automáticamente con todos los miembros de ese espacio.
   > ✏️ Si tienes un espacio privado que no está compartido con nadie, puedes crear tu tablero allí con seguridad.
3. **Confirmar configuración de privacidad.** Después de crear tu tablero, abre el diálogo **Compartir**. Aquí puedes verificar si el tablero está [compartido con tu equipo](03-sharing-boards-and-inviting-collaborators.md). Si es así, establece el nivel de acceso del equipo a **Sin acceso**.
   ![Animación que muestra cómo eliminar el acceso del equipo a un tablero en Miro.](../../../../../../docs/using-miro/sharing-boards/images/21016134729874_7-1-720p-10fps-s4-r20.gif)
   *Cómo eliminar el acceso del equipo a un tablero*

### Haz un tablero compartido privado

Para hacer un tablero existente privado en un plan Starter, Business, Enterprise o Education, debes eliminar el acceso de todos los colaboradores. Abre el cuadro de diálogo **Compartir** y deja de compartir el tablero en todos los niveles:

- Configura el acceso del equipo a **Sin acceso**.
- (En Enterprise) Establecer acceso de la empresa a **Sin acceso**.
- Deshabilitar cualquier enlace público (establecer en **Sin acceso**).
- Si el tablero está en un espacio, sácalo o deja de compartir el espacio.
- Elimina todos los usuarios individuales que aparecen en **Configuración de uso compartido** hasta que solo tú (el propietario) permanezcas.

:::note
Si **no** eres el propietario del tablero pero necesitas hacer el tablero privado, debes [invitar a tu propio correo](03-sharing-boards-and-inviting-collaborators.md) al tablero antes de eliminar el acceso del equipo, espacio o empresa. Si fallas en hacer esto, perderás acceso al tablero tan pronto como cambies la configuración de uso compartido.
:::

![Animación que muestra cómo cambiar la configuración de un tablero compartido de Miro a privado.](../../../../../../docs/using-miro/sharing-boards/images/21016121409426_7-2-720p-10fps-s4-r20.gif)
*Configurar un tablero de Miro compartido como privado*

Siempre puedes [check quién tiene acceso a tu tablero](05-who-has-access-to-my-board.md) en la ventana **Compartir**.

## Preguntas frecuentes

¿Por qué se bloquearon mis tableros después de cambiarme al plan Free?

El plan Free no permite tableros privados. Comparte el tablero con tu equipo para desbloquearlo. Más información en este artículo: [El tablero está bloqueado](../tools/troubleshooting/15-the-board-is-locked.md).

He visto la opción de mejorar el plan para que mi tablero sea privado. ¿Mi tablero es público de forma predeterminada?

En el plan Free, se comparte con todo el equipo de forma predeterminada. Solo se refiere a que tus tableros son "compartidos con el equipo" dentro de tu equipo Free.

¿Se pueden encontrar en línea mis tableros públicos?

Miro se esfuerza por evitar que los tableros públicos sean indexados por motores de búsqueda como Google o Bing. Sin embargo, cualquiera que tenga el enlace puede acceder a estos tableros, y el enlace podría compartirse más allá de tu público objetivo. Dependiendo de tu plan de Miro, puedes mejorar la seguridad [estableciendo una contraseña](13-password-protection-for-public-boards.md) para tu tablero público.

Soy miembro de un equipo Free y de un equipo de pago. ¿Puedo mover mis tableros del equipo Free al equipo de pago para hacerlos privados?

Sí, puedes [mover tus tableros de Miro](../managing-boards/04-how-to-move-a-board.md).

¿Se puede duplicar mis tableros públicos?

Sí, si está permitido en tu [configuración de contenido del tablero](14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).

Cuando comparto mi tablero públicamente, ¿debo pagar por los usuarios que accederán al tablero mediante un enlace?

No, los visitantes podrán acceder al tablero de manera gratuita. Obtén información sobre cómo puedes [compartir tus tableros públicamente](08-collaboration-with-visitors.md).
