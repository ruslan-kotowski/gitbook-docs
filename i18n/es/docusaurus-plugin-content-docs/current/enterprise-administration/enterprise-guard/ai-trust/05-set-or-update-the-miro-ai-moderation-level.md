---
title: "Configura o actualiza el nivel de moderaci\xF3n de Miro AI (Beta)"
article_id: 30613174297618
translation_id: 30613174297618
locale: es
sidebar_position: 3
created_at: '2025-10-29T01:15:35Z'
updated_at: '2026-01-12T11:22:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Con la moderación de Miro AI, los admins de empresa pueden ajustar los niveles de filtro de instrucciones que podrían conducir a resultados potencialmente dañinos o inapropiados. Puedes controlar la sensibilidad de la moderación de Miro AI en toda tu organización y filtrar entre categorías como odio, contenido sexual, violencia y autolesiones. Esto te ayuda a alinear el uso de Miro AI con los requisitos, políticas y tolerancia al riesgo de tu organización.

**Nota**: Si tu organización conecta su propio proveedor de LLM (por ejemplo, una integración directa con OpenAI), el selector de moderación se deshabilita y cualquier nivel previamente elegido se ignora para esa integración.

## Requisitos previos

- Asegúrate de tener el complemento de Enterprise Guard.
- Asegúrate de ser un **Company Admin** para la organización que deseas configurar.
- Revisa tus requisitos de gobernanza y política para elegir un nivel inicial adecuado. Se recomienda el predeterminado para la mayoría de las organizaciones.

## Configura o actualiza el nivel de moderación de Miro AI

1. Abre las **Configuraciones** de tu organización en Miro.
2. Ve a **Miro AI** › **Moderación**.
3. Elige un nivel:
   - **Estricto:** Bloquea todo lo del nivel Predeterminado más contenido de bajo a moderado riesgo (por ejemplo, odio sutil o codificado, contenido sexualmente sugerente, violencia no gráfica, menciones de autolesión no explícitas).
   - **Predeterminado (recomendado):** Bloquea contenido moderadamente a severamente dañino (por ejemplo, odio explícito, contenido sexual explícito, violencia gráfica, incitación a la autolesión).
   - **Mínimo:** Bloquea solo contenido gravemente dañino.
4. Haz clic en **Confirmar**.
   El cambio se aplica a todos en la organización de inmediato y se registra en el registro de auditoría.

## Valida el nivel de moderación (opcional)

- Pide a un grupo piloto que pruebe instrucciones típicas y reporte cualquier sobre o sub-filtrado.
- Supervisa los canales de asistencia o de derivación para detectar falsos positivos o daños no detectados durante la primera semana tras un cambio.

## Consejos y mejores prácticas

- Comienza con **Predeterminado**, luego ajusta según los comentarios del piloto y las revisiones de derivación.
- Si los usuarios reportan demasiadas instrucciones bloqueadas, prueba **Predeterminado** (desde Estricto) o **Mínimo** (desde Predeterminado) y publica ejemplos de instrucciones aceptables.
- Si contenido límite se filtra, cambia a **Estricto** y añade guías internas para reducir fricción.
- Revisa el nivel después de cambios en políticas, regulaciones o casos de uso.

## Resolución de problemas

**Control de moderación deshabilitado**
Una integración de LLM personalizada está conectada. Desconéctala para volver a habilitar el selector. Mientras esté conectada, cualquier nivel elegido previamente es ignorado para esa integración.

**Demasiados falsos positivos**
Considera cambiar de **Estricto → Predeterminado** y comparte ejemplos de uso aceptable. Revisa los cambios recientes en el registro de auditoría para confirmar el momento.

**Exposición a contenido dañino**
Asegúrate de que el nivel no esté en **Mínimo**. Considera **Predeterminado** o **Estricto** dependiendo de la tolerancia al riesgo.

**Los usuarios no saben por qué se bloquean las instrucciones**
Publica guías internas señalando tu nivel elegido, ejemplos de instrucciones y rutas de derivación.
