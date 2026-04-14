---
title: Exibir resultados da descoberta de dados
article_id: 15794382139154
translation_id: 15794382139154
locale: pt-br
sidebar_position: 16
created_at: '2023-12-15T15:47:29Z'
updated_at: '2025-11-25T15:40:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

O ciclo de descoberta de dados é executado pelo menos uma vez a cada hora e verifica todas as atualizações dos boards em busca de informações relacionadas à privacidade. Isso inclui os boards que já foram verificados no ciclo de descoberta de dados anterior.

:::note
Para visualizar os resultados do descoberta de dados , você deve ter a [função de admin de conteúdo Sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, entre em contato com seu Admin da empresa.
:::

*privacy_related_dd.png
Figura 1: Resultados da descoberta de dados*

Embora estejamos trabalhando continuamente com nossos parceiros de tecnologia e clientes para melhorar o sistema de detecção de conteúdo sensível, não podemos garantir que ele encontrará e sinalizará 100% dos dados confidenciais em seus boards. Nosso sistema de detecção de conteúdo sensível usa padrões e outros critérios para determinar a probabilidade de uma correspondência. Pode haver momentos em que o sistema sinaliza incorretamente dados em seus boards como provavelmente confidenciais (um falso positivo) ou não sinaliza dados como confidenciais (um falso negativo). Vários fatores contribuem para essas ocorrências, incluindo a proximidade de termos relacionados ou a formatação de dados confidenciais.

Para obter mais informações sobre como suprimir correspondências de falsos positivos, consulte [Suprimir uma correspondência de conteúdo confidencial](11-suppress-a-sensitive-content-match.md).

## Exibir informações sobre a última verificação de descoberta de dados concluída

A seção **Resultados** da descoberta de dados exibe quando a última verificação de descoberta de dados foi concluída, representada em um Formato de data Mês, Dia, Ano e Hora:Minuto AM/PM, com um formato de hora de especificação de fuso horário (GMT+deslocamento). Por exemplo, 14 de dezembro de 2023, 22h15 GMT+1 (Figura 1).

## Exibir resultados da descoberta de dados

A seção **Resultados** da descoberta de dados exibe informações, como o nome do regulamento, uma breve descrição, o etiqueta associado e a contagem de boards contendo conteúdo potencialmente sensível que pode estar sob o escopo do regulamento (Figura 1).

Para explorar os boards com dados confidenciais, clique no link de contagem de board . O buscador de conteúdo mostra a lista de boards. Para obter mais informações, consulte [boards de revisão com dados confidenciais](16-review-boards-with-privacy-related-information.md).
