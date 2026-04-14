---
title: Importar diagramas de Visio a Miro
article_id: 11842818558738
translation_id: 11842818558738
locale: es
sidebar_position: 8
created_at: '2023-06-06T10:11:36Z'
updated_at: '2026-02-16T14:27:52Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personas: Todos los usuarios con planes elegibles Planes: Business, Enterprise
    Plataformas: Navegador, Escritorio, Móvil'
---

Transfiere fácilmente tus diagramas de MS Visio a Miro y comienza a colaborar en una herramienta unificada.

Los diagramas importados son completamente funcionales para que puedas editar, colorear, mover y rediseñar según necesites.

:::warning
La edición de diagramas importados es solo unidireccional. Los cambios hechos en Miro no se reflejarán en Visio.
:::

## Importar un solo diagrama de Visio a un nuevo tablero de Miro

Sigue estos pasos para importar un diagrama individual de Visio. El diagrama importado creará un nuevo tablero de Miro:

1. En Visio, abre el diagrama que deseas exportar.
2. Selecciona el menú **Archivo** y elige **Guardar como**. Selecciona una ubicación y guarda tu archivo en formato `.vsdx`.
3. Navega al tablero de Miro desde el cual deseas iniciar la importación. Este puede ser cualquier tablero, ya que la importación creará uno nuevo.
4. En la barra de herramientas de Creación a la izquierda, selecciona **Formas** > **Más formas**, y luego selecciona el icono **Importar diagrama** ubicado en la parte superior derecha del panel de biblioteca de formas de diagramas.
5. En el cuadro de diálogo que aparece, arrastra y suelta el archivo `.vsdx` de Visio, o haz clic en el botón **Elegir archivo** y navega para seleccionar el archivo desde tu sistema.
6. Selecciona **Importar**.
   Cuando finalice el proceso de importación, verás un diálogo de **Archivo importado**.
7. Haz clic en **Ir al tablero** para abrir el nuevo tablero de Miro que contiene tu diagrama importado.

## Importar diagramas de Visio de forma masiva

También puedes importar varios diagramas de Visio a Miro simultáneamente desde tu panel. Cada diagrama se importará a su propio nuevo tablero de Miro, con el nombre del archivo original:

1. Ve a tu [panel de Miro](https://miro.com/app/dashboard/).
2. Selecciona **+ Crear nuevo** > **Importar** > **Importar diagrama**.
3. Arrastra tus archivos `.vsdx` al área designada, o utiliza el enlace **elegir archivos** para seleccionar varios diagramas de Visio. Ten en cuenta que todavía puedes eliminar archivos antes de importarlos.
4. Seleccionar **Importar archivos**.
   Cuando el proceso de importación termine, verás un diálogo de **Archivos importados**.
5. Seleccionar **Hecho**.

Esto crea un nuevo tablero para cada diagrama, nombrado según el nombre de archivo original.

## Entender el mapeo de objetos de Visio en Miro

La siguiente tabla compara cómo se representan típicamente los objetos y formas de Visio una vez importados en Miro. Ten en cuenta que, aunque Miro busca una alta fidelidad, para elementos complejos podrían ser necesarios algunos ajustes o recreaciones manuales.

| **Visio** | **Miro** |
| --- | --- |
| Bloqueo | Texto, Formas |
| Contenedores | Formas |
| Documentos | 🟠 Se puede recrear manualmente |
| Clave del diagrama | Texto, Formas |
| Marcos | Marcos y formas |
| GIFs | Imágenes |
| Hotspot | Enlace a |
| Imágenes | Imágenes |
| Línea | Conectores |
| Organigramas | Formas, Imágenes |
| formas | Formas |
| Contenedores inteligentes | Formas |
| Tabla inteligente | Formas |
| Nota adhesiva | Notas adhesivas |
| tablas | Formas |
| Texto | Texto |
| Línea de tiempo | Formas |
| Actividades visuales | Formas |
| **Otras propiedades** | |
| Autores | 🟠 Se puede recrear manualmente |
| Colaboradores y uso compartido | 🟠 Se puede recrear manualmente |
| Comentarios | 🟠 Se puede recrear manualmente |
| Agrupar | Importado |
| Conjuntos de iconos | Adjunto a formas |
| Capas | 🟠 Se puede recrear manualmente |
| Enlace a | Importado |
| Bloquear | 🟠 Se puede recrear manualmente |
| Notas/Anotaciones | 🟠 Se puede recrear manualmente |
| **Formas** | |
| **Formas de Visio** | **Formas de Miro** |
| Arquitectura AWS | Formas > AWS |
| Azure | Formas > Azur |
| BPMN 2.0 | Formas > BPMN |
| Diagramas de circuito | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Flujo de datos | Formas > Flujo de datos |
| Formas dinámicas | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Arquitectura empresarial | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Integración empresarial | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Relación de entidad | Formas > ERD |
| Ecuaciones | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Planos | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Formas de diagrama de flujo | Formas > Diagrama de flujo |
| Formas geométricas | Formas |
| Google Cloud Platform | Formas > GCP |
| Kubernetes | Formas > Kubernetes |
| Mapas mentales | Mapas mentales |
| Infraestructura de red | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Ingeniería de procesos | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Arquitectura de Salesforce | Formas > Salesforce |
| Diagramas de racks de servidores | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Mapas de sitio | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Formas estándar | Formas |
| Tech Clipart | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| Prototipos de IU | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
| UML | Formas > UML |
| Flujo de valor | Formas > Mapeo del flujo de valor |
| Diagramas de Venn | Importado y editable, pero no disponible en la biblioteca de formas de Miro |
