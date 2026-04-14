---
title: "Controle de dom\xEDnio"
article_id: 360034831793
translation_id: 13951277297938
locale: pt-br
sidebar_position: 1
created_at: '2023-09-25T02:03:34Z'
updated_at: '2026-03-27T15:51:56Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  plans: business, enterprise
  roles: company_admin, system_admin
---

> **Disponível em:** Business, Enterprise
> **Função necessária:** Admin da empresa, admin do sistema

O controle de domínio permite que Admins da empresa gerenciem o acesso de usuários em suas assinaturas. Ao utilizar o controle de domínio, admins podem aplicar a conformidade de segurança empresarial e controlar as atividades gerenciadas dos usuários em seus domínios.

Saiba como configurar e gerenciar o controle de domínio em sua organização.

**Com o controle de domínio, admins do plano Enterprise podem:**

- Realizar auditorias para identificar usuários associados a um domínio gerenciado que não esteja incluído na assinatura e convidá-los a se incluírem.
- Impedir que os usuários de um domínio criem assinaturas não autorizadas.
- Adicionar automaticamente usuários recém-registrados aos times designados.
- [Bloquear usuários desativados](../../user-management/02-block-deactivated-users.md) para impedir o acesso deles à Miro usando o e-mail corporativo.

**Admins do plano Business:**

- Podem usar a verificação automática de domínios para gerenciá-los. Somente os domínios recém-adicionados serão verificados automaticamente.
- Não podem alterar as políticas de controle de domínio.
- Não podem solicitar uma auditoria de domínio.

![domain-policies-business.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21046889202834_domain-policies-business.png)

*Os usuários do plano Business podem visualizar as políticas de domínio em Domínios gerenciados.*

Os usuários do plano Business deverão fazer upgrade para acessar outras funcionalidades avançadas.

:::note
O gerenciamento de domínio em massa não está disponível no momento.
:::

## Domínio principal

Seu domínio principal determina como a Miro identifica usuários internos e externos em sua organização. Para saber como visualizar, alterar ou gerenciar seu domínio principal, consulte [Gerenciar seu domínio principal](https://help.miro.com/hc/en-us/articles/34249718672274).

## Configurar o controle de domínio

### Passo 1: adicionar domínios

1. Abra seu painel da Miro.
2. Clique na foto do seu perfil no canto superior direito.
3. Selecione **Configurações** no menu suspenso.
4. No painel à esquerda, navegue até **Segurança e conformidade** e clique em **Domínios gerenciados**

   > ✏️ Nos planos Business, **Domínios gerenciados** é encontrado em **Conta**.
5. Clique em **+ Adicionar um domínio** e insira o nome completo do domínio (por exemplo, suaempresa.com).
   ![Managed-domains-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318776338_Managed-domains-settings.png)
*Configurações de domínio gerenciado*

:::note
Se você habilitou [**Bloquear usuários desativados**](../../user-management/02-block-deactivated-users.md), todos os usuários desativados associados a um domínio recém-verificado são bloqueados automaticamente.
:::

### Passo 2: Verificar domínios

1. Depois de adicionar um domínio, você receberá um código de verificação nas suas configurações de **Domínios gerenciados**. Copie esse código.

   ![Complete-domain-verification.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318779282_Complete-domain-verification.png)
*Copiando o código de verificação*
2. Se você gerencia seus registros DNS, atualize suas configurações de DNS adicionando um registro TXT com o código de verificação no campo **Valor**. (Se outra pessoa for responsável por gerenciar seus registros DNS, encaminhe a essa pessoa o código de verificação com instruções para a atualização dos registros.)
3. Faça login no site do seu provedor de domínio (GoDaddy, Amazon, Cloudflare, etc) e navegue até a seção de **registros** **DNS**.
4. Crie um novo **registro TXT** com as seguintes especificações:
   **Valor/Resposta/Descrição:** *“miro-verification=[INSERIR CÓDIGO DE VERIFICAÇÃO]”*
   **Nome/Host/Apelido:** Deixe em branco ou digite @ para incluir um subdomínio.
   **Tempo de vida (TTL):** “86400” (também pode ser herdado da configuração padrão).

   ![Creating-new-TXT-record.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318775314_Creating-new-TXT-record.png)
   *Criando um novo registro TXT*

:::note
Você pode atualizar o registro TXT através do console de administração ou painel do provedor de hospedagem DNS do domínio. Veja a [lista de provedores de DNS](https://support.google.com/a/topic/1409901).
:::

### Passo 3: Conferir a verificação do domínio

1. Depois de atualizar o registro DNS, verifique imediatamente o status da verificação do seu domínio nas configurações de **Domínios gerenciados**, clicando em **Conferir verificação**.
2. Se o domínio não for verificado de imediato, a Miro irá conferir automaticamente o código de verificação a cada duas horas pelos 30 dias seguintes.

### Passo 4: Notificação do status da verificação

1. Assim que seu domínio for verificado com sucesso, você receberá uma notificação por e-mail confirmando o status da verificação.
2. Não remova o registro DNS após a verificação, pois pode ser necessário para futuras verificações.
   ![Check-domain-verification.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017348597650_Check-domain-verification.png)
*Verificando a verificação do domínio*

## Regras ao verificar domínios

- Você deverá criar um registro TXT separado para cada domínio de nível superior e cada subdomínio que usar. Siga os passos 1 a 4 para cada domínio ou subdomínio que deseje verificar.
- Seu domínio deve ser uma correspondência exata.

  > ✏️ Não são permitidos subdomínios.
- Verifique se todas as zonas usadas na configuração do domínio verificado estão incluídas.
- O Nome de Domínio Absoluto (FQDN, Fully Qualified Domain Name) deve corresponder ao seu endereço de domínio. Por exemplo, [www.mycompanydomain.com](http://www.mycompanydomain.com).
- Se você usa DNS interno e externo, recomendamos verificar ambos para garantir o controle abrangente do domínio.

## Gerenciar usuários e acesso

### Editar configurações de domínio

As configurações do domínio determinam como são gerenciados os usuários existentes e recém-registrados no seu(s) domínio(s).

1. Depois de verificar um domínio, clique nos três pontos (**...**) e selecione **Editar configurações do domínio**.
   ![Edit-domain-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318773138_Edit-domain-settings.png)
*Editando configuração do domínio*
2. Você verá as opções para gerenciar novos usuários do seu domínio:

- **Captura automática de novos usuários**: adicione automaticamente usuários que criem conta na Miro com um e-mail de domínio gerenciado à assinatura desse domínio com o tipo de licença padrão. Você também pode definir a quais times os usuários serão adicionados (obrigatório).
- **Impedir que os usuários criem suas próprias assinaturas**: Proíba que usuários gerenciados dentro dos seus domínios criem novos times fora da sua assinatura. No entanto, esses usuários ainda podem ser convidados para times dos seus domínios e colaborar externamente.

  ![Managed-domain-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318773778_Managed-domain-settings.png)
*Opções para lidar com novos usuários no seu domínio*

  > ✏️ Se você ativar **Impedir que os usuários criem suas próprias assinaturas**, então os usuários não poderão se registrar sozinhos, a menos que sejam convidados, ou que a captura automática ou o JIT sejam ativados.

### Usuários internos e externos

Quando um domínio é reivindicado, os detalhes do usuário incluem uma classificação de **Interno** ou **Externo**.

![](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/33613933595794_image.png) *Os detalhes do usuário mostram se o usuário é externo ou interno ao seu domínio verificado*

Usuários internos possuem um e-mail de um domínio reivindicado pela sua conta Enterprise. Por exemplo, `user@acme.com` onde `acme.com` é um dos seus domínios verificados.

Usuários externos possuem um e-mail fora de qualquer domínio reivindicado pela sua conta Enterprise. Por exemplo, `user@not-domain.com` onde `not-domain.com` não é um dos seus domínios verificados.

:::note
Os detalhes do usuário são visíveis no perfil do usuário. No console de admin, os detalhes do usuário também são visíveis na lista de usuários, onde você pode optar por filtrar por classificação **Interna** ou **Externa**.
:::

A classificação interna ou externa é automática e baseada em se o domínio do usuário é reivindicado e verificado pela sua conta Enterprise.

## Consolidação de times autônomos no plano Enterprise

Se você for Admin da empresa, pode incluir todos os times criados com seus domínios no seu plano Enterprise. Ao reunir todos os times em um só lugar, você fortalece a segurança, melhora a colaboração e facilita o gerenciamento. Além disso, você também pode fazer uma auditoria dos domínios para identificar e consolidar usuários e times que fazem parte do seu domínio gerenciado, mas que ainda não estão incluídos na sua assinatura.

Para mais informações, [consulte a documentação sobre Consolidação de Times](../../managing-enterprise-teams-and-content/06-self-serve-teams-to-enterprise-plan-consolidation.md).

## Solicitações de alteração de e-mail

Se sua empresa reivindicou um domínio, nenhum usuário associado a esse domínio poderá alterar seu endereço de e-mail na Miro sem a aprovação do Admin da empresa. Ao tentar alterar o e-mail, os usuários receberão a seguinte mensagem de erro: **Você não pode alterar seu e-mail para ou de um domínio que pertence a uma organização**. Recomendamos que os usuários entrem em contato com o Admin da empresa, que pedirá assistência ao suporte da Miro.

## Perguntas frequentes

Posso usar o controle de domínio com um subdomínio?

Sim, os subdomínios são tratados como entidades separadas dos domínios primários. Siga o processo de configuração de cada subdomínio que queira verificar.

Como usar o logon único com o controle de domínio?

Você precisará configurar o controle de domínio antes de habilitar a autenticação por [logon único](../../security-integrations/single-sign-on-sso/09-single-sign-on-(sso).md).

E se meu nome de domínio mudar ou eu quiser adicionar um subdomínio?

Se seu nome de domínio mudar, exclua o domínio e reinicie o processo de verificação com o novo domínio ou subdomínios adicionados.

Onde encontro os registros DNS para meu domínio?

Para localizar os registros DNS do seu domínio, será necessário acessar a plataforma do registrador onde o seu domínio foi registrado. Se você não tem certeza de quem é o registrador do seu domínio, pode encontrar essa informação usando o **who.is** para pesquisar o domínio. Uma vez identificado o registrador, faça login no site dele e navegue para a seção geralmente rotulada como **Domínios** ou **Gerenciamento de DNS**. Lá, você encontrará as configurações ou registros de DNS do seu domínio.

Por que não consigo ver **Domínios gerenciados** nas minhas configurações de **Segurança e conformidade**?

Se você não consegue ver a opção **Domínios gerenciados**, isso pode ocorrer por dois motivos:

- Você não está em um plano Enterprise que inclui essa funcionalidade.
- Você não tem a função de Admin da empresa para acessar essa configuração.

Verifique os detalhes do plano e a função com um Admin da empresa para mais informações.

Posso excluir o registro TXT para meu domínio depois que ele for verificado?

Embora a exclusão do registro TXT após a verificação não afete imediatamente a operação do seu controle de domínio, é recomendável manter esse registro. Manter o registro TXT é crucial para futuras verificações. A remoção do registro TXT pode complicar novas verificações e exigir novamente todas as etapas de verificação.
