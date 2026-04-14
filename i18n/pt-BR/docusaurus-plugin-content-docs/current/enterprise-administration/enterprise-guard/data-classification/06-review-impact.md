---
title: Revisar impacto
article_id: 16594793714066
translation_id: 16594793714066
locale: pt-br
sidebar_position: 5
created_at: '2024-01-24T19:34:48Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
id: 06-review-impact
---

Esta é a última etapa do fluxo de configuração de classificação automática e guardrails. Nesta etapa do fluxo, você deve revisar o impacto das atualizações de configuração de classificação ou de guardrails. Nesta etapa do fluxo, você deve revisar o impacto das alterações que está fazendo na classificação ou na configuração de guardrails. As seções a seguir descrevem as informações disponíveis na página de impacto da revisão e várias ações que você pode tomar.

## Distribuição dos níveis de classificação

Esta seção permite que você analise o impacto da sua configuração atualizada em termos de alterações para cada nível de classificação da board .

A seção **Distribuição de níveis de classificação** é recolhível, melhorando sua capacidade de rolar pela lista de atualizações com mais eficiência (veja a Figura 1).

![Seção de distribuição de níveis de classificação recolhível](images/24937306596498_Collapsible_Distribution_of_classification.png)

*Figura 1: Seção de distribuição de níveis de classificação recolhível*
A interface de usuário baseada em colunas simplifica o processo de comparação e revisão de atualizações de classificação do board . Fornecemos colunas distintas que exibem o número de boards adicionadas, o número de boards removidas e o total atualizado para cada nível de classificação (Figura 2).

![Interface de usuário baseada em colunas exibindo o número de boards adicionadas, o número de boards removidas e o total atualizado para cada nível de classificação](images/24937306599186_columnview.png)

*Figura 2: Interface de usuário baseada em colunas exibindo o número de boards adicionadas, o número de boards removidas e o total atualizado para cada nível de classificação*

O recurso de detalhamento oferece uma visualizar abrangente (Figura 3) dos seguintes detalhes:
- Rótulos de classificação automática adicionados ou removidos.
- Guarda-corpos adicionados ou removidos.
- Número de boards que mudaram para um nível de classificação específico.
- Número de boards não afetadas pelas alterações de configuração que você fez.

![Recurso de detalhamento com visualizar abrangente das atualizações](images/24937299427602_drilldown_feature_classification.png)

*Figura 3: Recurso de detalhamento com visualizar abrangente das atualizações*

## Impacto das proteções

Esta seção exibe os guardrails que serão aplicados com base no nível de classificação do board e o número total de boards que terão cada guardrail específico. O número entre parênteses indica o número de boards para as quais o guardrail é adicionado ou removido após a publicação da nova configuração. Além disso, esta seção também exibe o número de boards que não são classificadas (Figura 4).

Para atualizar a configuração dos guardrails, clique em **Anterior**.
*![Configurar classificação Revisar impacto](images/24937299430802_guardrails.png)
Figura 4: Configurar classificação > Revisar impacto*

## Atualizar a configuração dos guardrails

Para fazer atualizações após revisar o impacto das atualizações feitas na configuração de classificação automática e guardrails, clique no botão **Anterior** , faça as atualizações na configuração e revise o impacto mais uma vez.

## Publicar configuração

Depois de revisar o impacto da classificação ou configuração de guardrails que você fez, clique em **Publicar**.

:::note
Observações:
- A configuração do nível de classificação é aplicada imediatamente.
- A configuração dos guardrails é aplicada imediatamente.
- Quando novos boards são adicionados com dados confidenciais, esses boards são classificados automaticamente após a conclusão do próximo ciclo de descoberta de dados .
- Quando o conteúdo do board é atualizado (remoção ou adição de conteúdo sensível), esses boards são classificados automaticamente após a conclusão do próximo ciclo de descoberta de dados .
:::
