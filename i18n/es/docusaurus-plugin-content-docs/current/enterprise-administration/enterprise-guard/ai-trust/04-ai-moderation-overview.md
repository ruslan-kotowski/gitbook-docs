---
title: "Visi\xF3n general de moderaci\xF3n de AI (Beta)"
article_id: 29491049430674
translation_id: 29491049430674
locale: es
sidebar_position: 2
created_at: '2025-09-15T16:27:59Z'
updated_at: '2026-01-12T11:21:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Con la moderación de Miro AI, los admins de empresa pueden ajustar los niveles de filtrado de instrucciones que podrían contener texto potencialmente dañino o inapropiado. Puedes configurar la sensibilidad de moderación de Miro AI a nivel organizacional para filtrar contenido, incluyendo odio, contenido sexual, violencia y autolesiones. Esto te ayuda a alinear el uso de Miro AI con los requisitos, políticas y tolerancia al riesgo de tu organización.

:::note
*Si tu organización conecta su propio proveedor de LLM (por ejemplo, una integración directa con OpenAI), el selector de moderación se deshabilita y cualquier nivel previamente elegido se ignora para esa integración.*
:::

## Niveles de moderación

Controla el contenido de Miro AI en toda tu organización con la moderación de Miro AI. Configura el nivel de filtrado a Estricto, Predeterminado o Mínimo para determinar qué instrucciones se bloquean. Revisa la tabla a continuación para comparar rápidamente los niveles y luego consulta las secciones detalladas para obtener más orientación.

| Nivel | Qué hace | Mejor para | Compensaciones |
| --- | --- | --- | --- |
| Estricto | Bloquea el contenido de "Default" + contenido de riesgo bajo a moderado. | Organizaciones altamente reguladas, educación. | Más falsos positivos; potencial sobrefiltrado. |
| Predeterminado (recomendado) | Bloquea contenido moderadamente a severamente perjudicial. | La mayoría de los casos de uso comercial. | Algunos contenidos límite pueden pasar. |
| Mínimo | Bloquea solo contenido gravemente dañino. | Contextos creativos/juegos/medios . | Mayor exposición a daño de bajo a moderado. |

:::note
*Se recomienda el estándar por defecto para la mayoría de las organizaciones. Filtra contenido que la mayoría considera inapropiado o dañino manteniendo una amplia usabilidad.*
:::

## Nivel estricto

### Qué filtra

Todo en el nivel Predeterminado más contenido de riesgo bajo a moderado (por ejemplo, discurso de odio sutil o codificado, contenido sexualmente sugestivo, violencia no gráfica o menciones no explícitas de autolesiones).

### Cuándo usar

- Industrias reguladas o políticas organizacionales adversas al riesgo
- Programas educativos o enfocados en la juventud
- Proyectos piloto con baja tolerancia al riesgo

### Compromisos

- Más falsos positivos y bloqueos de instrucciones en el límite
- Requiere orientación para reducir la fricción con los usuarios

## Nivel Predeterminado (recomendado)

### Qué filtra

Contenido moderadamente a severamente dañino (discurso de odio explícito, contenido sexual explícito, violencia gráfica, fomento del autolesionismo).

### Cuándo usar

- La mayoría de las organizaciones que buscan un equilibrio entre seguridad y usabilidad

### Trade-offs

- Instrucciones contextuales o fronterizas pueden pasar

## Nivel Mínimo

### Qué filtra

Solo contenido severamente dañino.

### Cuándo usar

- Equipos creativos que necesitan una expresión más amplia (juegos, medios)
- Proyectos de ideación interna con claros caminos de derivación

### Trade-offs

- Mayor exposición a contenido dañino de bajo a moderado en los resultados

## Auditoría y cumplimiento

Los cambios en el nivel de moderación se capturan en el registro de auditoría de la organización, incluyendo el valor anterior, el nuevo valor, quién lo cambió y cuándo se cambió. Para obtener más información, consulta nuestra documentación sobre [Registros de auditoría](../security-management/01-audit-logs.md).

## Prácticas recomendadas

- Empieza con el nivel Predeterminado y luego ajusta según los comentarios de las pruebas piloto y las revisiones de derivación.
- Combina el nivel Estricto con una guía interna clara sobre las instrucciones aceptables para reducir los falsos positivos.
- Si necesitas el nivel Mínimo, define cuándo los equipos deben derivar o reportar salidas problemáticas.
- Revisa tu configuración después de actualizaciones importantes de políticas o regulaciones.

- Visión general de moderación con IA
- Niveles de moderación
- Nivel estricto
- Nivel predeterminado (recomendado)
- Nivel mínimo
- Auditoría y cumplimiento
- Prácticas recomendadas
