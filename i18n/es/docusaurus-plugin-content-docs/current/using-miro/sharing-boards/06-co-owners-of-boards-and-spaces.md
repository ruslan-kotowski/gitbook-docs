---
title: Copropietarios de tableros y espacios
article_id: 360021580759
translation_id: 360021580759
locale: es
sidebar_position: 6
created_at: '2021-05-12T07:36:28Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  notes: 'Quién puede hacerlo: Propietarios de tableros, copropietarios de tableros,
    propietarios de espacios, copropietarios de espacios, administradores del equipo,
    administradores de la empresa. ¿Cuáles son los planes?: Business y Enterprise
    ¿Cuáles plataformas?: Navegador, escritorio, móvil'
---

La función de Copropietario mejora la colaboración al permitir a los propietarios del tablero delegar responsabilidades para preparar y facilitar el trabajo en un tablero, ya sea para sesiones en vivo o asincrónicas.

Un copropietario asegura un flujo de trabajo sin inconvenientes incluso si el propietario principal del tablero no está disponible, ya que los copropietarios pueden realizar casi todas las acciones a nivel de propietario, desde administrar los ajustes del tablero hasta controlar la visibilidad del contenido. Un copropietario ayuda a distribuir la carga de trabajo y proporciona un respaldo confiable para la gestión de tableros.

Para saber qué permisos tiene un copropietario de un tablero o Espacio, consulta la referencia de copropietarios.

## Habilitar el rol de copropietario para la organización

Como administrador de la empresa, sigue estos pasos:

1. Desde el panel de Miro, haz clic en tu avatar en la esquina superior derecha y haz clic en **Admin Console**.
2. Ve a **Seguridad** > **Compartir** > **Roles y permisos**.
3. Cambia **Permitir el rol de copropietario** a la posición de activado.

Ahora los administradores pueden habilitar el rol de copropietario para sus equipos.

## Habilitar la función de copropietario para un equipo

Como admin de empresa o admin de equipo, sigue estos pasos:

1. Desde tu panel de Miro, haz clic en tu avatar en la esquina superior derecha y haz clic en **Admin Console** | **Configuración**.
2. Ve a **Equipos** > **\{team name\}** > **Ajustes**.
3. En los **ajustes de colaboración**, activa la opción **Habilitar rol de copropietario en tableros y espacios**.

## Agregar copropietarios a los tableros

Como propietario de un tablero, o copropietario existente, sigue estos pasos:

1. Desde tu panel de Miro, realiza una de las siguientes acciones:
   1. Para un tablero, haz clic en los tres puntos (**...**) y selecciona **Compartir**.
   2. Abre un tablero, luego haz clic en **Compartir** en la esquina superior derecha.
2. Ingresa la dirección de correo electrónico de los usuarios que quieres agregar como copropietarios.
3. Para sus derechos de acceso, haz clic en **Es copropietario**.
4. (Opcional) Agrega un mensaje personalizado.
5. Haz clic en **Enviar invitaciones**.

:::note
Solo puedes asignar el rol de copropietario a los miembros del equipo. Para agregar un copropietario de fuera del equipo, primero invítalo a unirse al equipo.
:::

## Agregar copropietarios a los Espacios

Como propietario de un Espacio, o copropietario existente, sigue estos pasos:

1. Desde tu panel de Miro, realiza una de las siguientes acciones:
   1. Para un Espacio en la barra lateral, haz clic en los tres puntos (**...**) y haz clic en **Compartir**.
   2. Abre un Espacio, luego haz clic en la etiqueta en la parte superior que muestra el número de miembros.
2. Haz clic en **Administrar acceso**.
3. Para un miembro de Space, actualiza sus derechos de acceso a **Copropietario.**

> Puedes asignar el rol de copropietario solo a los miembros del Espacio. Para añadir a un copropietario desde fuera del Espacio, primero invítalos a unirse al Espacio.

> Un copropietario del Espacio tiene permisos de Editor para todo el contenido dentro de ese Espacio.

## Referencia de copropietarios

### Permisos de copropietario del tablero

Además de todos los permisos de Editor, un copropietario de un tablero tiene los siguientes permisos:

- **Administrar los ajustes de contenido del tablero y los ajustes de herramientas de colaboración**
  Controla quién puede copiar contenido del tablero y administra herramientas como el temporizador, la votación, el videochat, el uso compartido de pantalla y el manejo de atención.
- **Ocultar y mostrar marcos**
  Controla la visibilidad del contenido del marco durante presentaciones o talleres.
- **Agregar el bloqueo protegido**
  Evita mover o eliminar contenido accidentalmente durante la colaboración.
- **Agregar contraseña al tablero**
  Protege los tableros públicos requiriendo una contraseña para el acceso.
- **Descargar copia de seguridad del tablero**
  Crear copias archivadas de tableros. Los copropietarios también pueden restaurar tableros desde los backups.
- **Agregar copropietarios**
  Concede el estado de copropietario a otros usuarios.
- **Cambiar los detalles del tablero**
  Modificar la portada y renombrar el tablero
- **Compartir el tablero**
  Modificar los derechos de acceso para el equipo y otros usuarios en el tablero
- **Configurar permisos avanzados para compartir tableros**
  Especifica si el tablero puede compartirse fuera del equipo u organización

:::note
En los planes Enterprise, los copropietarios de tableros y los administradores de contenido pueden mover tableros usando la [API REST de Miro](https://developers.miro.com/reference/update-board), lo cual difiere intencionalmente de la experiencia de la interfaz de usuario de Miro, donde solo los propietarios pueden mover sus tableros.
:::

Un copropietario del tablero no puede realizar las siguientes operaciones:

- Eliminar el tablero
- Mover el tablero a otro equipo
- Cambiar el propietario del tablero

### Permisos de copropietario del espacio

Además de todos los permisos de Editor, un copropietario de Espacio tiene los siguientes permisos:

- Cambiar el nombre del espacio
- Compartir el espacio
- Modificar los derechos de acceso para el equipo y otros usuarios en el Espacio
- Agregar copropietarios al Espacio

Un copropietario de un Espacio no puede realizar las siguientes operaciones:

- Eliminar el espacio
- Cambiar el propietario del espacio

## Preguntas frecuentes

**No tengo la opción para asignar a un copropietario. ¿Por qué?**

La función de copropietario está disponible en los planes Business y Enterprise. El admin de la empresa debe activar esta función en los ajustes del equipo o de la empresa. Solo los miembros existentes del equipo pueden ser ascendidos a copropietarios. Asegúrate de que el usuario haya sido invitado al tablero por correo electrónico antes de intentar asignar el rol de copropietario.

**Soy un administrador con los permisos de administrador de contenido habilitados. ¿Por qué no puedo añadir copropietarios al tablero?**

Los admins con permisos de admin de contenido (CAP) necesitan primero agregarse como propietarios al tablero específico. Una vez que se convierten en propietarios del tablero, pueden asignar copropietarios.

**¿Debería pagar adicionalmente por los copropietarios invitados a mis tableros?**

Solo los miembros existentes del equipo pueden ser designados como copropietarios. Si el usuario que quieres convertir en copropietario no es ya parte de tu equipo, primero tendrás que invitarlo al equipo, lo que puede implicar comprar un asiento adicional, dependiendo de tu plan y del número de usuarios actuales. Después de que sean miembros del equipo, puedes asignarles el rol de copropietario.
