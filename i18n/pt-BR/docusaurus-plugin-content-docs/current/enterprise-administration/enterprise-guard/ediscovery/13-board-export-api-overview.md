---
title: "Vis\xE3o geral da API de exporta\xE7\xE3o do board"
article_id: 17774560667794
translation_id: 17774560667794
locale: pt-br
sidebar_position: 12
created_at: '2024-03-19T12:52:09Z'
updated_at: '2025-07-09T17:32:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

[As APIs de eDiscovery](https://developers.miro.com/reference/enterprise-create-board-export) permitem que clientes no plano Enterprise exportem dados do board do Miro para serem revisados ​​manualmente ou inseridos em ferramentas criadas especificamente para fins legais, de conformidade e segurança.

A API de exportação do board fornece um arquivo ZIP com um instantâneo dos dados do board no momento em que o trabalho é executado, incluindo a exportação do conteúdo do board em um formato especificado SVG, PDF ou HTML, um arquivo JSON com um registro de todos os comentários, um arquivo JSON com uma lista de todos os usuários que visualizaram ou modificaram o board, gravações de vídeo da webcam do TalkTrack associadas ao board, se aplicável, e um JSON com metadados do board . Para boards grandes, a exportação em formato PDF produz vários arquivos PDF representando a board completa.

O design da API assíncrona inclui pontos de extremidade para recuperar informações sobre um trabalho de exportação da board , como o status.

:::note
Se você estiver no plano Enterprise , poderá ter apenas um trabalho de exportação de board em execução por vez. Como cliente do Enterprise Guard , você pode executar até cinco trabalhos de exportação de board simultaneamente com uma velocidade de exportação significativamente maior.
:::

## Casos de uso

Alguns dos casos de uso comuns do eDiscovery incluem:

- **eDiscovery (descoberta eletrônica):** o processo de identificar, coletar, preservar e revisar informações armazenadas eletronicamente para uso em uma questão legal.
- **Arquivo de informações:** prática na qual as organizações mantêm dados fora do sistema original para fins de armazenamento de longo prazo e manutenção de registros. O conteúdo e os metadados ajudam os clientes a indexar e pesquisar o arquivo e monitorar proativamente as questões de conformidade .
