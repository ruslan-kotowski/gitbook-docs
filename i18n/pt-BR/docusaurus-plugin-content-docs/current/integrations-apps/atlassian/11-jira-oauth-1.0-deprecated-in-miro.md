---
title: Jira OAuth 1.0 obsoleto na Miro
article_id: 28738797627538
translation_id: 28739445112210
locale: pt-br
sidebar_position: 13
created_at: '2025-08-13T12:34:35Z'
updated_at: '2025-10-20T14:49:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Pessoas: Admins da empresa Planos: Starter, Business, Enterprise, Education
    Plataformas: Browser, Desktop'
---

A autenticação Jira OAuth 1.0 estará obsoleta a partir de agosto de 2025.

Se sua organização já atualizou para o Jira OAuth 2.0, você pode ignorar este artigo. Não é necessária nenhuma ação do Admin da empresa. Você pode confirmar com seu Admin da empresa que sua organização está usando o OAuth 2.0.

:::warning
Se sua organização não atualizou para o OAuth 2.0, a integração do Jira com a Miro, incluindo Jira Cloud, Server e Data Center, pode ser interrompida.
:::

Somente os Admins da empresa podem atualizar os times em sua organização.

Em caso de interrupção, a sincronização entre a Miro e o Jira é interrompida até que sua organização atualize para a autenticação OAuth 2.0. Os cartões do Jira existentes permanecem nos seus boards da Miro.

Interrupção significa que a importação está indisponível, os cartões não são atualizados, os detalhes não podem ser carregados e a criação e atualização de um Planner estão indisponíveis.

Para evitar interrupções, a Miro recomenda que o(s) Admin(s) da empresa atualizem para o Jira OAuth 2.0 imediatamente.

:::tip
Os admins podem verificar sua versão de OAuth.
:::

## Por que o OAuth 1.0 está obsoleto?

A Atlassian declarou obsoleto e não oferece mais suporte ao protocolo de autenticação OAuth 1.0.

**Mais informações:** Veja (Externo) [OAuth 1.0a para APIs REST (Obsoleto)](https://developer.atlassian.com/cloud/jira/platform/jira-rest-api-oauth-authentication/).

## Verifique sua versão do OAuth

Como admin do time Enterprise, ou admin de plano Starter ou Business, você pode verificar se o seu time está usando OAuth 1.0 ou OAuth 2.0.

Siga estas etapas:

1. No seu painel da Miro, clique no seu avatar no canto superior direito e selecione **Console de admin**.
2. Vá para **Times** > **[Nome do time]**.
3. Clique em **Apps**.
4. Encontre e clique em **Cartões do Jira**.
5. Vá para **Configurações do admin** > **Configuração do Jira**.
   A configuração indica qual versão OAuth o seu time está usando.
6. (Opcional) Repita as etapas de 1 a 5 para outros times que você deseja verificar.
7. Notifique o(s) Admin(s) da empresa sobre quaisquer times que não estão usando OAuth 2.0.

## Encontre seu Admin da empresa

Para identificar seu(s) Admin(s) da empresa, siga estas etapas:

:::note
(Enterprise) Se a privacidade do time estiver ativada, usuários não administradores da empresa não poderão ver listas de membros.
:::

1. Vá para **Configurações do perfil do time** na Miro.
2. Abra a página de **Membros**.
3. Clique em **Funções adicionais**.
4. Encontre usuários com a função **Admin da empresa**.

:::tip
Para garantir que seu time faça o upgrade para OAuth 2.0 e evite possíveis interrupções, compartilhe este artigo com seu(s) Admin(s) da empresa.
:::

## Faça o upgrade para OAuth 2.0 para Admins da empresa

Como Admin da empresa, você tem os seguintes recursos para ajudar a atualizar sua organização para o OAuth 2.0:

- [Conectar ao Jira Cloud usando OAuth 2.0](https://help.miro.com/hc/articles/8588617184402)
- [Conectar ao Jira Data Center usando OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
- [Conectar times da organização às configurações padrão do Jira](https://help.miro.com/hc/articles/26438407676434)

## Solução intermediária

Se o OAuth 2.0 não for uma opção para sua organização agora, a Miro oferece uma [solução provisória usando OAuth 1.0](https://help.miro.com/hc/articles/27689156602514).

No entanto, a Miro recomenda atualizar para o OAuth 2.0 para garantir o método de autenticação mais seguro e preparado para o futuro, que segue os padrões atuais da Atlassian.

## Ajuda adicional

Se você ou seu Admin da empresa tiverem dúvidas, entre em contato com o [Suporte Miro](https://help.miro.com/hc/articles/360020185799).
