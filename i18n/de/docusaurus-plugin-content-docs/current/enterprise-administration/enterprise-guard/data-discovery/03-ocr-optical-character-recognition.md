---
title: OCR (Optische Zeichenerkennung)
article_id: 22401862585234
translation_id: 22401862585234
locale: de
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

Die OCR ermöglicht die automatisierte Erkennung von Text in Bildern und erleichtert die Datenextraktion für eine verbesserte Datenerkennung. Die OCR-Unterstützung ist für hochwertige Bilder optimiert und ist in verschiedenen Sprachen verfügbar, wobei auch handschriftliche Inhalte berücksichtigt werden.

**Hinweis:** Die OCR ist für eingegebenen Text in hochauflösenden Bildern optimiert. Die Genauigkeit der Erkennung kann bei minderwertigen oder handschriftlichen Inhalten abnehmen.

## Best Practices für die OCR-Genauigkeit

#### **Bildauflösung**

- Empfohlen: Mindestens 1024 x 768 Pixel
- Minimum: 640 x 480 Pixel (ca. 300.000 Pixel)
- Bilder mit einer geringeren Auflösung können zu einer unvollständigen oder ungenauen Textextraktion führen.

#### **DPI (Dots Per Inch)**

- Empfohlen: 300 DPI oder höher
- Bei gescannten Bildern mit weniger als 300 DPI kann die Lesbarkeit beeinträchtigt sein.

#### **Unterstützte Dateitypen**

- JPG, JPEG, PNG
- Achte darauf, dass die Dateien nicht zu stark komprimiert sind, da die Komprimierungsartefakte die Genauigkeit der Erkennung verringern können.

#### **Bildklarheit**

- Verwende gut beleuchtete, scharfe Bilder mit wenig Hintergrund.
- Vermeide Schatten, Blendungen oder schräge Winkel.
- Der Text sollte sich nicht mit Grafiken oder komplexen Mustern überschneiden.

## Sprachsupport

Die OCR ist mit mehreren Sprachen kompatibel und ermöglicht so eine breite Anwendbarkeit für die Datenerkennung über mehrsprachige Datenquellen.

## Unterstützung handschriftlicher Texte

Die OCR verarbeitet handschriftlichen Text bestmöglich. Die Ergebnisse können erheblich variieren je nach:

- Deutlichkeit der Handschrift
- Konsistenz und Stil
- Verwendeter Sprache oder Skript
