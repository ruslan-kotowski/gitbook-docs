---
title: Conector Miro para fluxos de trabalho Okta
article_id: 8264504421394
translation_id: 8264504421394
locale: pt-br
sidebar_position: 1
created_at: '2022-10-25T14:04:07Z'
updated_at: '2025-02-26T12:20:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Configure o Miro Connector para Okta Workflows para usar o Miro admin Connector no painel do Okta Workflow.

Leia mais sobre o admin Connector e o User Connector em [Configurar automação de fluxo de trabalho para fluxos de trabalho do Okta](03-set-up-miro-connectors-for-okta-workflows.md).

> **Disponível para:** Plano Enterprise
> **Quem pode fazer isso:** Admins da empresa

## Configurar as configurações no Miro

### Gerar um token de acesso

1. Na página de configurações do Miro Enterprise , acesse **Aplicativos e integrações** > **Integrações Enterprise**e role para baixo até **Fluxos de trabalho do Okta**.

2. Para habilitar **os fluxos de trabalho do Okta**, clique no botão correspondente.

![okta-workflows-turn-on.png](images/24938326404498_okta-workflows-turn-on.png)
*Configurações de integrações do Okta Workflows no Miro Enterprise*

3. Para copiar o token de acesso, clique em **Copiar**.

4. Para gerar um novo token de acesso, clique em **Gerar novo token**.

![okta-workflows-enablement.png](images/24938289083282_okta-workflows-enablement.png)
*Token de acesso*

:::warning
Se a alternância já tiver sido habilitada por outro Admin da empresa, você não poderá copiar o token. Você só pode desabilitar a integração.
:::

:::warning
A integração será vinculada ao time com o maior número de usuários. Não é possível escolher um time diferente. No entanto, a integração funcionará para todas as times do seu plano Enterprise , e os eventos relevantes à integração serão exibidos para todo o plano nos seus logs de auditoria.
:::

## Configurar as configurações no Okta Workflows

### Criar uma nova conexão

1. No painel do Okta Workflows, vá para **Conexões**.

2. Clique no botão **+ Nova conexão** .

3. Na caixa de diálogo **Nova conexão** , selecione o conector **Miro admin** .

![Conector](images/21019735562258_Miro-Administrator-connection.png)
*de administração Miro*

4. Cole seu **ID da organização** e seu **token de acesso** nos campos de entrada correspondentes na caixa de diálogo.

5. Clique em **Criar**.

![Paste-org-ID-and-access-token-click-create.png](images/21019735565842_Paste-org-ID-and-access-token-click-create.png)
*Criando um novo conector*

6. Depois de estabelecer a conexão recém-criada, você pode começar a criar fluxos de trabalho do Okta.
