---
title: Conectar ao Jira on-premise com servidores de autorização de terceiros usando
  OAuth2.0
article_id: 25692796700306
translation_id: 26751283171602
locale: pt-br
sidebar_position: 9
created_at: '2025-05-16T09:13:56Z'
updated_at: '2025-11-25T15:50:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quem pode fazer isso: Admins da empresa Quais planos: Enterprise'
---

> *✏️* Conectar o Jira usando um servidor de autorização só é habilitado no nível da organização.

Este artigo fornece as etapas para conectar Miro ao Jira com um servidor de autorização de terceiros, no local, usando OAuth2.0.

Para aprender os detalhes técnicos sobre esta configuração, consulte o artigo de referência para [Jira on-premise com autorização de terceiros usando OAuth 2.0](https://help.miro.com/hc/articles/26726425696530).

## Pré-requisitos

- Verifique se você tem as seguintes permissões:
  - Admin da empresa Miro
  - (Opcional) Admin do sistema Jira, se você quiser usar webhooks automáticos.
- No seu servidor de autorização, crie um app OAuth 2.0.
- Configurar o URL de redirecionamento no seu aplicativo OAuth 2.0 para o seguinte URL:
  https://integrations.miro.com/api/external-auth/oauth2/callback
- Certifique-se de ter os seguintes detalhes do seu aplicativo OAuth 2.0 prontos para configurar na Miro:
  - URL de autorização
  - URL do token
  - ID do cliente
  - Segredo do cliente
  - Escopo

## Conectar-se ao Jira local com servidores de terceiros usando OAuth 2.0

1. No seu painel da Miro, selecione seu avatar no canto superior direito e vá para **admin console** | **Configurações**.
2. Vá para **Aplicativos e integrações ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)**> **Aplicativos** > **Guia Gerenciar aplicativos** .
3. Certifique-se de que **Permitir apenas aplicativos da lista abaixo** esteja habilitado.
4. Na coluna **App**, para **cartões do Jira** selecione **Configurações**.
5. Clique em **Adicionar nova conexão**.
6. Em **configuração do Jira**, clique em **Jira Data Center**.
7. Em **Método de autenticação**, selecione **OAuth 2.0 via Servidor de Autorização de Terceiros**.
8. No campo **Jira URL**, insira o URL da sua instância do Jira.
   > *✏️* Você pode adicionar seu URL base externo do Jira ou seu URL interno do Jira. Se você usar uma URL interna do Jira, então deve especificar o URL do seu gateway de API externo na etapa 10.

   > *✏️* Em geral, usar uma URL interna permite ajustar a funcionalidade de navegação para a fonte.
9. (Opcional) Para tornar esta conexão a conexão padrão para todos os times da sua organização, marque **Tornar Padrão**.
10. (Opcional) Se você usar um gateway de API para fazer solicitações ao Jira, então para **URL base do Jira API Gateway**, insira seu URL de gateway de API externo.
11. Insira os seguintes detalhes do seu aplicativo OAuth 2.0:
    - URL de autorização
    - URL do token
    - ID do cliente
    - Segredo do cliente
    - Escopo
12. (Opcional) Para receber atualizações em tempo real do Jira na Miro, marque **Criar webhook automaticamente**.
    > *✏️ Você pode adicionar o webhook manualmente depois.*
13. Clique em **Conectar**.
14. Siga o fluxo de autenticação para o seu servidor de autorização. Se solicitado, faça login no seu ambiente.
    Quando sua conexão é concluída, sua instância do Jira é listada em **Instâncias conectadas** com a seguinte tag: **Servidor de autenticação**.

## Garanta que seu time possa se autenticar

Agora que você conectou sua instância do Jira no nível da organização, pode começar a usar o Jira no nível do time.

1. No seu painel da Miro, selecione seu avatar no canto superior direito e vá para **Console de Admin**.
2. Selecione **Times** > **Seu time**.
   O controle deslizante do **seu time** abre.
3. Selecione a guia **Apps**.
4. Na lista de aplicativos, selecione **cartões do Jira**.
5. Em **Configurações do admin**, verifique se sua configuração do Jira mostra a etiqueta **GLOBAL CONNECTION** e exibe a URL correta da instância do Jira. Em seguida, faça um dos seguintes:
   - Se sim, você completou este procedimento. Você pode pular para [E agora?](https://help.miro.com/hc/articles/25699264170386)
   - Se não, selecione **Alterar configuração** > **Configurações da organização global** > **sua instância do Jira**.
6. Selecione **Salvar configurações**.

## O que vem a seguir?

Cada membro do time deve autorizar sua conta de usuário. Para garantir que cada usuário obtenha tokens de acesso e atualização, quando um membro do time tentar uma ação relacionada ao Jira em um board da Miro, será solicitado que autorizem sua conta.

## Perguntas frequentes

**Quais servidores de autorização posso usar?**

Você pode usar qualquer servidor de autorização que suporte os protocolos padrão do OAuth 2.0 para ambientes locais. Por exemplo, Azure Active Directory (Entra ID) e Okta.

**Posso usar o mesmo servidor de autorização para várias organizações?**

Sim, mas você deve adicionar manualmente o servidor a cada organização.

**Posso atualizar o segredo do cliente para um servidor de autorização?**

Não. Se você precisar alterar o segredo do cliente, então você deve desconectar e reconectar sua instância.

**Os admins da organização e do time ainda podem usar a autorização nativa no Jira?**

Sim. Dependendo da configuração selecionada, os admins podem continuar a usar o fluxo de autorização nativo no Jira.

**O que acontece se um time já estiver conectado a outra instância do Jira?**

Você pode atualizar times para as  [configurações padrão do Jira](https://help.miro.com/hc/articles/26438407676434) da sua organização.

**A Miro controla o mapeamento entre usuários autorizados e usuários do Jira?**

Não. O mapeamento entre usuários autorizados e usuários do Jira é responsabilidade do ambiente do cliente via seu gateway de API. A Miro não controla este gateway.

**Como saber se o OAuth 2.0 via um servidor de autorização de terceiros é a solução certa para a minha organização?**

Se todos os itens a seguir forem verdadeiros, então o OAuth 2.0 via servidor de autorização de terceiros é uma boa escolha:

- Sua instância do Jira está hospedada localmente.
- O acesso externo ao Jira é possível apenas com um gateway de API.
- O gateway de API aplica autorização usando um servidor de autorização personalizado.
- Você deve conectar a Miro ao Jira sem expor a URL base pública do Jira.

**Que problema esta solução resolve?**

Esta solução é projetada para organizações que hospedam Jira localmente e direcionam o tráfego de API externo por meio de um gateway de API. Nesse cenário, o Jira não é acessível publicamente, e o acesso é controlado por meio de um servidor de autorização personalizado. Em vez de ter uma URL base pública para o Jira, esta solução permite que você conecte suas instâncias locais do Jira configurando a Miro para autenticar via seu próprio servidor de autorização.
