---
title: Requisitos de sistema
article_id: 360017731553
translation_id: 360017731553
locale: es
sidebar_position: 1
created_at: '2019-02-11T10:14:54Z'
updated_at: '2026-03-06T14:57:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Este artículo describe los requisitos del sistema para usar Miro, incluyendo el dispositivo, GPU y WebAssembly.

Para trabajar en Miro, asegúrate de que tu dispositivo cumpla con los siguientes requisitos mínimos o recomendados del sistema.

Sin embargo, ten en cuenta que los parámetros mencionados a continuación no son definitivos, ya que el rendimiento de Miro puede estar relacionado con varios otros factores tales como:

- Tareas en segundo plano
- Número de pestañas en el navegador y con qué frecuencia alternas entre ellas
- La resolución del monitor desde el que abres Miro
- Estabilidad de la conexión Wi-Fi
- Número de usuarios en el tablero
- Sistema de refrigeración del dispositivo

Si experimentas problemas de rendimiento/acceso, por favor revisa las [guías de solución de problemas](../troubleshooting) y los [consejos para optimizar el rendimiento del tablero](../../tools/troubleshooting/04-board-performance-and-loading-issues.md).

|  |  |  |
| --- | --- | --- |
|  | **Mínimo** | **Recomendado** |
| **CPU** | 3 GHz (2 núcleos/4 hilos) | 2,8 GHz (4 núcleos/8 hilos) |
| **Memoria RAM** | 8 GB | 16 GB (DDR4) |
| **Ancho de banda de red** | 8 Mb/s | 32 Mb/s |

**Ten en cuenta que correr Miro en un hardware de gama alta que esté muy por encima de la especificación recomendada podría no resultar en el aumento de rendimiento esperado, ya que Miro es una aplicación web que funciona por medio del motor web del navegador. En tal caso, el motor web no podrá usar todo el potencial del dispositivo, pues el software instalado localmente en tu computadora está diseñado para una arquitectura particular del sistema operativo y la CPU.*

Los requerimientos mínimos del sistema para el uso cómodo de Miro en [tabletas](../../../getting-started/apps-for-devices/11-tablet-app.md) son 6 GB de RAM.

Miro se puede usar en diferentes tipos de dispositivos. Puedes abrir Miro en un navegador, descargar el [cliente de escritorio](../../../getting-started/apps-for-devices/05-desktop-app.md), la [aplicación para tabletas](../../../getting-started/apps-for-devices/11-tablet-app.md), la [aplicación móvil](../../../getting-started/apps-for-devices/08-mobile-app.md), o [usar Miro en una pantalla interactiva](../../../getting-started/apps-for-devices/07-interactive-displays.md).

**Modo sin conexión**

Dado que Miro se basa en la visión de una solución de nube perfecta para la colaboración *en línea*, un modo *sin conexión* de la herramienta no forma parte de nuestros planes en este momento. Sin embargo, ofrecemos varias opciones de exportación. [Aprende más](../../import-and-export/export/03-how-to-export-your-board.md).

## Requisitos de GPU y WebAssembly

Miro utiliza aceleración de hardware de GPU y WebAssembly (WASM) para un renderizado fluido y para soportar ciertas funciones avanzadas.

### Uso de Miro sin GPU

Para un rendimiento óptimo, Miro requiere aceleración de hardware de GPU.

Si la aceleración de hardware de GPU no está disponible, por ejemplo en algunas máquinas virtuales, o cuando la aceleración de hardware está deshabilitada, Miro cambia automáticamente a un renderizador basado en CPU.

:::tip
Para tener la mejor experiencia con Miro, mantén habilitada la aceleración por hardware cuando sea posible.
:::

Sin aceleración por hardware GPU, puedes experimentar los siguientes cambios en el rendimiento:

- Algunas funciones que dependen de GPU pueden no estar disponibles o mostrarse como marcadores de posición
- Desplazamiento y zoom más lento, especialmente en tableros grandes, o tableros con mucho contenido multimedia
- La funcionalidad básica del tablero puede no comportarse como se espera
- Mayor uso de CPU

### Uso de Miro sin WebAssembly (WASM)

Algunas funciones de Miro dependen de módulos WebAssembly (WASM).

La mayoría de los navegadores modernos habilitan WASM por defecto. Si WASM no está disponible, por ejemplo, bloqueado en cumplimiento de políticas empresariales, deshabilitado en el navegador, o no soportado en entornos antiguos, Miro cambia automáticamente a rutas de renderizado basadas en JavaScript donde sea posible.

**Más información:** Consulta [Cómo comprobar si WASM es compatible con tu navegador](https://help.miro.com/hc/articles/33769132852498).

:::tip
Para la mejor experiencia en Miro, mantén habilitado WebAssembly. En un entorno gestionado, si sospechas que WASM está bloqueado, entonces consulta con tu equipo de TI.
:::

Sin WASM, puedes experimentar los siguientes cambios en el rendimiento:

- Las funciones que requieren WASM pueden no inicializarse y aparecer ocultas o como marcadores de posición
- Los tableros que dependen de la funcionalidad basada en WASM pueden no cargarse completamente o no cargarse en absoluto
