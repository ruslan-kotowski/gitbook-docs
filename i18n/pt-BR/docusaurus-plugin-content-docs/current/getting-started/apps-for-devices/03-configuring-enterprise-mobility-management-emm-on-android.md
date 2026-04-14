---
title: Configurando o gerenciamento de mobilidade Enterprise (EMM) no Android
article_id: 13888848676498
translation_id: 13888848676498
locale: pt-br
sidebar_position: 3
created_at: '2023-09-21T14:45:02Z'
updated_at: '2025-11-25T15:38:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
availability:
  notes: 'gerais: sobre como configurar a solução EMM/MDM da sua empresa usando três
    exemplos de software específico: VMWare (Workspace ONE), Ivanti Neurons (antigo
    MobileIron Cloud) e Intune (Microsoft Endpoint Manager). Se você usar uma solução
    diferente, para obter etapas exatas, recomendamos consultar a documentação do
    seu provedor de EMM.'
---

O EMM permite que os admins da empresa configurem e distribuam o Miro aos usuários em sua organização de forma centralizada e unificada. O Miro oferece suporte ao provisionamento das seguintes configurações para os dispositivos do usuário final:

- Desabilitando o fluxo de criar conta .
- Limitar provedores de autenticação suportados (por exemplo, redes sociais, provedores de e-mail, etc.).
- Restringir o nome de usuário a um valor específico ou a uma lista de domínios de e-mail permitidos.
- Configuração avançada de SSO .

## Como configurar

### Adicione o Miro ao diretório de aplicativos da sua organização

Para a maioria, habilitar a configuração do EMM exigirá adicionar o Miro ao catálogo de aplicativos da sua organização. Esse processo pode variar de um provedor de EMM para outro. Ainda assim, normalmente, você adicionará o Miro ao seu catálogo de aplicativos diretamente da Google Play Store e definirá uma política de distribuição com base em grupos de dispositivos, grupos de usuário , etc.

#### Exemplos:

**VMware Workspace ONE**

O guia geral de implantação do VMware Workspace ONE pode ser encontrado [aqui](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Clique em **Adicionar** e depois em **Aplicativo Público.**
2. Selecione **Android** no menu suspenso Plataforma e pesquise a fonte**na App Store**.
3. Digite “**Miro**” na **caixa de texto Nome** e clique em Avançar.
4. Selecione o aplicativo da Miro e pressione **Aprovar** , se solicitado.
5. Publique o aplicativo clicando em **Salvar e Atribuir**.
6. Configure atribuições e configurações de distribuição de acordo com as preferências da sua organização.

**Neurônios Ivanti**

O guia geral de implantação do Ivanti Neurons pode ser encontrado [aqui](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/92/all/Managing_Google_Play_apps.htm).

- 1. Acesse **Aplicativos > Catálogo de aplicativos** e clique em **Adicionar.**
  2. Selecione “**Google Play Store**” e seu país como fonte.
  3. Procure por “**Miro**” e selecione “**Miro: lousa online online**” da lista de aplicativos disponíveis.
  4. Configure as configurações e políticas de distribuição de acordo com as preferências da sua organização.

**Intune (Gerenciador de Endpoint da Microsoft)**

O guia geral de implantação do Intune da MS pode ser encontrado [aqui](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-android).

1. Vá para **Aplicativos > Todos os aplicativos** e clique em **Adicionar**.
2. Selecione **Store App > Android store app** como o **tipo de aplicativo**.
3. Na página**Informações do aplicativo** , preencha os detalhes da [listagem do Miro na Google Play Store](https://play.google.com/store/apps/details?id=com.realtimeboard).
4. Configure as configurações e políticas de distribuição de acordo com as preferências da sua organização.

Configure as configurações e políticas de distribuição de acordo com as preferências da sua organização.

### Pré-preenchendo as configurações do aplicativo

Miro usa [AppConfig](https://www.appconfig.org/) como uma maneira unificada de configurar e proteger os dados dos clientes, o que fornece uma maneira fácil de configurar aplicativos móveis corporativos. Muitas soluções EMM suportam o formato AppConfig ou o aceitam em um “modo de compatibilidade”. Para saber as limitações exatas aplicáveis ao seu caso, consulte a documentação do seu provedor de EMM.

#### Exemplos:

**Espaço de trabalho VMWare ONE**

O guia geral de implantação do VMware Workspace ONE pode ser encontrado [aqui](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Vá para **Recursos > Aplicativos**.
2. Clique em **Atribuir** na coluna**status da instalação** no **Miro: lousa online online** linha de aplicativo.
3. Defina o **nome, os grupos de atribuição** e **o método de entrega do aplicativo** da distribuição.
4. Habilitar **acesso gerenciado** e **enviar configuração**
5. Defina a configuração do aplicativo.

**Neurônios Ivanti**

O guia geral de implantação do Ivanti Neurons pode ser encontrado [aqui](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/92/all/Using_the_Android_enterprise_App_Configuration.htm).

1. Acesse **Aplicativos > Catálogo de aplicativos**.
2. Navegue até “**Miro: lousa online online**" configurações.
3. Acesse **Configurações do aplicativo > Configurações gerenciadas para Android**.
4. Clique em **Adicionar** para criar **Restrições de Aplicativo**.
5. Defina o **necessário** e **o tempo de execução** **Permissões**.
6. Selecione o perfil de distribuição na seção **Distribuir esta configuração de aplicativo**.

**Intune (Gerenciador de Endpoint da Microsoft)**

O guia geral de implantação do Intune da MS pode ser encontrado [aqui](https://learn.microsoft.com/mem/intune/apps/app-configuration-policies-use-android).

1. Acesse **Aplicativos > Políticas de configuração de aplicativos > Adicionar > Dispositivos gerenciados** para criar uma nova configuração de aplicativo.
2. Defina o nome do seu perfil de configuração.
3. Selecione **Android Enterprise** como **plataforma**.
4. Selecione **Miro: lousa online online** como o **aplicativo de destino** clicando em **Selecionar aplicativo**.
5. Selecione **Usar designer de configuração** como **Formato de definições de configuração**.
6. Definir configuração do aplicativo.
7. Selecione o perfil de distribuição para a configuração.

## Lista completa de configurações suportadas

### Limitando as opções “Entrar com…” / “Inscrever-se”

Se a opção “Inscrever-se” estiver habilitada, todas as configurações de “Entrar com…” afetarão o fluxo de inscrição.

:::warning
Qualquer chave não definida explicitamente como "true" (ou ausente) é considerada definida como "false". Portanto, a opção de autenticação está disponível (comportamento padrão).
:::

| Chave | Tipo de | Valores permitidos |
| --- | --- | --- |
| **Facebook** miro.authentication.facebookRestrito | Booleano | verdadeiro/falso |
| **Google** miro.authentication.googleRestrito | verdadeiro/falso |
| **Microsoft Office 365** miro.authentication.office365Restrito | verdadeiro/falso |
| **Slack**   miro.authentication.slackRestrito | verdadeiro/falso |
| criar conta miro.authentication.signUpRestricted | verdadeiro/falso |
| **Entre com o Magic Link** miro.authentication.magicLinkRestricted | verdadeiro/falso |
| **espaço de trabalho Enterprise** miro.authentication.enterpriseWorksSpaceDesabilitado | verdadeiro/falso |

### Restrições de nome de usuário

Os clientes que desejam melhorar a segurança mantendo a autenticação de senha simples podem usar as seguintes opções.

| Chave | Valor | Descrição |
| --- | --- | --- |
| **Nome de usuário predefinido** miro.policy.autenticação.nome de usuário | **Tipo de valor:** string | O campo está bloqueado e não pode ser alterado pelo usuário |
| **Domínios na lista de permissões** miro.policy.authentication.allowedDomains | **Tipo de valor:** matriz  **Valor:** @miro.com, @seudominio.com  *Alguns provedores não suportam o tipo de dados **array** . Se for esse o caso, use o tipo **string** e matriz JSON como um valor. ["@miro.com", "@seudominio.com"] | Somente e-mails correspondentes a um dos domínios listados são permitidos. |

### Configuração SSO

Para melhorar a segurança da organização e simplificar o processo de autenticação para usuários finais, os admins da organização podem configurar a política de SSO usando o exemplo a seguir.

:::warning
Certifique-se de que a política de SSO na configuração do aplicativo corresponda às configurações de SSO da organização Miro . A incompatibilidade dessas políticas pode resultar em uma situação de “bloqueio”, quando os usuários não conseguem efetuar login. O Miro não pode validar as configurações antes de aplicá-las nos dispositivos de destino.
:::

|  |  |
| --- | --- |
| Chave de configuração | miro.policy.sso |
| Tipo de valor de configuração | corda |
| Objeto de política | \{ "authenticationRestricted" : false, "email": "usuário@domain.com", "allowedDomains": ["domain1.com", "domain2.com"], "forceSsoLogin": true \} |

| Atributos do objeto de política | | | |
| --- | --- | --- | --- |
| Parâmetro | Tipo de | Descrição | Nota |
| autenticaçãoRestrita | booleano | Se o botão "Login com SSO" está habilitado na página principal. | **A chave é ignorada quando outras opções de configuração são fornecidas.** |
| e-mail | corda | E-mail predefinido para login SSO . | O campo está bloqueado e não pode ser alterado |
| domínios permitidos | booleano | Mantenha o SSO como o único método disponível para autenticação. | O usuário final é imediatamente levado para a página “Login com SSO ”. Outras opções além de **email** e **allowedDomains** são ignoradas. Nenhum outro método de autenticação está disponível. |
