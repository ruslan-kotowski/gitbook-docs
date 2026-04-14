---
title: "OCR (reconocimiento \xF3ptico de caracteres)"
article_id: 22401862585234
translation_id: 22401862585234
locale: es
sidebar_position: 2
created_at: '2024-11-04T13:59:44Z'
updated_at: '2025-08-22T19:14:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

OCR es una función que permite el reconocimiento automatizado de texto en las imágenes, lo que facilita la extracción de datos para el descubrimiento de datos mejorado. OCR está optimizado para imágenes de alta calidad y está disponible en diversos idiomas con algunas consideraciones para el contenido escrito a mano.

**Nota:** OCR está optimizado para texto tecleado en imágenes de alta resolución. La precisión del reconocimiento puede disminuir con contenido de baja calidad o escrito a mano.

## Prácticas recomendadas para la precisión de OCR

#### **Resolución de imagen**

- Recomendada: al menos 1024 x 768 píxeles
- Mínima: 640 x 480 píxeles (aproximadamente 300 000 píxeles)
- Las imágenes de menor resolución pueden dar lugar a una extracción de texto parcial o inexacta.

#### **PPP (puntos por pulgada)**

- Recomendado: 300 PPP o más
- La legibilidad puede verse reducida en imágenes escaneadas por debajo de 300 PPP.

#### **Tipos de archivo compatibles**

- JPG, JPEG, PNG.
- Asegúrate de que los archivos no estén muy comprimidos, ya que los artefactos de compresión pueden reducir la precisión del reconocimiento.

#### **Claridad de imagen**

- Usa imágenes nítidas y bien iluminadas con mínimo ruido de fondo.
- Evita sombras, reflejos o ángulos sesgados.
- El texto no debe superponerse con gráficos o patrones complejos.

## Compatibilidad de idioma

OCR es compatible con varios idiomas, lo que favorece una amplia aplicabilidad para el descubrimiento de datos en fuentes de datos multilingües.

## Compatibilidad con escritura a mano

OCR procesa el texto escrito a mano con el mejor esfuerzo posible. Los resultados pueden variar significativamente en función de los siguientes factores:

- Claridad de la escritura a mano
- Consistencia y estilo
- Idioma o script utilizado
