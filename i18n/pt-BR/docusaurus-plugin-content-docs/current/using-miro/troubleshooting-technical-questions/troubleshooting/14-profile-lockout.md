---
title: Bloqueio de perfil
article_id: 360017571374
translation_id: 360017571374
locale: pt-br
sidebar_position: 14
created_at: '2019-02-11T10:08:55Z'
updated_at: '2026-02-24T12:02:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

O bloqueio de perfil é padrão paratodos os usuários e planos da Miro, sem possibilidade de personalização. Usuários que tentam [autenticar por meio de provedores de identidade externos](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) não serão afetados por esta funcionalidade.

Após uma tentativa de login incorreta no seu perfil, você tem **10 tentativas** para inserir a senha correta para um par e-mail e senha. As primeiras 5 tentativas são padrão, sem complexidade adicional.

As tentativas seguintes adicionam captcha (somente para aplicativos web e para desktop). Se não conseguir fornecer a senha correta **10 vezes consecutivas** para um par e-mail e senha, seu perfil de usuário será bloqueado por**1 hora**, durante a qual todas as tentativas de login no perfil falharão, mesmo que a senha correta seja fornecida.

:::tip
Durante a hora de bloqueio, você pode tentar fazer login sem senha ou com um provedor social.
:::

Assim que o seu perfil de usuário for bloqueado, a Miro envia um e-mail com um código de seis dígitos para desbloquear o perfil. O link no e-mail redireciona você para a página de confirmação, onde você deve fornecer o código de seis dígitos. Se o código fornecido estiver correto, seu perfil será desbloqueado e todas as tentativas são reiniciadas. O e-mail também recomenda alterar a senha.

O perfil bloqueado é desbloqueado **automaticamente** em 1 hora e todas as tentativas falhas são reiniciadas.

### O que fazer se você não receber o código

Se você não encontrar o e-mail na sua caixa de entrada, tente esses passos para solucionar o problema:

- Certifique-se de que não haja erros de digitação no e-mail que você enviou. Se encontrar um erro, tente fazer login com o endereço correto
- Abra as caixas de **Spam, Promoções, Lixo, Social** e **Atualizações** e verifique se o e-mail de confirmação da Miro está lá
- Verifique se sua caixa de entrada está cheia para ter certeza de que não atingiu o limite da sua caixa de entrada de e-mail. Se estiver cheia, talvez seja necessário excluir alguns e-mails existentes para receber novos. Após excluir os e-mails, clique em **Enviar código novamente** para receber um e-mail de registro
- Também pode ser que um firewall esteja impedindo o e-mail de chegar à sua caixa de entrada. Entre em contato com o seu *admin do sistema* e peça para que inclua nossos domínios e subdomínios na lista de permitidos: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) e [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Aqui está um artigo](../../tools/troubleshooting/02-allowlist-miro-mailers.md) com mais informações sobre os remetentes que você precisa colocar na lista de permitidos.
- Usuários AOL/CompuServe: certifique-se de que seus Controles de E-mail estejam configurados para receber e-mails da Internet. Se você bloqueou e-mails da Internet, por favor, altere seus Controles de E-mail acessando **Controles de E-mail** no AOL ou CompuServe. Depois disso, volte ao nosso formulário de registro para reenviar seu código de confirmação
- Normalmente, o código deve chegar instantaneamente, mas, devido às peculiaridades do seu sistema de e-mails, você pode precisar esperar até 24 horas
- Se nenhuma das soluções ajudar, [relate o problema ao Suporte Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
