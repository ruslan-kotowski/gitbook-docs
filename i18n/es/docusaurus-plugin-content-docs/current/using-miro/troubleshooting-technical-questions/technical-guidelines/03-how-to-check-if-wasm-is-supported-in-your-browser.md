---
title: Cómo verificar si WASM es compatible en tu navegador
article_id: 33769132852498
translation_id: 33769132852498
locale: es
sidebar_position: 3
created_at: '2026-03-04T12:47:24Z'
updated_at: '2026-03-16T13:02:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Quién puede hacerlo: Todos los usuarios Qué planes: Free, Starter, Business,
    Enterprise, Educación Qué plataformas: Navegador'
---

WebAssembly (WASM) puede estar deshabilitado por razones que incluyen el cumplimiento con políticas de seguridad establecidas por tu organización o la falta de soporte en entornos más antiguos, por ejemplo.

> **CONSEJO:** La [tabla de comparación de WebAssembly](https://webassembly.org/features/?categories=browsers) muestra qué funciones de WASM son compatibles con tu navegador.

Puedes verificar si tu navegador soporta WASM.

Sigue estos pasos:

1. Abre las herramientas de desarrolladores.
   - En tu navegador:
     - (MacOS) Chrome, Edge, Firefox: `⌘ + ⌥ + I`
     - (Linux, Windows) Chrome, Edge, Firefox: `Ctrl + Shift + I`, o `F12`
     - (MacOS) Safari: Ve a **Configuración** > **Avanzado**. Habilita **Mostrar menú Desarrollo en la barra de menú** | **Mostrar funciones para desarrolladores web**. Abre **Desarrollo** > **Mostrar consola de JavaScript**.
   - En la app de escritorio de Miro:
     - En la parte superior izquierda haz clic en **Ayuda** > **Abrir herramientas de desarrollo**.
2. En las DevTools, haz clic en la pestaña **Consola**.
3. En la línea de entrada de la consola, escribe o pega `typeof WebAssembly`.
4. En tu teclado, presiona **ENTER**.
5. Interpreta el resultado:
   - Si la consola devuelve `undefined`, entonces WebAssembly no es compatible o está deshabilitado.
   - Si la consola devuelve `object`, entonces WebAssembly es compatible.![](../../../../../../../docs/using-miro/troubleshooting-technical-questions/technical-guidelines/images/33770259460626_image.png)
     *La consola de DevTools muestra* `object` *cuando WASM está disponible en tu navegador.*

     > **NOTA:** Si la consola devuelve `object` y aún no puedes acceder a Miro, puedes revisar otras [posibles incidencias y soluciones](../troubleshooting), o contactar al [Soporte de Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
