---
title: "OCR (Reconnaissance optique de caract\xE8res)"
article_id: 22401862585234
translation_id: 22401862585234
locale: fr
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

L’OCR (Optical Character Recognition, ou reconnaissance optique de caractères) est une fonctionnalité de reconnaissance automatique du texte dans des images, facilitant l’extraction de données pour optimiser la découverte des données. Le service OCR est optimisé pour les images de haute qualité et est disponible dans différentes langues, avec certaines dispositions pour le contenu manuscrit.

**Note :** l’OCR est optimisée pour la reconnaissance de texte dactylographié dans les images de haute résolution. La qualité de la reconnaissance peut être affectée lorsque le contenu est de mauvaise qualité ou manuscrit.

## Meilleures pratiques pour une OCR précise

#### **La résolution**

- Recommandations : minimum 1024 × 768 pixels
- Minimum : 640 × 480 pixels (environ 300 000 pixels)
- Lorsque la résolution est plus faible, l’extraction du texte peut être partielle ou inexacte.

#### **DPI (points par pouce)**

- Recommandations : 300 DPI ou plus
- Les images numérisées à moins de 300 DPI peuvent être moins lisibles.

#### **Types de fichiers pris en charge**

- JPG, JPEG, PNG
- Assurez-vous que les fichiers ne sont pas fortement compressés, car les artefacts de compression peuvent affecter la précision de la reconnaissance.

#### **La clarté de l’image**

- Utilisez des images claires et nettes avec le moins de bruit numérique possible.
- Évitez les ombres, les reflets ou les prises de biais.
- Le texte ne doit pas chevaucher des graphiques ni des motifs complexes.

## Langues prises en charge

L’OCR est compatible avec plusieurs langues, ce qui permet de l’appliquer à la découverte de données issues de sources multilingues.

## Prise en charge des textes manuscrits

L’OCR prend en charge le texte manuscrit dans la mesure du possible. Les résultats peuvent varier significativement en fonction :

- de la lisibilité de l’écriture manuscrite
- de la cohérence et du style
- de la langue ou du script
