---
title: Importar tableros de Lucidspark a Miro
article_id: 9549014537490
translation_id: 9549014537490
locale: es
sidebar_position: 7
created_at: '2023-01-12T09:05:07Z'
updated_at: '2026-01-19T14:30:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personas: Cualquier usuario con acceso de edición a los tableros de Lucidspark
    y Miro Planes: Free, Starter, Business, Education y Enterprise Plataformas: Navegador,
    Escritorio'
---

Migra tu contenido de Lucidspark sin problemas a Miro para disfrutar de una experiencia de colaboración más sólida. Esta guía describe cómo importar tus tableros y qué esperar durante el proceso.

> **Advertencia:** La edición del contenido importado es unidireccional. Los cambios realizados en Miro no se sincronizarán con Lucidspark.

> **Nota:** Se pueden migrar tableros de Lucidspark con licencias Free o Limitadas.

## Cómo importar tableros de Lucidspark mediante exportación en PDF

Sigue estos pasos para importar tus tableros de Lucidspark a Miro utilizando el método de exportación en PDF:

1. Asegúrate de exportar el contenido de **Lucidspark** que deseas importar a Miro como un PDF.
2. En el panel de Miro **Home**, haz clic en **+ Crear nuevo**.
3. Selecciona **Importar** y luego **Importar desde Lucidspark**.
   Se abrirá el modal **Importar desde Lucidspark**. Puedes importar varios archivos PDF de Lucidspark al mismo tiempo.
4. Sigue las instrucciones en pantalla proporcionadas en el modal.
5. Selecciona **Importar tableros**.
6. Revisa el contenido importado y haz los ajustes necesarios. Si bien Lucidspark y Miro tienen funcionalidades similares, puede haber diferencias en las opciones de estilo y formato. Consulta [Cómo aparecen los objetos de Lucidspark en Miro (Método de Importación Masiva por PDF)](#lucidspark-object-mapping-bulk-import) para obtener orientación sobre cómo se traducen los objetos.

## Método alternativo: Copiar y pegar contenido

Como una alternativa más rápida para pequeños volúmenes de contenido, puedes copiar directamente elementos de un tablero de Lucidspark abierto y pegarlos en un tablero de Miro.

> **Nota:** Cualquier usuario con acceso de edición a los tableros de Lucidspark y de Miro puede copiar contenido de Lucidspark y pegarlo en Miro. Para obtener detalles sobre cómo se mapean los objetos con este método, consulta [Cómo aparecen los objetos de Lucidspark en Miro (Método de Copiar/Pegar)](#lucidspark-object-mapping-copy-paste).

## Cómo aparecen los objetos de Lucidspark en Miro (Método de Copiar/Pegar)

Esta tabla ofrece una comparación exhaustiva de cómo se mapean los objetos cuando se copia contenido directamente desde Lucidspark y se pega en Miro.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Tarjetas de Azure | Las tarjetas de Azure se migran como tarjetas de Miro: 1. Configura la integración de Azure en Miro. 2. Convierte las tarjetas de Miro en [tarjetas de Azure](../../integrations-apps/microsoft/03-azure-cards.md). |
| Colaboradores y compartición | 🟠 Se pueden recrear manualmente |
| Comentarios | 🟠 Se pueden recrear manualmente |
| Conectores y divisores | Conectores |
| Contenedores | Formas |
| Documentos de archivos y URL | 🟠 Se puede recrear manualmente |
| URL de documentos (PDF) | Documentos insertados |
| Dibujar | Imágenes |
| Tablas dinámicas | Tablas |
| Emojis | Imágenes |
| Marcos | Marcos |
| GIF de la barra de herramientas | Imágenes |
| GIF a partir de archivos | Imágenes |
| GIF desde URL | GIF |
| Imágenes | Imágenes |
| Tarjetas de Jira | Las tarjetas de Jira se migran como tarjetas de Miro:  1. Configura la integración de Jira en Miro 2. Convierte las tarjetas de Miro a [tarjetas de Jira](../../integrations-apps/atlassian/03-jira-cards.md). |
| Tarjetas Lucid | Tarjetas |
| Mapa mental | Mapa mental |
| Formas | Formas |
| Nota adhesiva | Notas adhesivas |
| Tablas | Tablas |
| Texto | Texto |
| Cronograma | 🟠 Se puede recrear manualmente |
| Videos y otros URLs | Previsualizaciones |

## Cómo aparecen los objetos Lucidspark en Miro (Método de importación masiva de PDF)

Esta tabla proporciona una comparación exhaustiva de los objetos entre Lucidspark y Miro tras la importación masiva de tu contenido vía PDF.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Tarjetas Azure | Imágenes |
| Colaboradores y uso compartido | 🟠 Se puede recrear manualmente |
| Comentarios | 🟠 Se puede recrear manualmente |
| Conectores y divisores | Conectores |
| Contenedores | Formas |
| Documentos | 🟠 Se puede recrear manualmente |
| Dibujar | Líneas |
| Tablas dinámicas | Formas y Conectores |
| Emojis | Imágenes |
| Marcos | Marcos y Formas |
| GIFs | Imágenes |
| Imágenes | Imágenes |
| Tarjetas de Jira | Formas |
| Tarjetas de Lucid | Formas |
| Mapa mental | Formas y Conectores |
| Formas | Formas |
| Nota adhesiva | Notas adhesivas |
| Tablas | Tablas/Formas y Conectores |
| Texto | Texto |
| Cronograma | Formas y conectores |
| Videos y otros URLs | 🟠 Pueden ser recreados manualmente |

## Limitaciones de la importación

Aunque Lucidspark y Miro ofrecen funcionalidades similares, ten en cuenta las siguientes diferencias y limitaciones al importar contenido:

- Los cuadros de texto de Miro pueden contener hasta 6,000 caracteres, incluidos los espacios. Cualquier texto adicional se recortará.
- Los colores y estilos se asignan a las coincidencias más aproximadas en Miro.
- Los valores de opacidad de Lucidspark no se extraen con precisión durante la importación.
- Las notas adhesivas de Miro no admiten rotación, ajustes de la paleta de colores ni viñetas de texto que se puedan haber aplicado en Lucidspark.

## Obteniendo ayuda

> **Nota:** Para más preguntas y soporte sobre la migración de Lucidspark, contacta al [equipo de Soporte de Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) o comunícate directamente con tu gerente de Customer Success de Miro.
