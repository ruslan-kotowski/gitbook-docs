---
title: Gerenciamento de ativos de software com Productiv
article_id: 4403963598226
translation_id: 4403963598226
locale: pt-br
sidebar_position: 2
created_at: '2021-07-19T15:14:00Z'
updated_at: '2026-01-09T13:02:45Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Analise e personalize o uso da sua assinatura em escala com a ajuda da integração Productiv e Miro . A integração permite obter a lista de usuários não ativos e desativá-los do aplicativo de gerenciamento de ativos.

> **Disponível para:** [Plano Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configurado por:** Admins da empresa

## Funcionalidades compatíveis

A integração dá acesso aos seguintes recursos:

- **Baixar assinaturas**
  - Obtenha uma lista do uso da assinatura do usuário e o número de licenças alocadas na sua assinatura do Miro Enterprise .
- **Reivindicar assinaturas**
  - Desative usuários no seu plano Miro Enterprise com base no uso da assinatura .

O Productiv fornece uso de recursos em tempo real até o nível da equipe.

![Miro_usage_info.jpg](../../../../../../../docs/enterprise-administration/enterprise-subscription-management/software-asset-management/images/21017695874578_Miro%20usage%20info.jpg)
*Informações de uso do Miro no Productiv*

## Etapas de configuração

:::note
Consulte as etapas de configuração na documentação do Productiv - [Conectar Miro](https://docs.app.productiv.com/onboarding/connectors/miro/index.html?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9kb2NzLmFwcC5wcm9kdWN0aXYuY29tL29uYm9hcmRpbmcvY29ubmVjdG9ycy8qIiwiQ29uZGl0aW9uIjp7IkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNzQyMzEzOTExfX19XX0_&Key-Pair-Id=APKAIYWO2HKDBSFULS4Q&Signature=EmSlxzMWt8s4ro~r6bsh4~5DdxVm4stcuZTaK0CsQetFeruzXAkMzXzKxOwJquamG~l8LPnL4EHIAYwWrNm3v4mX72s6tWLDl6x5QaxwZ-mvEh8eiNbzGKR13UQojdihneT1h619mN0CPcMKJibC2cDO~fy6KmLrJOryN4BZD-5vCA-7dKuN0YUtgZ1FByJnP3ltS-DLV4gkdGNJZ8bPGZY61s0JtP4CAyObJTF9R2WnchD7RAg4OsVq6XHXf1~zOAHpth3v~lE3YI5nWzFuQh8DIp59UHNHLc-fdIrRkPH5qCb~y4tGZLC16atXJS7C8ZWcN7rh7AjXCvsVwH8zkg__).
:::

Para copiar o token de acesso no lado do Miro , no console de admin , vá para **Aplicativos e integrações** > **Integrações Enterprise** e role para baixo até **SAM**.

![Configuração do SAM no console de admin do Enterprise](../../../../../../../docs/enterprise-administration/enterprise-subscription-management/software-asset-management/images/23921803379090_image.png)*Configuração do SAM no console de admin do Enterprise*

Depois de habilitar a alternância, você pode copiar o token de acesso ou gerar um novo.

:::note
Se a alternância tiver sido habilitada por outro admin, você não terá a opção de copiar o token. Uma mensagem indica qual admin habilitou o SAM e como contatá-lo.
:::

Para desativar o SAM, coloque **-o** na posição desligado.
