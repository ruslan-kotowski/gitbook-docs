---
title: Vista general de bloqueo de instrucciones (Beta)
article_id: 29332642230546
translation_id: 29332642230546
locale: es
sidebar_position: 4
created_at: '2025-09-09T07:58:00Z'
updated_at: '2026-01-12T11:23:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

El bloqueo de instrucciones permite a los administradores de contenido sensible evitar que los usuarios envíen instrucciones a la IA que incluyan información sensible, ayudándote a mantener los datos sensibles fuera de Miro AI en toda tu organización. Miro escanea el texto que un usuario ingresa en el campo de instrucciones y cualquier contenido basado en texto que añadan desde el tablero. Si ese contenido coincide con las etiquetas de sensibilidad o patrones de código fuente seleccionados en la configuración de bloqueo de instrucciones, Miro bloquea el envío de la instrucción.

:::note
Solo se admite contenido basado en texto en la versión Beta.
:::

## Cómo funciona

- Tú eliges qué categorías de etiquetas bloquear a nivel de la organización. Los cambios se aplican de inmediato para todos en tu organización.
- Cuando se detectan datos sensibles en una instrucción, Miro AI muestra un mensaje de política en el punto de entrada del usuario, la instrucción se bloquea y no se puede enviar a Miro AI.
- El bloqueo de instrucciones y el escaneo de tableros son diferentes. El escaneo de tableros localiza contenido sensible en los tableros y puede clasificar automáticamente el tablero. El bloqueo de instrucciones revisa lo que los usuarios intentan enviar a Miro AI.

## Qué se bloquea

- Etiquetas relacionadas con la privacidad: Selecciona entre todas nuestras etiquetas de privacidad integradas, como SPII, HIPAA, credenciales, números financieros. Para más información sobre nuestras etiquetas de privacidad integradas, consulta la [Referencia de etiquetas de sensibilidad e infotiopos](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md).
- Escaneo de código. Cuando está habilitado, Miro bloquea las instrucciones que incluyen código fuente reconocido. Consulta [Escaneo de código](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md) para más detalles.

## Resultados típicos para los usuarios

Cuando el usuario introduce una instrucción que contiene información sensible según tu configuración:

- Los usuarios ven un mensaje como "No podemos generar este contenido ya que puede violar la política de tu organización."
- La instrucción no se envía a Miro AI. Los usuarios pueden editar la instrucción e intentarlo nuevamente.

## Escaneo de código

El escaneo de código bloquea las instrucciones de AI que incluyen código fuente reconocible. Se requiere un mínimo de 5 líneas de código para activar el bloqueo.

Ejemplo:

```
function connect() {

  const token = "example-token";

  fetch("https://api.example.com/health");

  return true;

}
```

## Idiomas compatibles

- C
- C#
- C++
- Go
- HTML
- Java
- JavaScript
- JSON
- PHP
- PowerShell
- Python
- Rust
- Shell script
- SQL
- TypeScript
