---
title: Miro para Jira Cloud
article_id: 360017572414
translation_id: 7618477230610
locale: es
sidebar_position: 4
created_at: '2022-09-13T18:17:40Z'
updated_at: '2024-10-08T15:14:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Visualiza cualquier cosa junto con tu equipo; ocúpate de los trabajos pendientes del producto con notas adhesivas digitales, crea diagramas de flujo y otros tipos de diagramas, además de wireframes. Adjunta tableros a incidencias de Jira y colabora con tu equipo en tiempo real como en una reunión en pizarra.

> **Disponible en:** Planes Starter, Business y Enterprise
> Sólo Jira Cloud

:::note
También puedes insertar tableros de Miro con la característica Atlassian Smart Link.
:::

:::note
Ten en cuenta que Miro tiene dos tipos de integraciones con Jira: **Miro para Jira Cloud** (que permite insertar tableros de Miro en el lado de Jira) y **tarjetas de Jira**. Para obtener más información sobre las Tarjetas Jira, visita este artículo.
:::

## Cómo instalar

El proceso de instalación es estándar para todos los complementos de Jira. En primer lugar, inicia sesión en tu Jira con derechos administrativos y, a continuación, descarga el complemento [aquí](https://marketplace.atlassian.com/apps/1215456/miro-for-jira-cloud?tab=overview&hosting=cloud) (la app también se puede encontrar en **Atlassian Marketplace** > **Find new apps** > **Miro for Jira Cloud**): haz clic en **Get app**y **Get it now**.
¡Y eso es todo! La instalación está terminada.

Miro_para_Jira.jpg
Notificación de Jira sobre la instalación exitosa

Por favor ten en cuenta que, como administrador, no necesitas asignar usuarios de Miro a usuarios de Jira durante la configuración. Cada usuario deberá darse autorización a sí mismo en Miro dentro de Jira.

## Cómo usar el complemento

### Cómo adjuntar tableros a incidencias de Jira

Para adjuntar un tablero a una incidencia de Jira, abre la incidencia en Jira. Haz clic en **Añadir tablero** en la sección **Tableros de Miro**.
añadir_tableros_Miro_en_Jira.jpg
*El botón del complemento aparece después de la instalación*

> Si no tienes una sección de tableros de Miro, búscala en el menú de contexto de la incidencia.

sección_de_tableros_en_Miro.jpg
Cómo añadir la sección de tableros de Miro a una incidencia de Jira

Verás un seleccionador con tableros de Miro. Elige el tablero que quieras añadir (puedes cambiar entre tus equipos y el seleccionador). Si no estás autorizado en Miro, primero deberás iniciar sesión.

Establece los ajustes para compartir el tablero en el menú desplegable. Puedes permitir a los usuarios ver y comentar el tablero de modo que los que no tengan un perfil en Miro puedan acceder a él.

:::note
Para los usuarios del [plan Enterprise](https://help.miro.com/hc/articles/360017571534) de Miro, tu configuración de acceso respetará los controles de acceso de toda la organización, lo que podría implicar que algunas opciones para compartir estén restringidas.  Más información: Cómo administrar la política de uso compartido de Enterprise respecto de las integraciones insertadas./span>
:::

insertar_un_tablero_en_Jira.jpg
Ajustes para compartir al adjuntar un tablero a una incidencia de Jira

Ten en cuenta que solo puedes insertar tableros sobre los cuales tienes acceso de edición.

Tu tablero ahora está adjunto a la incidencia de Jira seleccionada:

tablero_de_Miro_en_Jira.jpg
Tablero de Miro adjunto a una incidencia de Jira

### Cómo crear tableros nuevos a partir de Jira

Para crear un tablero nuevo a partir de una incidencia de Jira, haz clic en **Add board (Añadir tablero)** y crea un **tablero nuevo** desde el seleccionador.

crear_un_tablero_nuevo_desde_el_seleccionador.jpg
Cómo crear un tablero desde el seleccionador

### Cómo ver, comentar y editar tableros

Sencillamente, haz clic en un tablero adjunto para verlo, comentarlo o editarlo, según los derechos de acceso correspondientes. La ventana del tablero se abrirá como una superposición que te permitirá trabajar y colaborar como si estuvieras en Miro.

Insertar_Miro_en_Jira.jpg
Superposición del tablero en Jira

 También puedes hacer clic en el botón de origen para abrir el tablero en Miro en una pestaña nueva por comodidad.

botón_origen.jpg
El botón para ir a la aplicación de Miro

### Cómo desvincular tableros

Para desvincular un tablero, basta hacer clic en el icono de la cruz y el tablero adjunto se eliminará de la incidencia al instante (en el lado de Miro, el tablero quedará intacto).

eliminar_un_tablero_adjunto.jpg
La opción para eliminar el tablero adjunto

## Cómo desactivar el complemento

Para deshabilitar la integración, abre **Atlassian Marketplace** > **Manage apps** (Administrar aplicaciones) > abre la página del complemento y haz clic en **Uninstall** (Desinstalar):

desinstalar_complemento_Jira.jpg
**La opción para desinstalar en la sección de complementos de Jira**

## Atlassian Smart Link para Miro

Puedes insertar tableros de Miro en incidencias de Jira gracias a la característica Atlassian Smart Link. La característica te permite insertar un tablero de forma automática sin tener que instalar un plugin.

:::note
Ten presente que solo los usuarios con acceso al tablero insertado en Miro podrán trabajar con la vista previa después de conectar sus cuentas de Miro y Atlassian. Si quieres que la vista previa esté disponible para todos los usuarios de Jira, puedes usar el complemento de Jira.
:::

Ve a la incidencia de Jira y copia un enlace al tablero o escribe el enlace para intentarlo.  Si usas la función por primera vez, se te pedirá que conectes tu equipo de Miro. Haz clic en Conectar la vista previa, **autoriza a Miro y elige un equipo desde el cual insertarás tus tableros.**

instalar_enlaces_de_Atllassian.jpg
Elegir un equipo desde el cual insertar los tableros

Cuando pegues el enlace de un tablero de Miro en una incidencia de Jira, se convertirá en un widget de Jira de forma automática. Haz clic en el enlace y verás las opciones para mostrarlo como tarjeta o un elemento insertado.

mostrar_como_enlace.gif
Las opciones para mostrar el enlace de un tablero de Miro como enlace, tarjeta o elemento insertado

Si eliges mostrar el tablero como elemento insertado, puedes cambiar su tamaño si arrastras sus lados.

cambiar_tamaño_insertado_en_Jira.gif
Cómo cambiar el tamaño de la inserción de Miro en Jira

:::warning
Si las cookies de terceros están bloqueadas en tu navegador, puede haber problemas inesperados cuando se muestran los tableros insertados.
:::

## Preguntas frecuentes

¿Puedo ocultar la sección de tableros de Miro en las incidencias de Jira?

Sí, haz clic en los tres puntos de la esquina superior derecha de la sección y elige **Ocultar tableros de Miro**.
esconder_tableros_de_Miro.jpg
*Ocultar tableros de Miro en Jira*

¿El complemento funciona en los proyectos Next-gen de Jira?

Sí, puedes adjuntar tus tableros a dichos proyectos.

¿El complemento de Jira tiene un costo adicional?

Miro para Jira Cloud está disponible para todos los planes de pago sin coste adicional (planes Starter, Business y Enterprise).

Migraremos Jira de una instancia de nube a otra. ¿Los tableros de Miro insertados en las incidencias de Jira se verán afectados?

No debería haber problemas con los tableros de Miro insertados si el contenido se mueve sin cambios.
