---
title: Autenticação em dois fatores (2FA) – guia do usuário
article_id: 27601422748434
translation_id: 27601422748434
locale: pt-br
sidebar_position: 2
created_at: '2025-06-24T07:36:23Z'
updated_at: '2025-11-06T13:29:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: 'Relevante para: Starter, Business, Education, Enterprise'
---

## O que é a autenticação em dois fatores (2FA)

A autenticação em dois fatores (2FA) adiciona mais segurança às suas contas online. Quando o Admin da empresa ativa a autenticação em dois fatores (2FA), cada início de sessão na Miro usando seu e-mail e senha será seguido por uma camada extra de segurança. Esta etapa adicional garante proteção aprimorada para sua conta, exigindo verificação além de suas credenciais de login regulares.

:::tip
Aprenda como ativar a autenticação em dois fatores (2FA) para sua organização nos [planos Enterprise](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md) e em [todos os outros planos](01-two-factor-authentication-2fa.md).
:::

## Como configurar a autenticação em dois fatores (2FA)

**Novos usuários:** Durante o seu [processo de criação de conta](https://miro.com/signup/) com o e-mail da sua empresa, você será solicitado a habilitar a autenticação em dois fatores (2FA).
**Usuários existentes:** No seu próximo [início de sessão](https://miro.com/login/), se sua organização exigir 2FA e você não estiver usando o logon único (SSO), será solicitado a configurar a autenticação em dois fatores (2FA).

1. Baixe um aplicativo autenticador no seu dispositivo móvel. Aplicativos autenticadores, como Google Authenticator, Microsoft Authenticator e Authy, geram um código de uso único baseado em tempo (TOTP) para logins seguros na Miro. Para obter orientação sobre qual aplicativo autenticador escolher, pergunte ao Admin da empresa ou ao admin de TI.

2. Clique em **Eu tenho um aplicativo autenticador** na tela de configuração de 2FA da Miro.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../docs/administration/security-compliance/images/27601397095698_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *Confirmação do download do aplicativo autenticador*
3. Usando o aplicativo autenticador, agora você tem duas opções:


   Escanear o código QR

   1. Abra seu aplicativo autenticador.
   2. Use o aplicativo para escanear o código QR.
   3. Após escaneá-lo, clique em **Escaneei o código**
      na Miro.

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../docs/administration/security-compliance/images/27601422721298_2FA-setup-step-2-Scan-QR-code.png)*Escaneando o código QR*

   Inserir o código da Miro manualmente

   1. Se você não conseguir escanear o código QR, clique em **Não consegue escanear o código QR?** na Miro.
   2. A Miro fornecerá então um código de autenticação. **Copie** esse código.
   3. Abra seu aplicativo autenticador e cole o código copiado.
   4. Após adicionar o código ao aplicativo, clique em **Adicionei o código** na Miro.

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../docs/administration/security-compliance/images/27601397098898_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*Copiando o código da Miro para colar no aplicativo autenticador*
4. O aplicativo autenticador gerará um código de verificação de 6 dígitos. Insira este código na Miro e clique em **Verificar código**.

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../docs/administration/security-compliance/images/27601422725906_2FA-setup-step-3-enter-6-digit-code.png)
   *Verificando o código de 6 dígitos*
5. Após verificar sua conta com sucesso com o código de 6 dígitos, a Miro fornecerá um código de recuperação. Clique **Copiar** para salvar este código com segurança. É crucial ter esse código, pois ele permite que você redefina seu 2FA caso perca o acesso ao seu aplicativo autenticador.

   Para confirmar que você registrou o código, selecione **Eu registrei este código**, em seguida, clique em **Continuar** para concluir o processo.

   ![Save-2FA-recovery-code.png](../../../../../../docs/administration/security-compliance/images/27601422727314_Save-2FA-recovery-code.png)*Salvando o código de recuperação*

## Entrar com autenticação de dois fatores (2FA)

Depois de configurar com sucesso a autenticação em dois fatores (2FA) para sua conta, toda vez que você tentar iniciar sessão, a Miro pedirá para você inserir um código de uso único de 6 dígitos baseado em tempo (TOTP).

Este código é gerado pelo seu aplicativo autenticador e fornece uma camada extra de segurança para sua conta. Basta abrir seu aplicativo autenticador, recuperar o código atual e inseri-lo na página de iniciar sessão para obter acesso à sua conta.

![2fa-user-guide.png](../../../../../../docs/administration/security-compliance/images/27601397105298_2fa-user-guide.png)
*Iniciando sessão na Miro com 2FA*

Você tem três tentativas antes de solicitarmos para reiniciar o processo de iniciar sessão.

![Too-many-attempts.png](../../../../../../docs/administration/security-compliance/images/27601397107474_Too-many-attempts.png)*Muitas tentativas de iniciar sessão com 2FA*

### Dispositivos confiáveis autenticados por dois fatores (2FA)

Se o seu admin tiver configurado, você pode marcar a caixa de seleção **Confiar neste dispositivo** ao iniciar sessão na sua conta com 2FA ao usar um dispositivo seguro (não use **Confiar neste dispositivo** se iniciar sessão em um computador compartilhado ou de acesso público). Ao fazer isso, você poderá iniciar sessão sem inserir seu segundo fator, até que um período de tempo especificado tenha passado. Esse período é definido pelo seu admin, e pode ser entre 7 e 90 dias.

![2FA-signin.png](../../../../../../docs/administration/security-compliance/images/27601397108882_2FA-signin.png)

*A duração da confiança em um dispositivo é exibida ao lado da caixa de seleção ao fazer login com autenticação de dois fatores*

Se você não vir a opção "Confiar neste dispositivo", então seu admin não a habilitou para sua organização.

Se fizer login com um novo dispositivo, ou depois de limpar os cookies do seu dispositivo confiável, a autenticação de 2FA será necessária novamente.

## Como redefinir a autenticação em dois fatores (2FA)

Se você tiver problemas com seu aplicativo autenticador, perder seu dispositivo ou precisar redefinir seu 2FA por qualquer outro motivo, siga estas etapas:

### Eu tenho um código de recuperação

1. Clique em **Redefinir a autenticação em dois fatores**.
2. Use o código de recuperação salvo durante sua configuração inicial de 2FA. Você será guiado pelo processo de configuração novamente para reconfigurar seu aplicativo autenticador.

![Reset-two-factor-authentication.png](../../../../../../docs/administration/security-compliance/images/27601422733714_Reset-two-factor-authentication.png)*A opção para redefinir a autenticação de dois fatores*

### Não tenho um código de recuperação

Se você perdeu seu código de recuperação ou não consegue usar o fluxo de autorrecuperação, será necessário solicitar que seu admin redefine sua 2FA.

Os admins podem redefinir a autenticação em dois fatores apenas para usuários cujos domínios de e-mail estão verificados em sua organização se o admin iniciar a redefinição. Se o usuário solicitar a redefinição, qualquer admin na organização pode aprová-la.

1. Clique em **Pedir para o seu admin redefinir**.
   ![2fa-user-reset.png](../../../../../../docs/administration/security-compliance/images/27601397113106_2fa-user-reset.png)
   *Peça ao seu admin para redefinir sua autenticação em dois fatores se você não tiver um código de recuperação*
2. Se você pertence a mais de uma organização que utiliza autenticação em dois fatores, será necessário selecionar para qual admin da organização deseja fazer a solicitação.
3. Você receberá um e-mail com um código de verificação.
4. Informe o código de verificação.
5. Uma confirmação de que a solicitação foi enviada ao admin escolhido será exibida.
6. Quando o admin redefinir seu 2FA, você precisará passar pelo processo de configuração do 2FA na próxima vez que fizer login.

## Perguntas frequentes

Por que preciso configurar o 2FA?

A autenticação de dois fatores aumenta a segurança da sua organização. Todos os usuários que não possuem logon único devem usar autenticação de dois fatores para fazer login, caso esse requisito seja imposto pelo Admin da Empresa.

Tenho que usar a autenticação em dois fatores toda vez que iniciar sessão?

Sim. Após concluir a configuração inicial, você deve usar seu aplicativo autenticador para cada início de sessão para garantir que sua conta permaneça segura.

Tentei configurar a autenticação em dois fatores, mas recebi um erro de "Código inválido", embora meu código esteja correto. O que devo fazer?

Certifique-se de que o fuso horário, a data e a hora do seu dispositivo estejam definidos corretamente. Se o problema persistir, tente configurar a autenticação em dois fatores em um dispositivo diferente.

E se eu acidentalmente confiar em um dispositivo compartilhado?

Se você acidentalmente confiar em um dispositivo compartilhado, será necessário limpar os cookies da Miro naquele dispositivo. Fazer isso é simples:

1. Clique no ícone do controle deslizante no lado esquerdo da barra de endereço do seu navegador.
2. Clique em "Cookies e dados do site" no menu.
3. Em seguida, clique em "Gerenciar dados do site no dispositivo".
4. Clique no ícone da lixeira ao lado de cada URL exibido para limpar os cookies e os dados do site.

Observe que, depois de limpar os dados do site do dispositivo, você terá que fazer login novamente usando a autenticação de dois fatores.

E se eu perder o acesso a um dispositivo confiável?

Se você perder o acesso a um dispositivo confiável antes que o período confiável expire, você pode usar a opção **Sair de todos os lugares** para remover o acesso de todos os dispositivos conectados (exceto o dispositivo que você está usando no momento). Isso desconectará você de todos os outros dispositivos e revogará a autenticação de dois fatores de qualquer dispositivo confiável. Você pode encontrar o link **Sair de todos os lugares** nas configurações do seu perfil de usuário. Você precisará então passar pelo processo de login 2FA novamente nos dispositivos aos quais você tem acesso.
