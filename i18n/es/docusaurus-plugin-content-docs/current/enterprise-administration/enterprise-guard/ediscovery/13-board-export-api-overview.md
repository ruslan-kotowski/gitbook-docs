---
title: "Visi\xF3n general de la API de exportaci\xF3n de tableros"
article_id: 17774560667794
translation_id: 17774560667794
locale: es
sidebar_position: 12
created_at: '2024-03-19T12:52:09Z'
updated_at: '2025-07-09T17:32:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

[Las API de eDiscovery](https://developers.miro.com/reference/enterprise-create-board-export) permiten a los clientes del plan Enterprise exportar datos de tableros de Miro para revisarlos manualmente o introducirlos en herramientas creadas específicamente para fines legales, de cumplimiento y de seguridad.

La API de exportación de tableros proporciona un archivo ZIP con una instantánea de los datos del tablero en el momento en que se ejecuta el trabajo, incluida la exportación del contenido del tablero en un formato especificado SVG, PDF o HTML, un archivo JSON con un registro de todos los comentarios, un archivo JSON con una lista de todos los usuarios que vieron o modificaron el tablero, grabaciones de vídeo de la cámara web Talktrack asociadas al tablero, si procede, y un JSON con los matadatos del tablero. Para tableros grandes, la exportación en formato PDF produce varios archivos PDF que representan el tablero completo.

El diseño asíncrono de la API incluye puntos finales para recuperar información sobre un trabajo de exportación de tableros, como el estado.

:::note
Si estás en el plan Enterprise, sólo puedes tener un trabajo de exportación de tableros ejecutándose a la vez. Como cliente de Enterprise Guard, puedes ejecutar hasta cinco trabajos de exportación de tableros simultáneamente con una velocidad de exportación significativamente mayor.
:::

## Casos prácticos

Algunos de los casos de uso más comunes del eDiscovery son:

- **eDiscovery (descubrimiento electrónico):** el proceso de identificar, recopilar, preservar y revisar información almacenada electrónicamente para su uso en un asunto legal.
- **Archivo de información:** práctica en la que las organizaciones mantienen los datos fuera del sistema original con fines de almacenamiento y registro a largo plazo. El contenido y los metadatos ayudan a los clientes a indexar y buscar en el archivo y a controlar proactivamente los problemas de cumplimiento.
