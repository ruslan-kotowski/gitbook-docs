---
title: "Traga sua pr\xF3pria IA (BETA)"
article_id: 21885197978642
translation_id: 21885197978642
locale: pt-br
sidebar_position: 20
created_at: '2024-10-09T18:45:40Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: ai-generate-image
---

O recurso Bring Your Own AI (BYOAI) permite que você use seu próprio provedor de IA em vez do Miro AI para alguns recursos do Miro AI .

> **Disponível para:** Enterprise
> **Disponível em:** Desktop

Você pode conectar seu provedor de IA ao Miro com BYOAI e aproveitar [recursos de IA que dependem do GPT](18-miro-ai-reference.md). Os recursos do Miro AI não suportados pelo BYOAI, como geração de imagens, podem ser desabilitados opcionalmente. Para obter mais informações, consulte Desabilitar recursos de IA não fornecidos pelo Bring Your Own AI.

Atualmente, o BYOAI oferece suporte ao OpenAI e ao Azure OpenAI.

:::note
O BYOAI suporta apenas recursos do Miro AI desenvolvidos pela GPT. Para saber quais recursos do Miro AI são alimentados pelo GPT, consulte [Visão geral do Miro AI](18-miro-ai-reference.md).
:::

## Como configurar o Bring Your Own AI

> **Disponível para:** Admins da empresa

Os procedimentos a seguir explicam como configurar o Bring Your Own AI (BYOAI) para Open AI e Azure OpenAI.

### IA aberta

Siga estas etapas:

1. Nas configurações de admin , selecione **Aplicativos e integrações**.
2. Em **Integração Enterprise**, para **Traga sua própria IA,** selecione **OpenAI**.
3. Para **a chave de API**, insira sua chave OpenAI.
   > ⚠️ Para maior segurança, copie e cole a chave da API.
4. Selecione **Conectar**.
5. Certifique-se de ter o Miro AI habilitado para sua organização.
   **Mais informações:** Consulte Habilitar Miro AI para Traga sua própria IA.

   Você configurou com sucesso o BYOAI com o OpenAI.

:::note
O Miro usa um sistema de armazenamento unidirecional para armazenar e criptografar com segurança sua chave de API, que nunca fica visível durante a entrada da chave. Nem o Miro nem os admins podem recuperar a chave da API depois que ela for atualizada e armazenada com segurança.
:::

### Azure OpenAI

Siga estas etapas:

1. Nas configurações de admin , selecione **Aplicativos e integrações**.
2. Em **Integração Enterprise**, para **Traga sua própria IA,** selecione **Azure OpenAI**.
3. Insira sua chave de API do Azure, nome da implantação e URL da implantação.
   > ⚠️ Para maior segurança, copie e cole a chave da API. Certifique-se de que a implantação esteja usando GPT-4o.
4. Selecione **Conectar**.
5. Certifique-se de ter o Miro AI habilitado para sua organização.
   **Mais informações:** Consulte Habilitar Miro AI para Traga sua própria IA.

   Você configurou com sucesso o BYOAI com o Azure OpenAI.

:::note
O Miro usa um sistema de armazenamento unidirecional para armazenar e criptografar com segurança sua chave de API, que nunca fica visível durante a entrada da chave. Nem o Miro nem os admins podem recuperar a chave da API depois que ela for atualizada e armazenada com segurança.
:::

### Habilitar Miro AI para Bring Your Own AI

Depois de conectar o Open AI ou o Azure Open AI, certifique-se de ter o Miro AI habilitado para sua organização.

Siga estas etapas:

1. Nas configurações do admin , selecione **Acesso ao recurso**.
2. Em **Ativação de recurso**, para **Miro AI,** selecione uma das seguintes opções:
   - **Todos podem usar**
   - **Times específicos podem usar**
3. (Opcional) Ative a opção **Habilitar recursos beta do Miro AI** .

   Você habilitou com sucesso o Miro AI para sua organização.

:::note
Por padrão, todos os recursos do Miro AI ficam disponíveis quando você ativa o Miro AI. Para desabilitar recursos do Miro AI não suportados pelo seu provedor de IA, entre em contato com o Suporte do Miro . Para saber mais, consulte Desabilitar recursos de IA não fornecidos pelo Bring Your Own AI.
:::

## Desabilitando recursos de IA não fornecidos pelo Bring Your Own AI

Por padrão, todos os recursos do Miro AI ficam disponíveis quando você ativa o Miro AI. O Bring Your Own AI (BYOAI) oferece suporte apenas aos recursos do LLM, que aproveitam o GPT. Para garantir que o BYOAI use apenas recursos LLM suportados pelo seu provedor de IA, você pode, opcionalmente, desabilitar recursos Miro AI não LLM.

Para desabilitar recursos não LLM do Miro AI , entre em contato com seu gerente de sucesso do cliente da Miro ou [com o Suporte da Miro](../tools/troubleshooting/06-contacting-miro-support.md).

**Mais informações:** Veja [a visão geral do Miro AI](18-miro-ai-reference.md).

## Perguntas frequentes

**Quem é responsável por criar a saída de IA quando uso BYOAI?**

Com o BYOAI, você assume o controle da geração de resultados com IA, com a qualidade definida com seu fornecedor de IA.

**Como o aproveitamento do meu próprio provedor de IA afeta a moderação de entrada?**

Com o BYOAI, o Miro não filtra o conteúdo antes que seu provedor de IA gere a saída. Se você preferir ter a moderação habilitada, confirme se a moderação de entrada foi habilitada pelo seu provedor e, em seguida, entre em contato com seu gerente de sucesso do cliente ou [com o Suporte da Miro](../tools/troubleshooting/06-contacting-miro-support.md).

**Como o BYOAI afeta o consumo de créditos de IA?**

Com o BYOAI, você consome tokens do seu próprio provedor de IA para executar os recursos do Miro AI . Você também continua consumindo créditos Miro AI . Para saber mais, consulte [Créditos Miro AI para planos Enterprise](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md).

**O que acontece se minha chave de API expirar ou eu ficar sem tokens?**

Como admin , você verá uma mensagem de erro e os usuários finais não poderão mais usar os recursos de IA fornecidos pela BYOAI.

**Como obtenho suporte se tiver problemas com a integração do meu provedor de IA?**

Entre em contato com seu gerente de sucesso do cliente ou com o suporte ao cliente. Recomendamos que você também entre em contato com seu provedor de IA.

**O Miro usará alguma entrada ou saída se eu usar BYOAI?**

Não, a entrada e saída de dados estão sujeitas ao acordo que você tem com seu provedor.
