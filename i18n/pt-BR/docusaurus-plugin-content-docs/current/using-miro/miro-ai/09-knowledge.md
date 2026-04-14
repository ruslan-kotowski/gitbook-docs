---
title: Conhecimento
article_id: 29737566936850
translation_id: 29737566936850
locale: pt-br
sidebar_position: 9
created_at: '2025-09-25T08:24:51Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: sticky-notes
availability:
  notes: 'Quem pode fazer isso: Membros do time Quais planos: Business, Enterprise
    Quais plataformas: Navegador, Desktop, Mobile'
---

O Conhecimento na Miro integra-se com provedores como Glean, Microsoft Copilot (Beta) e Miro Insights, para tornar o conhecimento da sua empresa acessível e acionável diretamente no canvas.

O Conhecimento permite que os times recuperem informações internas e resultados de pesquisas na web de forma integrada, usando o canvas da Miro como prompt para um desenvolvimento mais rápido.

Conecte sistemas de conhecimento que você já utiliza, e depois converta facilmente o que sua empresa sabe em Formatos como Documentos, Tabelas, Notas adesivas e Slides.

O Conhecimento suporta as seguintes integrações, incluindo pesquisa na web.

- [Amazon Q](../../integrations-apps/amazon-web-services-aws/03-amazon-q-beta.md) (Beta)
- [Gemini Enterprise](../../integrations-apps/google/01-gemini-enterprise-integration.md) (Beta)
- [Glean](../../integrations-apps/glean/01-glean-for-miro.md)
- [Microsoft Copilot](../../integrations-apps/microsoft/01-microsoft-copilot-integration.md) (Beta)
- [Miro Insights](../tools/use-miro-insights/02-use-miro-insights-on-the-canvas.md)

Os admins da empresa devem ativar e aprovar cada integração para seus times.

:::note
Algumas integrações, como Microsoft Copilot e Gemini Enterprise, requerem licenças pagas com o respectivo fornecedor.
:::

Para saber mais sobre integrações específicas de conhecimento, veja [Integrações e Aplicativos](../../integrations-apps).

## Principais funcionalidades

- **Integrações de conhecimento**
  Knowledge conecta a Miro a provedores líderes como [Glean](../../integrations-apps/glean/01-glean-for-miro.md), [Microsoft Copilot](../../integrations-apps/microsoft/01-microsoft-copilot-integration.md) (Beta), [Amazon Q](../../integrations-apps/amazon-web-services-aws/03-amazon-q-beta.md) (Beta) e Miro Insights, permitindo que você recupere e aplique o conhecimento da sua empresa diretamente no canvas.
- **Conhecimento corporativo como prompt**
  Utilize o conhecimento recuperado como contexto para o prompt do [Miro AI](01-miro-ai-overview.md) e avance da ideação para a criação mais rapidamente.
- **Múltiplos pontos de acesso**
  A funcionalidade de Conhecimento está disponível em diversos pontos de entrada na Miro, como [Assistente de IA](07-sidekicks.md) e [fluxos](04-flows-overview.md), garantindo que você especifique o conteúdo mais relevante para uma determinada etapa do seu fluxo de trabalho.

:::note
Os admins podem gerenciar permissões de Conhecimento e do Miro AI, capacidades de busca na web, e criação de Formatos para garantir conformidade com as políticas da organização.
:::

## Use Conhecimento para recuperar informações da empresa

Acesse o Conhecimento em qualquer um dos seguintes pontos de entrada.

:::note
Ao conectar um provedor de conhecimento pela primeira vez, será solicitado que você autentique.
:::

- [**Assistentes de IA**](06-sidekicks-overview.md)
  Acima da barra de Criação, clique em **Assistentes de IA**. O painel do **Assistente de IA** será aberto. Na caixa de prompt, clique em **Conhecimento**. Conecte ou ative um provedor de conhecimento na posição ligada.
  ![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)*No painel do Assistente de IA, selecione um provedor de conhecimento para recuperar conhecimento da empresa no Miro.*
  Escreva seu prompt de Assistente de IA. Você pode, opcionalmente, selecionar objetos no canvas para adicionar contexto. Ao executar seu prompt, o Conhecimento utiliza o(s) provedor(es) que você selecionou.

  > 💡 Use o Conhecimento para criar Assistentes de IA especializados que ajudam você com tarefas no canvas como agentes personalizados de IA.
- [**Docs**](04-flows-overview.md) **em Fluxos**
  No menu de contexto do Doc, clique em **Editar com IA**. O painel do **Assistente de IA** será aberto. Na caixa de prompt, clique em **Conhecimento**. Conecte ou selecione um fornecedor de conhecimento. Quando você executa seu prompt, o Conhecimento utiliza o fornecedor que você selecionou.
- [**Bloco de instrução de IA**](05-flows.md) **em fluxos**
  No bloco de instrução de IA, clique em **Selecionar base de conhecimento.** Conecte ou selecione um provedor de conhecimento. Quando você executar sua instrução de IA, o recurso de conhecimento usará o provedor que você selecionou.
- **Chat independente**
  Você pode acessar os recursos de Conhecimento no aplicativo de chat independente da Miro.
  - Acima da barra de Criação, clique em **Assistentes de IA**. O painel de **Assistente de IA** se abre. Acima de **Oi \{Seu nome\}**, clique na seta para baixo, e depois clique em **Explorar mais Assistentes de IA**. Clique na guia **Conhecimento**.
  - Na barra de Criação, selecione **Ferramentas, Mídia e Integrações**. Procure e selecione seu provedor de Conhecimento. Por exemplo, **Gemini**.O painel de chat se abre.
