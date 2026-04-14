---
title: "Vis\xE3o geral do painel de descoberta de dados"
article_id: 26806897106834
translation_id: 26806897106834
locale: pt-br
sidebar_position: 1
created_at: '2025-05-19T11:10:19Z'
updated_at: '2025-11-25T15:51:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

O painel de descoberta de dados fornece uma visualização centralizada das informações sensíveis detectadas nos boards da sua organização. Isso permite que admins monitorem, classifiquem e gerenciem riscos de dados identificando conteúdos relacionados à privacidade ou sensíveis para o negócio. O painel de descoberta de dados inclui as seguintes métricas:

:::note
Todas as métricas no Enterprise Guard excluem boards de times na lixeira e boards sob retenção legal.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Título** | **Descrição** | **Domínio** | **Aparece no painel de visão geral** | **Tem métrica histórica** |
| Número de boards sensíveis | Número de boards que têm pelo menos uma etiqueta integrada, etiqueta de palavra-chave ou etiqueta de privacidade atribuída. | Descoberta de dados | ✅ | ❌ |
| Número de boards que têm itens confidenciais da empresa | Número de boards que têm pelo menos uma etiqueta integrada ou etiqueta de palavra-chave atribuída. | Descoberta de dados | ✅ | ✅ |
| Número de boards que possuem itens sensíveis relacionados à privacidade | Número de boards que têm pelo menos uma etiqueta de privacidade atribuída. | Descoberta de dados | ✅ | ✅ |
| Número de boards que têm uma etiqueta atribuída por etiqueta | Para cada etiqueta individual nas três categorias (integrada, palavra-chave ou privacidade), conte o número de boards com essa etiqueta atribuída. | Descoberta de dados | ❌ | ❌ |
| Quantidade de etiquetas relacionadas à privacidade habilitadas. | Quantidade de etiquetas relacionadas à privacidade habilitadas. | Descoberta de dados | ❌ | ❌ |
| Quantidade de etiquetas de palavras-chave habilitadas. | Quantidade de etiquetas de palavras-chave habilitadas. | Descoberta de dados | ❌ | ❌ |
| Quantidade de etiquetas Confidencial da empresa habilitadas | Quantidade de etiquetas Confidencial da empresa habilitadas | Descoberta de dados | ❌ | ❌ |

## Entenda os erros, os estados vazios e as alterações históricas

Compreender como interpretar estados vazios e mensagens de erro é essencial para ler com precisão as métricas do painel do Enterprise Guard.

### Entenda o comportamento de dados históricos quando as configurações são alteradas

Se a descoberta de dados for desabilitada após a coleta dos dados, as métricas históricas ainda exibirão valores do período ativo. Por exemplo, se você desabilitar a descoberta de dados em maio e a descoberta de dados estava ativa em abril:

- Os valores de abril continuarão aparecendo no painel.
- O gráfico de maio exibirá **sem dados disponíveis**, pois a coleta de dados foi interrompida.

## Visualizar resultados da descoberta de dados

O ciclo de descoberta de dados ocorre pelo menos uma vez por hora e verifica todas as atualizações do board em busca de informações relacionadas à privacidade, sensíveis da empresa ou personalizadas sensíveis ao negócio, conforme sua configuração de descoberta de dados. Isso inclui os boards que já foram verificados no ciclo de descoberta de dados anterior.

Os resultados da descoberta de dados aparecem abaixo dos gráficos de métricas. Você pode visualizar informações como o nome da etiqueta, status, tipo, classificação, número de boards, e assim por diante.

Para mais informações sobre a revisão de boards com documentação relacionada à privacidade, [consulte este artigo](16-review-boards-with-privacy-related-information.md).

Para mais informações sobre a revisão de boards com dados sensíveis da empresa e informações personalizadas sensíveis para os negócios, [consulte este artigo](14-review-boards-with-business-sensitive-and-custom-business-sensitive-information-beta.md).

Para mais informações sobre a revisão de boards com etiquetas personalizadas e sensíveis para os negócios, [consulte este artigo](15-review-custom-business-sensitive-labels-and-data-discovery-results.md).

:::note
- Para visualizar os resultados da descoberta de dados, você deve ter a [função de admin de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, fale com seu Admin da empresa.

- Continuamos trabalhando com nosso parceiro de tecnologia e clientes para melhorar o sistema de detecção de conteúdo sensível, mas não podemos garantir que 100% dos dados confidenciais em seus boards serão encontrados e sinalizados. Nosso sistema de detecção de conteúdo sensível usa padrões e outros critérios para determinar a probabilidade de uma correspondência. Pode haver momentos em que o sistema sinalize incorretamente os dados dos seus boards como provavelmente confidenciais (um falso positivo) ou falhe ao sinalizar dados como confidenciais (um falso negativo). Vários fatores contribuem para essas ocorrências, incluindo a proximidade de termos correlatos ou a formatação de dados confidenciais.

Para mais informações sobre como suprimir correspondências falso-positivas, veja [Suprimir uma correspondência de conteúdo sensível](11-suppress-a-sensitive-content-match.md).
:::

##

##
