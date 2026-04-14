---
title: Insertar un tablero de Miro
article_id: 360016335640
translation_id: 360016335640
locale: es
sidebar_position: 2
created_at: '2020-09-09T07:54:13Z'
updated_at: '2025-09-19T09:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Personas: Editores del tablero Planes: Todos los planes Plataformas: Web,
    Escritorio, Móvil'
---

Puedes insertar cualquier tablero de Miro o un elemento específico (marco o formato) del tablero en aplicaciones y sitios web compatibles para que tus compañeros de equipo trabajen en contexto sin cambiar de herramientas.

Los elementos insertados heredan la [configuración para compartir](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) del tablero:

- **Enlace público activado** — cualquiera con el enlace puede ver (o, en planes de pago y Education, comentar o editar).
- **Enlace público desactivado** — solo los colaboradores invitados pueden abrir el elemento insertado después de iniciar sesión.

Los [administradores de Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md) pueden gestionar la disponibilidad del enlace público en la [configuración de seguridad](../../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Elige tu método de inserción

Miro ofrece dos maneras de insertar tableros:

- **Usando aplicaciones compatibles**:

  - Trabajando dentro de plataformas como Zoom, Teams, Confluence, Jira o Notion.
  - Buscas funciones de integración nativa y un flujo de trabajo sin interrupciones.
  - Los usuarios interactuarán principalmente a través de esa plataforma específica.
  - Necesitas el proceso de configuración más sencillo.
- **Usando código de inserción**:

  - Insertar en sitios web, blogs o plataformas personalizadas.
  - Trabajando con WordPress, Webflow u otros constructores web.
  - Necesitas más control sobre el tamaño y la apariencia.
  - La plataforma admite iFrames pero no tiene una integración nativa de Miro.

## Insertar un tablero en aplicaciones compatibles

Miro tiene una serie de aplicaciones compatibles en las que puedes compartir fácilmente tus tableros de Miro. Las aplicaciones compatibles incluyen:

- [Zoom](../../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md)
- [Webex](../../../integrations-apps/more-integrations/10-miro-for-webex.md)
- [Microsoft Teams](../../../integrations-apps/microsoft/microsoft-teams/02-miro-for-microsoft-teams-user-guide.md)
- [Jira](../../../integrations-apps/atlassian/02-miro-for-jira-cloud.md)
- [Confluence](../../../integrations-apps/atlassian/01-miro-for-confluence.md)
- [Notion](https://miro.com/marketplace/notion-embed/)
- [Coda](https://miro.com/marketplace/coda-embed/)
- [Productboard](https://miro.com/marketplace/productboard-embed/)
- Medios

Cuando insertas un tablero de Miro en otra aplicación, puedes establecer derechos de acceso específicamente para los usuarios de la aplicación y permitirles ver, comentar o editar el tablero desde dentro de la aplicación. El acceso al tablero desde Miro no se verá afectado. Aprende más sobre [cómo funcionan los permisos y el uso compartido en tableros insertados](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

Para insertar un tablero en una de las aplicaciones compatibles:

1. En la aplicación de destino, escribe **/miro** o elige **Miro** en el menú de inserción.
2. Selecciona el tablero.
3. Selecciona la **Vista inicial**:
   - **Tablero completo** — todo el lienzo.
   - **Elemento específico**, como un marco o formato (Doc, Diagrama, Tablas, Cronograma o Diapositivas).
4. Activa el **modo sin distracciones** para crear una inserción sin interrupciones. Déjalo desactivado para permitir la interacción completa.
5. Selecciona la **configuración de acceso** para todos los visitantes:
   - **Pueden ver** — cualquier persona que vea el elemento insertado puede ver el tablero.
   - **Requiere acceso** — cualquiera que vea el elemento insertado debe tener acceso para ver, comentar o editar el tablero.
6. Selecciona **Insertar tablero**.

La inserción respeta la configuración de compartición del tablero. En dispositivos móviles, todas las inserciones son solo de visualización.

## Inserta un tablero con código de inserción

Usa esta opción para cualquier plataforma que soporte iFrame, como **WordPress** o **Webflow**.

1. Abre el panel de **Compartir** usando uno de estos métodos:
   - En la esquina superior derecha, selecciona **Compartir** > **Insertar**, o
   - En el menú principal del tablero, selecciona **Tablero** > **Exportar** > **Insertar**, o
   - En el lienzo, selecciona el elemento que deseas insertar (marco o formato). Por ejemplo, un documento. Abre el menú contextual de tres puntos y selecciona **Insertar este documento**.
2. Selecciona la **Vista de inicio**:
   - **Tablero** — el lienzo completo.
   - **Elemento específico**, como marco o formato (Documento, Diagrama, Tabla, Cronograma o Diapositivas).
3. (Opcional) **Establecer área de inicio** — arrastra para delinear una región exacta del tablero.
4. Decide sobre la interacción:
   - Selecciona **Solo ver** para bloquear la visualización.
   - Desmarca **Solo ver** para permitir que los visualizadores desplacen, hagan zoom, comenten o editen (si tienen permiso).
5. Selecciona **Copiar código** y pégalo donde lo necesites.
   Si el destino solo acepta URLs, selecciona **Copiar enlace** en su lugar.

Puedes crear múltiples inserciones para el mismo tablero, cada una con su propia vista inicial, área de inicio u objeto de enfoque.

### Reproducción automática de diapositivas

Para reproducir automáticamente un insertado de Diapositivas, ajusta el **Intervalo de diapositivas automáticas** de 1 a 30 segundos en la pestaña de **Insertar**. La reproducción automática se ignora cuando insertas un tablero dentro de otro tablero.

## Cómo aparecen las inserciones

- El nombre del tablero no es clicable.
- El mini-mapa, [notas](../../essential-tools/17-visual-notes.md), y las ventanas emergentes están cerrados por defecto.
- Algunas opciones del menú, como **Establecer vista inicial**, están ocultas.
- Todos los insertados son solo de visualización en móviles.
- Los bloqueadores de cookies de terceros pueden evitar que los insertados se carguen correctamente.

## Preguntas frecuentes

**¿Cuál es la diferencia entre una vista inicial y el modo sin distracciones?**
 Una vista inicial establece la posición inicial, pero los visualizadores aún pueden explorar el tablero. El modo sin distracciones oculta todo excepto el objeto seleccionado y siempre es solo de visualización.

**¿Puedo hacer editable un insertado en modo sin distracciones?**
 No. Para habilitar la colaboración, desmarca **Solo ver** y otorga derechos de edición en la configuración para compartir del tablero.

**¿Qué widgets son compatibles?**
 Documentos, Diagramas, Tablas, Cronogramas, Diapositivas, y cualquier marco.

**¿Puedo eliminar el logotipo de Miro?**
No. La eliminación del logotipo no está disponible.

**¿Puedo insertar un tablero dentro de otro tablero?**
Sí. Copia el código de inserción y pégalo en el tablero de destino con **Pegar código iFrame**.
