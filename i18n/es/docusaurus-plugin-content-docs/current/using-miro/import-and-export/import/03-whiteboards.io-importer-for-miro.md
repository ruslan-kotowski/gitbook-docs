---
title: Importador de pizarras.io para Miro
article_id: 20624350720402
translation_id: 20624350720402
locale: es
sidebar_position: 3
created_at: '2024-08-07T16:30:40Z'
updated_at: '2026-01-19T14:08:30Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
---

El Importador de Pizarras.io de ServiceRocket para Miro es una solución fácil de usar, diseñada para agilizar la importación de datos desde las [Pizarras.io](https://whiteboards.io/) a la app [Miro](https://miro.com/app/dashboard/). Carga tus copias de seguridad generadas en la pizarra con rapidez y facilidad.

Consigue hoy mismo tu acceso al importador. Visita `https://www.servicerocket.com/miro/whiteboards-io-miro-migration` para más detalles.

## **Exportar tableros de Whiteboards.io**

1. Iniciar sesión en [Pizarras.io](https://whiteboards.io/).
2. En la página principal, haz clic en Exportar tableros en el mensaje de estado de advertencia.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeiEjTayvBy6uufihIKif-C14REIupCmqvKKU6_DMUVhT6lrGC01PkVkXOVJENoCmA2piy40VIRGxFT4YGIE870A9TSYnIpSDyY37H1euf5ZsiP_dbN3zMpcp5GOCIRAcsaJonD8obCfo-WSOxfax4HVtuN?key=RrckFddS6o4KjRqYlXDbPw)
*Haz clic en Exportar tableros desde el mensaje de estado de advertencia para empezar*

3. A continuación, realiza los siguientes pasos para exportar el tablero.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeyDxMc_ob24RYp6Rne_MAIXICO3JRrSesUAHtsyJ0hsG3DjTC5iiNg6_b-97m97XkgtjWRbX0uDcmbyBqMz6tGEEayg0eLvmVIUzLNwTizSYtlQBQXIP5XSNMQFTX2psIIE6SnbVo74EQABRH9vDwe9SPK?key=RrckFddS6o4KjRqYlXDbPw)
*Comprueba que los ajustes son correctos al exportar tu tablero*

1. 1. Selecciona sólo el formato .json.
   2. Desmarca Incluir medios (imágenes, vídeos y otros archivos).
   3. Haz clic en Exportar para confirmar los ajustes y exportar el tablero.

4. Se generará correctamente un archivo .zip.

## **Importar tableros de Whiteboards.io a Miro**

1. Abre tu tablero de Miro.
2. En la barra de herramientas, haz clic en Más apps > selecciona o busca Whiteboards.io Miro Importer.
3. Haz clic en Elegir archivo para cargar el archivo (.zip) generado a partir del archivo [Pizarras.io](http://whiteboards.io/) app.
4. A continuación, selecciona el tablero que quieras importar y haz clic en Importar.
5. Una vez finalizada la importación, el sistema mostrará el estado del tablero como COMPLETADO.
6. Cierra la app y vuelve a la página principal de Miro. La app importará los tableros seleccionados a tu cuenta de equipo.

## **Pizarras.io mapa de datos en Miro**

El mapeo de datos es esencial para mantener la integridad de los datos, la coherencia y las diferencias de esquema durante la transición de una app a otra. En las tablas siguientes se enumeran toda la terminología equivalente, las estructuras de datos, los nombres de los campos, los formatos, etc.

|  |  |  |
| --- | --- | --- |
| **Pizarras.io** | **Miro** | notas |
| Texto | [Texto](https://developers.miro.com/docs/text-1) | N/A |
| forma | [forma](https://developers.miro.com/docs/shape-1) | - La forma de corazón se importará como una forma de nube. - La forma paperTape se importará como una forma de diagrama de flujo_entrada_salida. - Se importará un icono como imagen. |
| Tarjeta | [Nota adhesiva](https://developers.miro.com/docs/stickynote-1) | - El formato de las fuentes se perderá al convertir a tarjeta. - El color de las tarjetas se perderá y la alineación estará desalineada. - El tamaño de la nota adhesiva puede variar. |
| Línea | [Conector](https://developers.miro.com/docs/connector_intro) | N/A |
| marco | [marco](https://developers.miro.com/docs/frame-1) | Los objetos hijos del marco no pueden vincularse al marco padre. |
| Dibuja gratis | [Imagen](https://developers.miro.com/docs/image-1) (.svg) | N/A |
| Comentarios | N/A | Miro no proporciona ningún método para trazar este mapa. |
| Archivo | [Archivo](../../troubleshooting-technical-questions/technical-guidelines/03-supported-file-formats.md) | Tipo y formato de archivo:   - Imágenes - Tablas y hojas de cálculo - Documentos de texto - Presentaciones |
| Imagen | [Imagen](https://developers.miro.com/docs/image-1) | N/A |
| Insertar iFrame | [Elemento insertado](https://developers.miro.com/docs/embed-2) | N/A |
| Tabla de tarjetas | [Tarjeta](https://developers.miro.com/docs/card-1) y [marco](https://developers.miro.com/docs/frame-1) | Sin la columna ni el nombre del carril. |
| Mapa mental | [Mapa mental](https://developers.miro.com/docs/mind-maps) (Experimental) | No se admite el color del borde. |
| Tarjeta GitHub | [Tarjeta](https://developers.miro.com/docs/card-1) | N/A |
| tarjeta de Jira | Texto con URL de incidencia de Jira | N/A |
