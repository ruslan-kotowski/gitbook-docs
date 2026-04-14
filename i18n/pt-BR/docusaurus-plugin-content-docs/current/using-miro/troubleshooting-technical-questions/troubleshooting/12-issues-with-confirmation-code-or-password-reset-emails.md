---
title: "Problemas com c\xF3digo de confirma\xE7\xE3o ou e-mails de redefini\xE7\xE3\
  o de senha"
article_id: 360017731373
translation_id: 360017731373
locale: pt-br
sidebar_position: 12
created_at: '2019-02-11T10:14:22Z'
updated_at: '2024-10-25T14:25:54Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Se você não receber um código de confirmação ou um e-mail de redefinição de senha, pode haver várias razões para isso. As informações abaixo podem ajudar a resolver a situação dando algumas opções para você tentar.

## Motivos comuns pelos quais os códigos ou e-mails não chegam

Os dois motivos mais comuns pelos quais você não recebe e-mails de redefinição de senha ou não consegue solicitar um novo código de confirmação são:

1. Sua empresa usa um firewall e o firewall está bloqueando os e-mails dos domínios da miro.com. Peça ao seu admin de TI para permitir os e-mails de [domínios](http://miro.com/)miro.com. Se você for admin, veja a seção abaixo para instruções sobre como acrescentar domínios da Miro à lista de permissões.
2. Sua empresa usa SSO. Veja a seção abaixo para instruções sobre como resolver isso.

## Como resolver e-mails perdidos/problemas de código de confirmação

1. Se sua empresa usa SSO, você deve fazer login com suas credenciais SSO corporativas. Se tentar redefinir sua senha com a Miro, redirecionaremos você para a página de login do SSO. Se isso acontecer, tente usar suas credenciais SSO corporativas. Se isso não funcionar, continue com a solução de problemas abaixo.
2. Um firewall pode estar impedindo que o e-mail chegue à sua caixa de entrada. Peça ao admin do sistema  para incluir nossos domínios e subdomínios na lista de permissões: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com and realtimeboard.com*, *.realtimeboard.com.

   Confira a lista de IPs dedicados: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. Leia mais sobre [como acrescentar e-mails da Miro à lista de permissões.](../../tools/troubleshooting/02-allowlist-miro-mailers.md)
3. Certifique-se de que não haja erros de digitação no e-mail que você enviou. Se você encontrar um erro de digitação, [registre um perfil novamente](../../../getting-started/start-here/02-how-to-register-with-miro.md)/redefina sua senha usando o endereço de e-mail correto.
4. Verifique as pastas de **Spam, Promoções,** **Lixo eletrônico, Social** e **Atualizações** no seu provedor de e-mail.
5. Você também pode se registrar ou fazer login usando opções alternativas de inscrição/login: faça login ou inscreva-se com Google, Slack, Office 365, Apple ou Facebook.
   > ⚠️ Observe que os logins alternativos **não** estão conectados a logins SSO corporativos. Se estiver usando a Miro em um ambiente corporativo, use as credenciais que seu admin da Miro configurou para você.

   ![](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)altnew-sing-in-third-party.png
   Métodos de autenticação disponíveis

Se você não conseguir se inscrever ou fazer login usando outros métodos de autenticação:

- Verifique se sua caixa de entrada está cheia e se não atingiu o seu limite de armazenamento de e-mail. Se estiver cheia, talvez precise excluir alguns e-mails para receber novos. Depois de excluir os e-mails, volte para nossa página de registro e clique em **Reenviar código.**
- Você deve receber o e-mail imediatamente. Se não, pode ser necessário esperar até 24 horas.
- Se você estiver usando suas credenciais SSO corporativas e não conseguir fazer login, leia sobre [os erros comuns de SSO e como resolvê-los](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

### Outros problemas de confirmação

Meu código é inválido.

Se o código que você inseriu for **inválido:**

1. Verifique sua caixa de entrada e certifique-se de inserir o código mais recente que recebeu. Se mesmo assim o código for inválido, clique em **Reenviar código** e insira o código do novo e-mail.
2. Outra maneira de concluir o registro é clicar em **Confirmar seu e-mail** no e-mail com o código de confirmação. Neste caso, você não precisa do código de confirmação.
   ![botão confirmar e-mail.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725339026_confirm%20email%20button.png)
   *A opção de confirmar seu e-mail*

Excedi as tentativas de confirmação de e-mail.

Se você não conseguiu confirmar seu e-mail após quatro tentativas, verá a mensagem **Tentativas de confirmação de e-mail excedidas** na página de registro.

Aguarde 60 segundos e clique em **Reenviar código.** Isso gerará um novo código para você. Digite o código e conclua o registro.

Fechei acidentalmente a guia onde insiro o código de confirmação.

[Faça login](https://miro.com/login/) usando o e-mail e a senha que você inseriu durante o registro e a [página de confirmação](https://miro.com/email-confirm/) será reaberta novamente.

:::note
Se você não confirmar seu e-mail, receberá lembretes após 12 e 24 horas. Se não confirmar seu e-mail em sete dias, seu **perfil será excluído**. Você poderá registrar um novo perfil usando o mesmo endereço de e-mail.
:::

:::note
Os códigos de confirmação só podem ser enviados por e-mail.
:::

:::note
Se você ainda estiver tendo problemas, [entre em contato com o Suporte da Miro](https://miro.com/contact/recover/).
:::
