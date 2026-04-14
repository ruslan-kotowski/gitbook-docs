---
title: OCR (Optical Character Recognition)
article_id: 22401862585234
sidebar_position: 3
created_at: '2024-11-04T13:59:44Z'
updated_at: '2025-08-22T19:14:08Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

OCR is a feature enabling automated recognition of text within images, facilitating data extraction for enhanced data discovery. The OCR support is optimized for high-quality images and is available across various languages with some considerations for handwritten content.

:::note
OCR is optimized for typed text in high-resolution images. Recognition accuracy may decrease with low-quality or handwritten content.
:::

## Best practices for OCR accuracy

#### **Image resolution**

- Recommended: At least 1024 x 768 pixels
- Minimum: 640 x 480 pixels (approximately 300,000 pixels)
- Lower-resolution images may result in partial or inaccurate text extraction.

#### **DPI (Dots Per Inch)**

- Recommended: 300 DPI or higher
- Scanned images below 300 DPI may suffer reduced readability.

#### **Supported file types**

- JPG, JPEG, PNG
- Ensure files are not heavily compressed, as compression artifacts can reduce recognition accuracy.

#### **Image clarity**

- Use well-lit, sharp images with minimal background noise.
- Avoid shadows, glare, or skewed angles.
- Text should not overlap with graphics or complex patterns.

## Language support

OCR is compatible with multiple languages, facilitating broad applicability for data discovery across multilingual data sources.

## Handwriting support

OCR handles handwritten text on a best-effort basis. Results may vary significantly depending on:

- Clarity of handwriting
- Consistency and style
- Language or script used
