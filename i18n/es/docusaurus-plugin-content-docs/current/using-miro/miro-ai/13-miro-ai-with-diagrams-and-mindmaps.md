---
title: Miro AI con Diagramas y mapas mentales
article_id: 28782102127890
translation_id: 28782102127890
locale: es
sidebar_position: 13
created_at: '2025-08-15T08:50:59Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: creation-toolbar
---

Crear un diagrama o mapa mental

1. Encima de la barra de herramientas de Creación, selecciona **Crear con IA**.
   Se abrirá el panel de **Crear con IA**.
2. Haz clic en **Biblioteca de Sidekicks** (botón de cuatro cuadrados en la esquina superior derecha) **>** **Formatos** > **Diagrama o mapa mental**.
   Se abrirá el panel de instrucciones.
3. Selecciona un tipo de diagrama o mapa mental.
4. En el cuadro de respuesta, describe el diagrama o mapa mental que deseas crear.

   > 💡 Selecciona una de las instrucciones iniciales para comenzar tu descripción.

   > 💡 Aprende cómo Miro AI maneja la entrada de estilo y color para diagramas. Consulta Entrada de estilo y color para diagramas de Miro AI.
5. Presiona **ENTER** en tu teclado, o haz clic en la flecha de respuesta.
   Miro AI genera un diagrama o mapa mental en el tablero. Para interrumpir la generación, puedes optar por hacer clic en **DETENER** y repetir el paso 3.
6. Haz una de las siguientes acciones:
   - Haz clic en **Aplicar al lienzo**.
      Tu diagrama o mapa mental está listo para que lo edites. Has completado el procedimiento.
   - Haz clic en **Descartar todo**.
      Tu boceto de diagrama o mapa mental se borra y el panel de **Crear con IA** se restablece.
   - En la barra lateral de **Crear con IA**, continúa describiendo tu diagrama o mapa mental y repite el paso 6 hasta que hayas aplicado tu diagrama o mapa mental al tablero.

## Digitaliza diagramas dibujados a mano

Miro AI incluye Digitalizar Diagrama (BETA), una función que convierte tus bocetos de diagramas dibujados a mano en diagramas completamente editables en tu tablero.

Sigue estos pasos:

1. Carga una imagen de tu diagrama a mano alzada en un tablero de Miro.
2. Selecciona la imagen.
   Se muestra el menú contextual.
3. En el menú contextual, haz clic en **Miro AI**.
4. Selecciona **Digitize Diagram**.
   Miro AI genera una versión completamente editable de tu diagrama. Asegúrate de inspeccionar el resultado y hacer los ajustes o alineaciones necesarios.

## Entrada de estilo y color para diagramas de Miro AI

Miro AI responde a las instrucciones de estilo semántico. Por ejemplo, en tu instrucción puedes describir una estética o especificar un estilo preferido. Miro AI genera tu diagrama o mapa mental basado en tu descripción o preferencia y asegura que todas las propiedades correspondan. Puedes seguir dando instrucciones o editar manualmente para refinar tu resultado.

La siguiente tabla muestra cómo Miro AI produce resultados basados en tu instrucción para diagramas.

| Caso de uso | Descripción | Acción de IA | Paleta de colores | Color del borde |
| --- | --- | --- | --- | --- |
| **Sin entrada de color** | No proporcionas ninguna preferencia ni especificación de color, por ejemplo, "Crear un diagrama de flujo" | El sistema usa la paleta de colores predeterminada | Amarillo sol, Azul océano y Verde musgo | Cada elemento recibe un color de borde más contrastante y apropiado |
| **Entrada de color vaga** | Das una preferencia estética o tema, por ejemplo, "Crear un diagrama naranja" | El sistema usa tu preferencia como entrada y adapta el color a la paleta de colores apagados de Miro, optimizada para accesibilidad | En este ejemplo, Miro AI genera un diagrama con naranja apagado | En este ejemplo, Miro AI genera un borde naranja de mayor contraste correspondiente |
| **Entrada de color específica** | Proporcionas valores HEX o RGB para especificar los colores de la marca, por ejemplo, "Generar secuencia UML... en color #006FF" | Reemplaza los valores predeterminados del sistema | Cumple con los valores especificados en la solicitud | Miro crea automáticamente un color de borde apropiado y de mayor contraste basado en la forma o color especificado |
