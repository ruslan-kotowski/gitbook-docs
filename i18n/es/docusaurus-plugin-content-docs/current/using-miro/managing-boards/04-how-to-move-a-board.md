---
title: "C\xF3mo mover un tablero"
article_id: 360017730093
translation_id: 4420488181010
locale: es
sidebar_position: 4
created_at: '2022-02-15T04:42:04Z'
updated_at: '2026-03-27T16:07:20Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  roles: board_owner
  notes: 'Relevant for: All plans'
backstage_link:
  entity_kind: capability
  entity_id: move-board-to-space
---

> **Quién puede hacerlo:** Propietarios de tableros
> **Relevante para:** Todos los planes

Todos los usuarios de Miro pueden ser miembros de varios equipos. Tu perfil de Miro es tu correo electrónico. Puedes mover un tablero de Miro de un equipo a otro o transferir tu tablero de Miro a otro perfil.

:::note
En los planes Enterprise, los copropietarios de tableros y los administradores de contenido pueden mover tableros usando la [API REST de Miro](https://developers.miro.com/reference/update-board), lo cual difiere intencionalmente de la experiencia de la interfaz de Miro, donde solo los propietarios pueden mover sus tableros.
:::

:::note
Los admins de empresa del plan Enterprise pueden [restringir la opción de mover tableros hacia y desde un equipo](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) para todos los usuarios no administradores y propietarios de tableros.
:::

## Escenarios comunes

Aquí hay varios escenarios comunes que involucran mover tableros, junto con la sección de este artículo que explica cómo hacerlo:

- Tienes **dos perfiles de Miro** (direcciones de correo electrónico asociadas con Miro) y quieres mover los tableros de un perfil a otro.
  *Sigue los pasos de* [*esta sección*](04-how-to-move-a-board.md)*, usando la pestaña del **plan Free**.*
- Pasaste de un **plan Free a un plan de pago** y quieres mover los tableros al plan de pago.
  *Sigue los pasos de* [*esta sección*](04-how-to-move-a-board.md)*, usando la pestaña del **plan Free**.*
- Quieres **mover tableros entre dos equipos de pago**.
  *Sigue los pasos en* [*esta sección*](04-how-to-move-a-board.md)*, usando la pestaña **Planes de pago y Education**.*

## Mover tableros entre equipos

:::warning
Cuando mueves un tablero a otro equipo, su [historial de versiones](12-board-history-versions.md) se perderá. Si deseas conservar el historial de versiones, te recomendamos [copiar el contenido del tablero](../working-on-the-board/09-copy-as-text-or-as-an-image.md) en su lugar.
:::

Para mover un tablero entre equipos, debes:

- ser propietario del tablero
- ser miembro de ambos equipos

Hay dos maneras de mover un tablero a un equipo diferente: desde el panel o directamente desde dentro de un tablero.

### Cómo mover un tablero directamente desde dentro del tablero

1. Abre tu tablero y haz clic en el ícono de tres puntos (**...**) a la derecha del nombre del tablero (esquina superior izquierda)
2. Ve a **Tablero > Mover a > Otro equipo![moving-board-three-dots.png](../../../../../../docs/using-miro/managing-boards/images/21537437708306_moving-board-three-dots.png)**

### Cómo mover un tablero usando el panel

1. Ve a tu panel para ver todos los tableros en un equipo.
2. Pasa el mouse sobre la tarjeta del tablero que quieres mover.
3. Haz clic en los tres puntos, luego haz clic en **Mover al equipo**.
   Se abrirá un cuadro de diálogo.
4. Selecciona la organización a la que quieres mover el tablero.
5. Selecciona un equipo dentro de esa organización.
6. Haz clic en **Mover**.

### Cómo mover un tablero a otro espacio

1. Abre tu tablero y haz clic en el ícono de tres puntos (**...**) directamente a la derecha del nombre de tu tablero (esquina superior izquierda)
2. Navega a **Tablero > Mover a > Otro espacio.** Además, puedes elegir notificar a los miembros del equipo que el tablero ha sido movido a otro espacio.![moving-boards-spaces.png](../../../../../../docs/using-miro/managing-boards/images/21537453797394_moving-boards-spaces.png)*Mover un tablero a otro espacio*

### Acceso denegado por el usuario

Si cualquier colaborador del tablero no forma parte del equipo al que se está trasladando el tablero, verás un mensaje de acceso denegado.

Hay dos maneras de ver cuáles son los correos electrónicos de los usuarios que perderán el acceso al tablero después de que lo muevas. Si la cantidad de usuarios es menor a diez, podrás ver la lista de correos electrónicos haciendo clic en **Ver correos electrónicos de los usuarios** en el **Mensaje de acceso denegado.** Si el número es mayor que diez, habrá un enlace para descargar la lista de correos electrónicos.

Para asegurarte de que todos los colaboradores mantengan acceso al tablero, puedes [invitar a los miembros al nuevo equipo](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) antes de mover el tablero.

También puedes elegir **Move anyway (Mover de todas formas)** y añadir colaboradores al tablero nuevamente después de que lo hayas trasladado.

![warning when moving a board.png](../../../../../../docs/using-miro/managing-boards/images/16759524012690_warning%20when%20moving%20a%20board.png)
*Mensaje de acceso denegado al mover un tablero de un equipo a otro*

**Si mueves un tablero a un equipo Free**, se compartirá con todos los miembros del equipo.

![private boards are not available in free teams.png](../../../../../../docs/using-miro/managing-boards/images/16759539790738_private%20boards%20are%20not%20available%20in%20free%20teams.png)
*Los tableros privados no están disponibles en equipos Free*

## Mover tableros entre perfiles

Tu perfil en Miro es la dirección de correo electrónico con la que te registraste. Si te registraste con dos correos electrónicos diferentes, significa que tienes dos perfiles. Puedes transferir un tablero de un perfil a otro.

### Cómo mover tableros entre perfiles

Planes de pago, Education Plan Free

Si el tablero está ubicado en un equipo de pago o Education y quieres moverlo a otro equipo de pago o Education, solo guarda una copia de seguridad del tablero y cárgala a ese equipo.

1. Abre tu panel.
2. Pasa el mouse sobre la tarjeta del tablero que quieres mover.
3. Haz clic en los tres puntos.
4. Haz clic en **Descargar copia de seguridad del tablero**.
5. El archivo .rtb se guardará en tu dispositivo.

   ![board-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136352530_board-backup.png)
6. Inicia sesión en tu segundo perfil de Miro.
7. Cambia al equipo al que quieres mover el tablero.
8. Haz clic en **+ Crear nuevo** > **Importar** > **Importar copia de seguridad**.
9. Se abrirá el seleccionador de archivos.
10. Elige el archivo de copia de seguridad .rtb que hayas guardado anteriormente y haz clic en **Abrir**. El tablero estará disponible desde tu panel.

    ![board-import-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136353682_board-import-backup.png)

Sigue estos pasos si tu tablero está ubicado en un equipo gratuito o si necesitas mover un tablero a un equipo gratuito.

1. Inicia sesión en Miro bajo el perfil n.º 1.
2. Comparte el tablero con el perfil n.º 2. Haz clic en **Compartir**.
   ![free-sharing-board.png](../../../../../../docs/using-miro/managing-boards/images/23122136354066_free-sharing-board.png)
3. Ingresa el correo electrónico para el perfil n.º 2 > haz clic en **Enviar invitaciones**.

   ![free-sharing-board-dialog.png](../../../../../../docs/using-miro/managing-boards/images/23122136354706_free-sharing-board-dialog.png)
4. Transfiere la propiedad del tablero del perfil n.º 1 al perfil n.º 2. Haz clic en el botón **Compartir** > **Configuración de compartición** > elige perfil n.º 2 > selecciona **Propietario** en el menú desplegable.
5. Inicia sesión en Miro bajo el perfil n.° 2 donde verás el tablero.
6. Mover el tablero a otro equipo.

:::warning
Si tu segundo perfil está en un plan Free y lo invitas a un perfil de pago, estás usando una licencia en ese plan de pago. Si esto excede el número de licencias de tu plan, es posible que se te cobre por una licencia adicional.
:::

## Preguntas frecuentes

**¿Por qué no veo la opción de mover a un equipo en el menú de mi tablero?**

Solo los propietarios de tableros que son miembros de varios equipos pueden mover tableros entre ellos. Si no eres el propietario del tablero, puedes [duplicar el tablero](03-how-to-duplicate-a-board.md) (si esto es permitido en las [configuraciones de contenido del tablero](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)) y mover la copia del tablero.

La opción para mover tableros también puede estar restringida por los admins de empresa en el plan Enterprise.

**¿Cómo puedo transferir la propiedad de mi tablero a otro usuario?**

Aprende cómo [transferir la propiedad del tablero a otro colaborador](05-how-to-transfer-board-ownership.md).

**¿El enlace del tablero cambia cuando lo muevo a otro equipo?**

No, la URL del tablero no cambia.

**¿Puedo mover un tablero de plantilla al equipo de otro usuario?**

Sí, puedes pedirle al usuario que te invite a su equipo y luego mover el tablero, o [compartir el tablero](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) y permitirles [duplicar tu tablero](03-how-to-duplicate-a-board.md) en los [ajustes de contenido del tablero](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).

**¿Puedo mover Espacios entre equipos?**

No, solo puedes mover tableros separados.

**¿Puedo mover varios tableros de forma masiva?**

No, no admitimos esta función por el momento.

**Intento mover el tablero pero no sucede nada o aparece un mensaje de error - ¿Qué hago?**

Por favor, intenta mover el tablero en otro navegador o en el modo incógnito. También puedes intentar cambiar a otra red o dispositivo.

Otra opción es [duplicar el tablero](03-how-to-duplicate-a-board.md) y mover la copia del tablero. Si eso no ayuda, [informa del problema al Soporte de Miro](../tools/troubleshooting/06-contacting-miro-support.md).
