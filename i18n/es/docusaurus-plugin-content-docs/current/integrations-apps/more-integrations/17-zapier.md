---
title: Zapier
article_id: 360025942994
translation_id: 360025942994
locale: es
sidebar_position: 18
created_at: '2019-07-04T17:26:16Z'
updated_at: '2025-02-26T12:10:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Conecta tus aplicaciones favoritas a Miro vía Zapier, ampliando la lista de posibilidades de automatización de tus tareas diarias. Mueve información entre tus aplicaciones y tableros automáticamente para que puedas concentrarte en el trabajo más сrucial.

> **Disponible en:** planes Free, Starter, Business y Enterprise

## Cómo crear un Zap con Miro

Para conectar Miro a otras aplicaciones vía Zapier, necesitas tener una cuenta de Zapier.

Para crear un Zap, haz clic en el botón correspondiente en el [panel de Zapier](https://zapier.com/app/dashboard).

Crear_Zap.jpg
Botón Create Zap (Crear Zap)

Zapier crea un flujo de trabajo automatizado entre aplicaciones con **Triggers** (Disparadores) y **Actions** (Acciones).

:::warning
Ahora Miro solo puede funcionar como una **Acción** en Zapier.
:::

**Disparador**

Un disparador es un evento en una aplicación que inicia el Zap. Una vez configurado un Zap, Zapier monitoreará la aplicación para ese evento. Para el ejemplo "Save new events in Google Calendar to Miro card widgets" (Guardar nuevos eventos en el calendario de Google en los widgets de tarjeta de Miro), el Zap solo se activa cuando se crea un nuevo evento en el calendario de Google.

disparador_evento_nuevo.jpg
Configurar un evento Disparador en Zap

**Acción**

Una acción es un evento que completa el Zap. En el ejemplo anterior "Save new events in Google Calendar to Miro card widgets" (Guardar nuevos eventos en el calendario de Google en los widgets de tarjeta de Miro), las nuevas tarjetas de Miro se comportarán como una Acción.

:::warning
Ahora Miro funciona solo como una Acción en Zapier.
:::

Busca a Miro y elige una de las tres Acciones que hay: Copiar tablero, Crear tablero, Crear widget de tarjeta.

crear_un_Zap_con_Miro_como_una_acción.gif
Crear tu propio Zap con Miro como una Acción

### Acción de copiar tablero

Es una acción diseñada para crear una copia de un tablero en particular. Tendrás que seleccionar un equipo donde se creará la copia del tablero.

instalar_Zapier.jpg
Selección de un equipo de Miro

En el siguiente paso, elige los siguientes parámetros:

- Tablero original: elige un tablero del equipo para copiar. Puedes buscar el tablero por su nombre o ID *(*por ej. *o9J_rxLXasqA).* Si no puedes encontrar un tablero en la lista, vuelve a cargar los datos y comprueba una vez más.
- Título: ingresa un nombre de título para la copia del tablero. Si dejas el campo en blanco, el tablero se creará con el nombre **Untitled** (Sin título).
- Descripción: ingresa el texto para la descripción del tablero.
- Acceso del equipo: puedes elegir entre los tipos de acceso al tablero del equipo **Private** (Privado), **View** (Ver), **Comment** (Comentar) y **Edit** (Editar)
- Acceder vía enlace: crea reglas para compartir este tablero con un enlace. Puedes configurar grupos de acceso **Private** (Privado), **View** (Ver) y **Comment** (Comentar)

configurar_acción.jpg
/em> Configurar el evento de acción Copiar tablero /font>

### Acción Crear tablero

Esta acción creará un tablero con un título, una descripción y ajustes de acceso específicos.

- Título: ingresa un nombre de título para el tablero nuevo. Si dejas el campo en blanco, el tablero se creará con el nombre **Untitled** (Sin título).
- Descripción: ingresa el texto para la descripción del tablero.
- Acceso de equipo: puedes elegir entre los tipos de acceso para tu equipo **Private (Privado)**, **View (Ver)**, **Comment (Comentar)** y **Edit (Editar)**.
- Acceso vía enlace: crea reglas para compartir este tablero con un enlace. Puedes configurar el acceso **Private** (Privado), **View** (Ver) o **Comment** (Comentar) a través de un enlace público.

acción_crear_tablero.jpg
Configurar el evento de acción Crear tablero

### Acción Crear widget de tarjeta

Esta acción te permite transferir información (mensajes de Slack, por ejemplo) como un widget de [tarjeta](../../using-miro/essential-tools/02-cards.md) directamente dentro de un [marco](../../using-miro/essential-tools/07-frames.md) específico en un tablero de Miro con reglas personalizadas.

- Tablero: elige un tablero del equipo que quieras usar. Puedes buscar el tablero por su nombre o ID *(*por ej. *o9J_rxLXasqA).* Si no puedes encontrar un tablero en la lista, vuelve a cargar los datos y comprueba una vez más.
- Marco: selecciona un marco del tablero que hayas elegido. Puedes buscar el marco por su nombre y, si no puedes encontrarlo allí, intenta volver a cargar los datos y comprueba una vez más.
- Título de tarjeta: ingresa un título para tu tarjeta.
- Enlace de título de tarjeta: aquí puedes insertar un enlace desde la aplicación conectada (por ejemplo, puedes crear una tarjeta con un enlace a una tarea recientemente creada en Asana)
- Descripción de tarjeta: crea una descripción para tu tarjeta
- Fecha de vencimiento de tarjeta: establece una fecha de vencimiento para la tarjeta
- Color de borde de tarjeta: elige un color personalizado para los bordes de tu tarjeta (por ejemplo, **#ff0000** en este campo establecerá el color de la tarjeta en rojo).

acción_crear_tarjeta.jpg
Configuración del evento de acción Crear tarjeta

## Deshabilitar la integración de Zapier

Para eliminar la integración de Zapier de tu equipo de Miro, abre [Team settings](../../administration/get-started-as-a-miro-admin/06-manage-starter-and-education-plan.md) (Ajustes del equipo)**> Apps & Integrations (Aplicaciones e integraciones) > Zapier**y haz clic en **Uninstall** (Desinstalar)*.*

desinstalar_Zapier.jpg
Opciones para desinstalar Zapier

## Preguntas frecuentes

1. *¿Necesito tener una cuenta Zapier de empresa para utilizarlo con Miro?*
   - No, no es necesario. La integración con Miro se puede hacer con cualquier plan de Zapier.
2. *¿Dónde se almacenan mis datos de Zapier?*
   - Esta es una integración oficial mantenida por Miro y todas las prácticas de almacenamiento de datos en Miro se aplican aquí también.
3. *¿Necesito ser el admin de equipo en Miro para establecer la integración de Zapier?*
   - Depende de la configuración de admins en Miro y en Zapier. De manera predeterminada, hasta los miembros de un equipo que no son admins pueden configurar la integración.
4. *¿Las tarjetas (Trello, Asana, etc.) se sincronizan con las tarjetas importadas en los tableros de Miro?*
   - No, Zapier actualmente no proporciona sincronización. Por ejemplo, si mueves tu tarjeta Trello de "doing" (haciendo) a "done" (hecho), no se refleja del lado de Miro.
5. *No puedo vincular Gmail a Miro vía Zapier.*  ¿Por qué?
   - Comprueba tu correo electrónico. Actualmente, los usuarios con una cuenta de Gmail que termina en *@gmail.com* o *@googlemail.com* no pueden vincular Gmail a Miro, ya que Zapier puede enviar información de Gmail a una cantidad limitada de aplicaciones.
