---
title: Configurar as integrações do Microsoft e do Power BI
article_id: 25132703621394
translation_id: 25132703621394
locale: pt-br
sidebar_position: 3
created_at: '2025-03-06T10:27:14Z'
updated_at: '2025-11-25T15:49:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
availability:
  notes: Para obter documentos administrativos abrangentes especificamente sobre a
    integração da Miro com a Microsoft ou Power BI, incluindo diagramas detalhados
    e perguntas frequentes adicionais, consulte a [documentação administrativa da
    Microsoft](https://docs.google.com/document/d/1Gw94z5Pc-elS-pRXKGZVBWKKNEIFR9y9yzAAkbXKwMM/edit?usp=sharing)
    ou a [documentação administrativa do Power BI](https://docs.google.com/document/d/1hMepF163jQF8LI-U8ES8DzHVMW4TltXDr14fJ2KU29k/edit?tab=t.0#heading=h.gu9ng058yy7y).
---

Este artigo explica como configurar uma integração da Microsoft ou Power BI com a Miro.

## Configurar uma integração do Microsoft ou Power BI

Para configurar uma integração com o Microsoft ou Power BI, você deve habilitar os usuários a autorizarem seus próprios conteúdos do Microsoft ou Power BI na Miro.

### Pré-requisitos

- Verifique se você tem acesso de admin ao Microsoft Entra.
- Um Admin da empresa aprovou o Microsoft ou Power BI para sua organização na Miro (isso se refere às políticas de aprovação de apps do lado da Miro, caso sua organização restrinja instalações de apps).

### Procedimento

Estas etapas concentram-se em configurar o Microsoft Entra para permitir a integração da Miro.

1. Faça login no **Entra** como admin.
2. Vá para **Aplicativos empresariais** > **Consentimento e permissões**.
3. Para **os usuários poderem solicitar o consentimento do admin para aplicativos aos quais não conseguem consentir**, selecione **Sim**.
4. Em **Quem pode revisar solicitações de consentimento de admin**, escolha os usuários, funções ou grupos necessários que você deseja autorizar para revisar as solicitações de consentimento de admin para aplicativos.

:::note
Os administradores do Entra designados no Passo 4 acima podem então ir para **Aplicativos empresariais > Solicitações de consentimento do administrador** no Microsoft Entra para revisar e aprovar o aplicativo "Contenthub PowerBI Integratio" (ou um nome similar) para a organização.
:::

## Valide sua integração do Microsoft ou PowerBI

Copie e cole um link para o seu board da Miro.

Se o aplicativo for pré-aprovado pelo Admin da empresa, siga as instruções no modal na tela. A Miro adiciona o conteúdo do seu aplicativo ao board como um iFrame.

Se o aplicativo não for pré-aprovado, o modal **Adicionar e permitir** será aberto e permitirá que você envie uma solicitação ao Admin da empresa. Enviar sua solicitação.

Quando o Admin da empresa responder, você receberá uma notificação.

**Mais informações:** Veja [Gerenciamento do aplicativo](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).
