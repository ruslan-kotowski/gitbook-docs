---
title: Autenticação em dois fatores (2FA) Enterprise – guia do admin
article_id: 7935391125394
translation_id: 7935391125394
locale: pt-br
sidebar_position: 1
created_at: '2022-10-04T08:57:18Z'
updated_at: '2026-01-13T13:35:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Relevante para: Enterprise Plan Configurado por: Admins da empresa'
---

## Autenticação em dois fatores (2FA) para organizações

2FA adiciona uma camada extra de segurança a perfis online, indo além de apenas nome de usuário e senha. Os Admins da empresa Enterprise podem exigir uma prova adicional de identidade quando os usuários acessarem a assinatura da Miro de sua organização. Este requisito é aplicável para todos os logins utilizando e-mail e senha.

Para empresas que utilizam logon único, a 2FA inclui apenas colaboradores externos que não usam SSO. Para empresas que não usam logon único, a 2FA se estende a todos os usuários.

:::note
Este artigo explica a autenticação em dois fatores (2FA) para planos Enterprise. Para todos os outros planos, consulte [Autenticação em dois fatores (2FA)](../../../administration/security-compliance/01-two-factor-authentication-2fa.md) em Administração.
:::

## Configuração de 2FA obrigatória para sua organização

:::note
Antes de ativar a autenticação em dois fatores (2FA), é importante informar todos os usuários impactados, incluindo membros da sua organização e colaboradores externos. Para garantir uma transição tranquila, sugerimos compartilhar nosso [guia do usuário de 2FA](../../security-integrations/two-factor-authentication-2fa/02-enterprise-two-factor-authentication-2fa-–-user-guide.md) para auxiliá-los nesse processo.
:::

## Como habilitar a 2FA para seus usuários

1. Vá para a console de admin > **Segurança** > **Autenticação**.
2. Ative **Exigir autenticação em dois fatores para usuários sem logon único**.

![2FA-enable.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277317394_2FA-enable.png)*Implementando autenticação em dois fatores para usuários sem logon único*

### Confiança em dispositivos de autenticação em dois fatores

Quando ativada, uma caixa de seleção será exibida para os seus usuários de autenticação em dois fatores, permitindo que eles pulem a autenticação em dois fatores cada vez que iniciarem sessão nesse dispositivo pelos próximos X dias, onde "X" é o período estabelecido pelo administrador. Você pode permitir que os dispositivos dos usuários sejam confiáveis por 7 a 90 dias. Por padrão, a funcionalidade de confiar nos dispositivos de autenticação em dois fatores está ativada, embora você possa desabilitá-la no seu console de admin.

![2FA-trusted-devices.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277323410_2FA-trusted-devices.png)

:::warning
Se a confiança nos dispositivos de autenticação em dois fatores estiver desativada, os usuários terão que inserir um código de autenticação em dois fatores em cada início de sessão. Isso tornará a experiência de login mais lenta.
:::

A autenticação em dois fatores será necessária novamente após o término do período confiável.

A autenticação em dois fatores não será ignorada se os usuários iniciarem sessão em um novo dispositivo ou navegador, ou se limparem os cookies do navegador.

## Redefinindo a autenticação em dois fatores para os usuários

Se um usuário perde o acesso ao seu método de autenticação em dois fatores, os admins podem redefinir sua autenticação em dois fatores. Assim que o usuário solicita a redefinição do método de autenticação em dois fatores, o admin responsável receberá uma notificação por e-mail.

:::note
Os admins podem redefinir a autenticação em dois fatores apenas para usuários cujos domínios de e-mail estão verificados em sua organização, se o admin iniciar a redefinição. Se o usuário solicitar a redefinição, qualquer admin na organização pode aprová-la.
:::

Para redefinir o método de autenticação em dois fatores do usuário:

1. Vá para o **console de admin** > guia **Usuários** > guia **Usuários ativos**.
2. Encontre o usuário que precisa ter seu método de autenticação em dois fatores redefinido.
3. Clique no ícone de **três pontos** (**...**) na linha do usuário.
   ![reset-2fa.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24650686629138_reset-2fa.png)
   *Redefinindo a autenticação em dois fatores no console de admin*
4. Clique em **Redefinir autenticação em dois fatores**.
   Um diálogo será aberto solicitando confirmação.
5. Clique no botão **Redefinir 2FA** no diálogo.
6. Uma mensagem de confirmação aparecerá no topo da sua tela confirmando que as instruções de redefinição foram enviadas ao usuário.

## Impacto na experiência do usuário

- Usuários sem logon único serão instruídos a configurar seu segundo fator durante o próximo login. Este processo não os desconectará de sessões em andamento.
- Os usuários precisam configurar a autenticação em dois fatores (2FA) usando seu dispositivo móvel juntamente com um aplicativo de senha única baseada no tempo (TOTP), como o Microsoft Authenticator, Google Authenticator ou Authy.
- Para os usuários que utilizam a autenticação em dois fatores, há um limite de 3 tentativas para inserir um código TOTP válido. Se este limite for ultrapassado, será necessário iniciar novamente o processo de autenticação.
- Embora o login com 2FA esteja disponível em aplicativos móveis e para tablets, o processo de registro inicial é suportado exclusivamente em aplicativos de navegador e desktop.

## Importante saber

A aplicação da autenticação em dois fatores se aplica somente a *usuários que se autenticam com e-mail e senha ou via links mágicos (enviados por e-mail)*.

- 2FA não está ativado para colaboradores externos que se autenticam usando logon único.
- Se um colaborador externo da sua organização Enterprise já está se autenticando usando logon único de sua organização de origem, ele continuará a acessar todos os times e boards na Miro usando logon único.
- Quando um usuário se autentica por meio de uma integração de login de terceiros (por exemplo, Google, Microsoft, Slack), ele manterá o acesso a todos os times e boards da Miro através desse método de login. Os admins têm a opção de encorajar esses usuários a configurar um segundo fator dentro de sua respectiva integração de login. No entanto, o fluxo de autenticação da Miro não irá solicitar que esses usuários configurem um segundo fator.

## Logs de auditoria

Admins podem rastrear usuários que configuraram a autenticação em dois fatores, juntamente com sucessos e falhas de login em dois fatores, com os seguintes eventos de log de auditoria:

- `mfa_setup_succeeded` - se um usuário configurou com sucesso seu segundo fator
- Atualização para o evento `sign_in_succeeded` para incluir o atributo MfaFactorType se um login bem-sucedido for completado com 2FA
- Atualização para o evento `sign_in_failed` para incluir o atributo MfaFactorType se um login com 2FA não foi bem-sucedido devido ao usuário exceder o número máximo de tentativas (falha não técnica)
