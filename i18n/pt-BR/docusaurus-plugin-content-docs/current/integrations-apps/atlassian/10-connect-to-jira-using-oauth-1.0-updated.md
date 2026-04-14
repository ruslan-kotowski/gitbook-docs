---
title: Conectar ao Jira usando OAuth 1.0 (Atualizado)
article_id: 27689156602514
translation_id: 27689199867410
locale: pt-br
sidebar_position: 12
created_at: '2025-06-27T13:20:27Z'
updated_at: '2025-11-25T15:52:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quem pode fazer: Admins da empresa, Admins de times Quais planos: Starter,
    Business, Enterprise, Education Quais plataformas: Navegador, Desktop'
---

Organizações que não estão prontas para migrar para OAuth 2.0 podem usar o seguinte procedimento para conectar Miro ao Jira usando OAuth 1.0.

A Atlassian [declarou OAuth 1.0 como obsoleto](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively), e o método fornecido neste artigo é uma solução provisória. Para evitar problemas e alinhar-se às melhores práticas de segurança e compatibilidade, Miro recomenda fortemente que você migre para OAuth 2.0 o quanto antes.

:::note
O método anterior de autenticação OAuth 1.0 [é obsoleto](https://help.miro.com/hc/articles/360019501754-Set-up-and-disable-Jira-Cards-OAuth-1-0) e será removido em 31 de julho de 2025.
:::

Este artigo também explica como usar uma instância do Jira para vários times da Miro e como desabilitar os cartões do Jira no nível da organização e do time.

## Pré-requisitos

- Você deve ter as seguintes permissões:
  - (Business, Enterprise) admin da empresa Miro
    (Starter, Education) admin do time Miro
  - Admin do sistema Jira

    > ✏️ Para completar o procedimento, você deve ser capaz de criar um link de aplicação no Jira.
- No Jira, remova todos os links de aplicação existentes para o Miro.

## Procedimento

Para se conectar ao Jira usando OAuth 1.0, siga estas etapas:

1. No seu painel da Miro, selecione seu avatar no canto superior direito e clique em **Console de Admin**.
2. Na barra lateral à esquerda, vá para **Apps e integrações** > **Apps** > guia **Gerenciar apps**.
3. Verifique se **Permitir somente aplicativos da lista abaixo** está habilitado.
4. Na coluna **App**, para **Cartões do Jira**, selecione **Configurações**.
5. Na guia **Configurações padrão**, selecione **Adicionar nova conexão**.
6. Em **Configuração do Jira**, selecione **Jira Cloud** ou **Jira Data Center**.
7. Em **Método de autenticação**, selecione **OAuth 1.0x (Atualizado)**.
8. Em **URL do Jira**, insira o URL da sua instância do Jira.
9. (Opcional) Para tornar esta conexão a conexão padrão para todos os times na sua organização, marque **Definir como padrão**.
10. Em **Instruções de configuração**, verifique se você possui as seguintes propriedades:
    - URL
    - Chave do consumidor
    - Nome do consumidor
    - Chave pública
11. No Jira, crie um link de aplicação.
    1. (Cloud) Vá para **Configurações** > **Produtos** > **Links de Aplicação**.
       (Data Center) Nas configurações de admin do Jira, vá para **Produtos** > **Links de Aplicação**.
    2. Clique em **Criar link**.
    3. (Cloud) Para **Tipo de aplicação**, selecione **Aplicação direta**.
       (Data Center) Para **Tipo de aplicação**, selecione **Produto Atlassian**.
    4. Para **URL da Aplicação**, cole a URL das instruções de configuração do Miro. Veja o passo 10.
    5. Clique em **Continuar**.
    6. Para **Nome da aplicação**, nomeie sua aplicação.

       > **⚠️** Não insira dados em nenhum outro campo. Você fornecerá os dados do Miro em um passo seguinte.
    7. Marque **Criar link de entrada**.
    8. Clique em **Continuar**.
    9. Copie e cole seu Consumer key, Consumer name e Public key das instruções de configuração do Miro. Veja o passo 10.
    10. Clique em **Continuar**.
        Você criou seu link de aplicação.
12. No Miro, clique em **Conectar**.
    Você conectou o Miro ao Jira usando OAuth 1.0.

## E depois?

Você configurou e conectou sua integração do Jira com a Miro usando o Jira OAuth1.0. Na primeira vez que um usuário tenta uma ação relacionada ao Jira na Miro, ele é solicitado a autenticar-se.

**Mais informações:** Veja [Como usar cartões do Jira](https://help.miro.com/hc/articles/360017572434).

## Uma instância do Jira para vários times da Miro

Você pode instalar cartões do Jira no nível da organização ou no nível do time. Se você tiver vários times, pode especificar configurações no nível da organização para evitar configurações repetitivas para cada time. O link de aplicação existente é então usado para todos os times.

:::note
Conectar várias instâncias do Jira a um único time da Miro não é suportado.
:::

Para solicitações de atualização, após conectar sua organização ou time a uma instância do Jira, um webhook é adicionado aos seus webhooks do Jira para aquela organização ou time do Miro.

:::tip
Dê um nome único a cada webhook por time. Vá à sua página WebHooks no Jira e edite cada novo webhook criado.
:::

Se você especificar configurações a nível da organização, os times que já possuem suas próprias configurações de time mantêm sua configuração. Qualquer time com sua própria configuração pode mudar para as configurações a nível da organização a qualquer momento.

Por outro lado, qualquer time pode substituir as configurações a nível da organização para se conectar a uma instância separada do Jira.

## Desabilitar cartões do Jira

### Nível da organização

Para desabilitar cartões do Jira a nível da organização, siga estas etapas:

1. No seu painel da Miro, clique no seu avatar no canto superior direito e clique em **Console de Admin**.
2. Vá para **Aplicativos e Integrações** > **Gerenciar aplicativos**.
3. Localize **Cartões do Jira**.
4. Para os cartões do Jira, altere a chave **Permitido** para a posição desligada.

:::warning
Se você desabilitar os cartões do Jira para a organização, todos os membros dos times Enterprise não poderão usar os cartões do Jira. Para saber mais sobre a gestão de aplicativos, consulte [Gestão de aplicativos](https://help.miro.com/hc/articles/4404659741458).
:::

### Nível do time

Para desabilitar os cartões do Jira no nível do time, siga estas etapas:

1. No seu painel da Miro, clique no seu avatar no canto superior direito e clique em **Console de admin**.
2. Vá para **Times**.
3. Clique na linha do time que você deseja gerenciar.
   O painel de configurações do time é aberto.
4. Clique na guia **Apps**.
5. Localize e clique em **Cartões Jira**.
6. Clique em **Remover para o time**.
