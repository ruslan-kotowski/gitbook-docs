---
title: "N\xE3o consigo fazer login via SSO"
article_id: 360019271654
translation_id: 360019271654
locale: pt-br
sidebar_position: 10
created_at: '2019-03-07T15:50:03Z'
updated_at: '2025-11-25T16:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Obtenha conselhos sobre solução de problemas para você e seus admins de TI sobre questões relacionadas ao logon único (SSO).

> **✏️** Saiba mais sobre [como configurar o Miro SSO](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) e [o Miro SCIM](https://developers.miro.com/docs/scim).

## Erros de SSO da Miro

Se você vir alguma dessas mensagens de erro de SSO, explore as soluções abaixo.  Você pode precisar de ajuda do seu departamento de TI ou dos Admins da empresa.

Seu e-mail não está associado a uma conta de SSO

Isso acontece quando o endereço de e-mail que você inseriu no Miro não é reconhecido como um usuário que deve ser autenticado via SSO.

Possíveis causas:

- **Você não é membro de nenhuma assinatura que estabeleceu o SSO como requisito de login**. Faça login usando as opções padrão (e-mail e senha) ou entre em contato com seu admin para ser convidado para a assinatura da sua empresa.
- **Você deveria fazer login via SSO, mas há uma confusão com seu endereço de e-mail**. Talvez você tenha vários e-mails (ou aliases) e o convite para o plano com SSO estabelecido foi enviado para seu outro endereço. Faça login com outro endereço de e-mail.

Seu e-mail não está associado à conta de SSO. Solicite acesso ao Admin da empresa

Isso geralmente acontece em dois cenários:

- **Seu perfil de usuário no sistema do Provedor de Identidade não tem permissão para entrar no Miro (você não tem uma função atribuída)**. Se esse for o caso, você provavelmente não encontrará o Miro como um bloco no painel MyApps do seu provedor. Entre em contato com o admin do seu provedor para obter as permissões necessárias.
- **Você alterou recentemente seu** e-mail (por exemplo, devido a mudança de sobrenome) e a alteração não foi aplicada corretamente em todos os sistemas, criando conflitos. Entre em contato com seu admin para esclarecer a situação e, se necessário, ele entrará em contato conosco para aprovar quaisquer alterações necessárias.

Se você não conseguir fazer login no Miro via SSO, poderá solicitar acesso aos Admins da empresa clicando no botão correspondente na [página de login do Miro SSO](https://miro.com/sso/login/).

![sso-new-sign-in.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/20463017477778_sso-new-sign-in.png)*A opção de solicitar acesso aos Admins da empresa*

Você precisará inserir o código de confirmação enviado para seu endereço de e-mail. Depois de inserir o código, uma notificação será enviada aos admins da assinatura da sua empresa, informando-os de que você precisa de assistência.

Algo deu errado A validação da assinatura para resposta não foi bem-sucedida

Isso significa que há uma configuração incorreta nas configurações do Miro SSO ou no final do seu Provedor de Identidade. É provável que nenhum dos seus colegas consiga fazer login. Entre em contato com seu departamento de TI ou com o admin do Provedor de Identidade para que eles possam verificar os seguintes pontos:

- A resposta SAML deve conter a *asserção*assinada. Este é um requisito do Miro .
- Seu Provedor de Identidade pode estar tratando respostas assinadas de uma maneira específica. Por exemplo, o SSO do Google *cancela* a assinatura da afirmação quando a *resposta* está assinado. Se for esse o caso, cancele a assinatura da resposta.
- A resposta SAML contém a asserção assinada necessária, mas o valor do certificado X.509 que deveria validá-la não está presente (também pode acontecer se sua VPN/firewall [cortar partes da transferência de dados](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)). Certifique-se de que o valor do certificado X.509 seja passado no tráfego SAML para o Miro.
- A resposta SAML contém um *valor de certificado X.509 diferente do que o adicionado nas* [configurações da Miro](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), portanto, há uma incompatibilidade e a validação falha. Verifique se os valores do certificado no lado do IDP e no lado do Miro correspondem.

Algo deu errado Não foi fornecido o usuário na resposta SAML.

Isso significa que há uma configuração incorreta no seu Provedor de Identidade, seja na configuração geral ou no seu perfil de usuário específico. Entre em contato com seu departamento de TI ou com o admin do Provedor de Identidade para que eles possam verificar os seguintes pontos.

- O formato Nome de usuário (NameID, Unique user ID) na sua configuração de SSO não é especificado ou definido como um atributo que não seja por e-mail, portanto, o valor do usuário enviado para a Miro não pode ser reconhecido.  Especifique o nome de usuário para **EmailAddress** no lado do Provedor de Identidade (ou para qualquer outro atributo que esteja no formato de e-mail).
- A resposta SAML não contém o valor de e-mail do usuário, portanto, o usuário não pode ser reconhecido (isso também pode acontecer se sua VPN/firewall [cortar partes da transferência de dados).](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)). Certifique-se de que o e-mail seja transferido no tráfego SAML para a Miro.
- A resposta SAML é criptografada. Não use criptografia, pois o Miro não oferece suporte a ela.

Algo deu errado A resposta SAML não está correta

Isso geralmente acontece quando há problemas com seu perfil no Provedor de Identidade.
Possíveis causas:

- **Seu perfil de usuário no sistema do Provedor de Identidade está configurado incorretamente**. Por exemplo, você não tem permissão para entrar no Miro (você não tem uma função atribuída). Se esse for o caso, você provavelmente não encontrará o Miro como um bloco no painel MyApps do seu provedor. Entre em contato com o admin do seu provedor para obter as permissões necessárias.
- **Seu perfil de usuário no sistema do provedor de identificação está configurado corretamente, mas tem restrições aplicadas**.  Por exemplo, há restrições de IP, portanto, você só tem permissão para fazer login de determinados lugares. Entre em contato com o admin do seu Provedor de Identidade e pergunte sobre suas permissões.

Para autorizar com SSO, use o link de URL fornecido pelo seu empregador.

Isso significa que você não deve acessar a Miro a partir desta página ou que a configuração de SSO no seu plano Enterprise da Miro não está completa.  Nesse caso, você pode fazer login no seu painel MyApps.
Possíveis causas:

- **Seu IDP está configurado somente para** [login iniciado IdP](https://blogs.oracle.com/dcarru/sp-vs-idp-initiated-sso) **, e você não deve conseguir fazer login na página de login do Miro .** Faça login por meio do link fornecido no seu painel MyApps ou entre em contato com o Admin da empresa para obter instruções.
- **O SSO está habilitado no seu plano Miro Enterprise , mas a configuração não foi concluída**. Entre em contato com seu departamento de TI ou admin do provedor de identidade para que eles concluam a configuração de acordo com [estas instruções](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

## Erros de entrada ou ADFS

A configuração de logon único indisponível para este aplicativo na experiência de aplicativos Enterprise .

O texto completo da mensagem: *A configuração de logon único indisponível para este aplicativo na experiência de aplicativos Enterprise . Miro (antigo RealtimeBoard) é um aplicativo multilocatário e o aplicativo é de propriedade de outro locatário.**Para alterar propriedades como URL de resposta e identificadores, entre em contato com o titular do aplicativo.*Entre em contato com seu departamento de TI e peça para verificar a configuração do SSO . Provavelmente, já existe um aplicativo da Miro configurado no seu Entra ID onde nosso identificador (`https://miro.com/)` é usado e, portanto, tomado. O Entra é mais ou menos único, pois esse provedor de identidade exige que o identificador (ID da entidade) seja único.
Para possivelmente resolver a situação, recomendamos que você verifique os aplicativos Enterprise da sua instância Entra e use aquele que você já configurou nas configurações do Miro .
Se você tiver certeza de que não há outros aplicativos Miro em seus aplicativos Enterprise , tente obter uma nova cópia do aplicativo da Miro na galeria Entra.

Ocorreu um erro. Entre em contato com seu admin para obter mais informações

Compartilhe esta postagem da comunidade com seu departamento de TI: [“Ocorreu um erro. Entre em contato com seu admin para obter mais informações”](https://blog.kloud.com.au/2015/07/22/adfs-sign-in-error-an-error-occurred-contact-your-administrator-for-more-information/)

Nenhum acesso concedido: erro AADSTS50105

![mceclip3.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044185746_mceclip3.png)
Compartilhe este artigo da comunidade com seu departamento de TI: [Erro "Função não atribuída"](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50105-user-not-assigned-role)

Aplicativo mal configurado: erro AADSTS650056

![mceclip2.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044184722_mceclip2.png)
Verificamos a documentação da Microsoft para o erro AADSTS650056 (bem como algumas sugestões da comunidade) e parece que o erro pode ser causado pelas alterações que você adicionou às permissões do aplicativo. Seu admin Entra pode precisar dar consentimento ao aplicativo da Miro para permitir que os usuários finais se autentiquem no Miro. [Este tutorial da Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow)deve ser útil neste caso.

Leia [o artigo support.microsoft.com sobre outros possíveis erros de SSO](https://support.office.com/article/how-to-troubleshoot-issues-that-you-encounter-when-you-sign-in-to-office-apps-for-mac-ipad-iphone-or-ipod-touch-when-using-active-directory-federation-services-e44357b4-c9c4-4580-a946-ef5dabdb98cd?ui=en-US&rs=en-US&ad=US).

## Erros SAML do Google

Consulte [esta seção da documentação do Google](https://support.google.com/a/answer/6301076?hl=en) que lista possíveis erros e instruções sobre como resolver a situação.

## Problemas para fazer login no aplicativo da Miro via SSO no aplicativo de desktop, tablet ou celular

Se você não conseguir fazer login no aplicativo da Miro via SSO em um desktop/tablet/dispositivo móvel, mas conseguir fazer login na [versão do navegador](https://miro.com/app/), tenteo seguinte:

1. Exclua o aplicativo do dispositivo e reinstale-o. Para o aplicativo de desktop, certifique-se de remover todas as pastas do aplicativo a seguir [estas instruções](../../../getting-started/apps-for-devices/05-desktop-app.md). A causa mais comum desse problema é um cache ruim, então excluir tudo e reinstalar tudo deve ajudar.
2. Tente alterar o navegador padrão do seu dispositivo para um diferente para fazer um teste e ver se, com um navegador diferente, você consegue concluir o processo.  Certifique-se de que seu navegador preferido permita cookies de terceiros/span>.
3. Verifique se o seu provedor de identidade *não* gerencia o parâmetro **RelayState** . É um token exclusivo que o Miro gera e usa para reconhecer que o usuário deve ser enviado de volta ao aplicativo em vez de permanecer na página do navegador. Veja que os campos na sua configuração IdP que gerenciam o RelayState ficam vazios (o campo pode ser nomeado de forma diferente, por exemplo, em Okta, seria **RelayState padrão**, no Google SSO - *URL inicial*).
4. Se o problema persistir, é possível que este dispositivo específico não possa acessar o ambiente de SSO da empresa.  Verifique com seu departamento de TI se há alguma restrição em relação a dispositivos específicos que têm permissão para usar SSO. Por exemplo, com soluções MDM, podem surgir problemas se o Miro não for devidamente [na lista de permissões](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md).
5. Especificamente para o aplicativo para desktop Miro Desktop, verifique se o esquema do nosso aplicativo funciona corretamente para você e não está quebrado. Para fazer isso, digite **miroapp://** na linha de endereço do seu navegador preferido e clique para abri-lo *como um site* (não pressione simplesmente Enter, pois isso iniciará a pesquisa).
   ![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)
   Neste momento, você deve obter um ​pop-up solicitando que você abra o aplicativo da Miro. Se isso não acontecer, o esquema pode estar quebrado. Para verificar se o esquema está instalado corretamente, siga as instruções para Windows ou Mac (isso não se aplica à versão MS Store do aplicativo da Miro).

   Para WindowsPara Mac

   1. Acesse o [aplicativo Editor do Registro](https://support.microsoft.com/windows/how-to-open-registry-editor-in-windows-10-deab38e6-91d6-e0aa-4b7c-8878d9e07b11)
   2. Pressione Ctrl + F e encontre **aplicativo miro.** Seu registro deve ficar assim: *![registry_editor_map.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057554322_registry%20editor%20map.png)*

   1. Execute o seguinte comando no aplicativo do terminal:

      **sudo /System/Library/Frameworks/CoreServices. framework/Versions/A/Frameworks/LaunchServices. framework/Versions/A/ Suporte/lsregister -dump URLSchemeBinding | grep miroapp**

      O resultado deve ser algo como isto:

      ![](/attachments/token/I53o1MUemZ9TqkRlz9dQ7ndsr/?name=image.png)

Se a sua situação for diferente (o registro do esquema não é exibido no registro ou é exibido em um caminho diferente, por exemplo), tente reinstalar o aplicativo [do nosso site](https://miro.com/apps/).

Se isso não ajudar, entre em contato com sua time de TI e peça para verificar a situação, especialmente os seguintes pontos:

- se protocolos URI personalizados são permitidos. Se eles forem bloqueados, nosso esquema poderá ser impedido de ser instalado durante o processo de instalação do aplicativo.
- se o registro está sob alguma outra restrição ou política que pode impedir ou modificar a instalação padrão.

## Meu e-mail mudou e não consigo fazer login no meu perfil via SSO

Observe que se sua organização usa SSO, a alteração do endereço de e-mail precisa ser feita no lado do Miro e no lado do Provedor de Identidade antes que um usuário final tente usar suas novas credenciais para efetuar login no Miro. Se a alteração não for feita antes do próximo login, seu e-mail será reconhecido como um novo usuário, e você pode ter problemas para fazer login no Miro.

Entre em contato com seu admin para esclarecer a situação. Você e seu admin podem precisar entrar em contato com o suporte da Miro/span> [para que possamos excluir seu novo perfil vazio e alterar o endereço de e-mail no perfil existente.](../../tools/troubleshooting/06-contacting-miro-support.md) Forneça as seguintes informações:

- Seu novo endereço de e-mail e seu antigo endereço de e-mail
- Envie uma cópia para o admin Miro da sua empresa e peça para ele enviar uma confirmação de que podemos prosseguir com a alteração (necessário por motivos de segurança)

:::note
Se você não conseguiu encontrar uma solução acima, [entre em contato com o Suporte Miro](https://miro.com/contact/recover/).
:::
