---
title: "OCR (Optical Character Recognition; reconhecimento \xF3ptico de caracteres)"
article_id: 22401862585234
translation_id: 22401862585234
locale: pt-br
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

O OCR é uma funcionalidade que permite fazer o reconhecimento automático de texto em imagens, o que facilita a extração de dados para otimizar a descoberta de dados. A tecnologia OCR é otimizada para imagens de alta qualidade e está disponível em vários idiomas, embora tenha algumas limitações com relação a conteúdo escrito à mão.

**Observação:** o OCR é otimizado para reconhecer textos digitados em imagens de alta resolução. A eficácia do reconhecimento pode ser menos precisa com conteúdo escrito à mão ou de baixa qualidade.

## Melhores práticas para precisão do OCR

#### **Resolução de imagem**

- Recomendado: pelo menos 1024 x 768 pixels
- Mínimo: 640 x 480 pixels (aproximadamente 300 mil pixels)
- A extração de texto pode ser parcial ou imprecisa em imagens com resolução mais baixa.

#### **DPI (pontos por polegada)**

- Recomendado: 300 DPI ou superior
- A qualidade de leitura pode ser reduzida em imagens digitalizadas com menos de 300 DPI.

#### **Tipos de arquivos compatíveis**

- JPG, JPEG, PNG.
- Certifique-se de que os arquivos não estejam excessivamente compactados, já que isso pode comprometer a precisão do reconhecimento.

#### **Nitidez da imagem**

- Use imagens bem iluminadas e nítidas, com mínimo ruído de fundo.
- Evite sombras, brilho ou ângulos inclinados.
- O texto não deve se sobrepor a gráficos ou padrões complexos.

## Idiomas compatíveis

O OCR é compatível com vários idiomas, o que torna a descoberta de dados mais abrangente em fontes de dados multilíngues.

## Compatibilidade com texto escrito à mão

O OCR processa textos escritos à mão sempre que possível. Os resultados podem variar bastante, a depender de:

- Clareza da escrita à mão
- Consistência e estilo
- Idioma ou escrita usada
