---
title: Adicionando vários provedores de identidade
article_id: 16287287497234
translation_id: 16287287497234
locale: pt-br
sidebar_position: 1
created_at: '2024-01-10T10:51:24Z'
updated_at: '2026-02-18T08:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponível para: Enterprise Configurado por: Admins da empresa'
---

:::note
Adicionar vários provedores de identidade é uma funcionalidade privada disponível exclusivamente para clientes Enterprise. Para acessar e ativar esta funcionalidade, entre em contato com seu Gerente da Conta da Miro ou Gerente de Sucesso do Cliente. O Suporte da Miro não pode ativar esta funcionalidade.
:::

Use vários provedores de identidade (IdPs) para logon único (SSO). Isso é especialmente útil para grandes organizações com diferentes filiais ou subsidiárias, cada uma com seu próprio IdP, mas que precisam de acesso à mesma assinatura da Miro.

## Preparando-se para adicionar vários provedores de identidade

Para garantir que o [logon único (SSO)](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) continue funcionando após adicionar vários aplicativos de provedores de identidade, você precisa atualizar a configuração do aplicativo IdP existente.

O Entra ID e alguns outros IdPs não oferecerão suporte ao novo formato de configuração até que sua organização ative a funcionalidade de múltiplos provedores de identidade (multi-IdP). Para evitar interrupções de login, sugerimos agendar uma ligação com seu Gerente de Sucesso do Cliente, que pode orientá-lo passo a passo para habilitar a funcionalidade de multi-IdP ao mesmo tempo em que a configuração é atualizada.

### Como configurar suas configurações de Enterprise

1. Desativar SCIM.
2. Atualizar a configuração do logon único.
3. Verificar sua funcionalidade do logon único.

#### Desativar SCIM

Atualmente, não damos [suporte](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) a SCIM com múltiplos IdPs. Para desativar o SCIM no seu plano Enterprise, vá até as configurações de **Empresa** > **Conta** > **Integrações Enterprise**, e desative a **Provisionamento SCIM**.

#### Atualizar a configuração do SSO

**Configuração antiga**

É provável que, quando o SSO da Miro foi configurado originalmente no seu IdP, os seguintes valores de configuração tenham sido usados:

- **URL de retorno de chamada/ACS:** https://miro.com/sso/saml
- **ID de entidade:** https://miro.com

**Nova configuração**

Para garantir que o IdP saiba a qual configuração da Miro ele se refere, os valores abaixo precisam ser atualizados. Vá para **Configurações** > **Segurança** > **Autenticação**.

Esses valores estarão disponíveis nas configurações de logon único assim que sua organização habilitar a funcionalidade de multi-IdP privado e terão o seguinte formato:

- **URL de retorno de chamada/ACS:** https://miro.com/sso/saml/&lt;org_id&gt;/&lt;saml_settings_id&gt;
- **ID da entidade:** https://miro.com/&lt;org_id&gt;/&lt;saml_settings_id&gt;

![Callback URL and Entity ID in the Enterprise admin console](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/23763575205778_image.png)

*URL de retorno de chamada e ID da entidade no console de admin do Enterprise*

#### Verifique a funcionalidade do seu logon único (SSO)

Depois de terminar de atualizar a configuração do seu provedor de identidade (IdP), teste se o logon único (SSO) está funcionando corretamente efetuando logout e login novamente.

## Adicionando um novo provedor de identidade (IdP)

O processo para adicionar novos IdPs é semelhante à configuração de [logon único](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) existente, mas inclui algumas alterações importantes:

- **Novos campos:** "Nome do IdP" e "Descrição do IdP" (opcional). Esses campos ajudam usuários e admins a identificar o IdP correto durante o login, especialmente se vários IdPs forem usados.

  Como esses campos são exibidos nas configurações do admin e podem ser mostrados aos usuários quando eles fazem login via logon único, recomendamos definir esses nomes intencionalmente (por exemplo, Business Unit ou nome do IdP).

  ![idP-name-and-IdP description.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016020733970_idP-name-and-IdP%20description.png)
*A opção de adicionar um nome e uma descrição do IdP*
- **Campos somente leitura:** 'Callback URL' (URL de Retorno Permitida, URL do Serviço de Consumidor de Asserção Personalizado, URL de Resposta) e 'ID da Entidade' (Identificador, Identificador de Confiança da Parte Confiável) agora são gerados automaticamente nas suas configurações do IdP da Miro quando sua organização habilita a funcionalidade privada de múltiplos IdPs.

  Anteriormente, esses valores eram estáticos, pois eram os mesmos para todas as configurações de IdP. Uma vez gerados, você também precisará copiar e colar esses valores nos campos correspondentes nas configurações do seu provedor IdP.

  ![Callback-ID-and-Entity-ID-fields.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034166290_Callback-ID-and-Entity-ID-fields.png)
*Campos de URL de Retorno e ID da Entidade*

## Gerenciando vários provedores de identidade (IdPs)

> **💡** Você pode adicionar e habilitar até 20 provedores de identidade por vez.

Depois de adicionar os IdPs, cada configuração pode ser ativada ou desativada conforme necessário. Para desativar um IdP, vá para as configurações da **Empresa** > **Conta** > **Autenticação** e desative o IdP.

![Toggle-on-or-off-IdPs.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034165010_Toggle-on-or-off-IdPs.png)
*A opção para ativar ou desativar um IdP*

## Visualização de iniciar sessão para domínios de e-mail com vários IdPs

Se o domínio de e-mail de um usuário estiver vinculado a várias configurações de IdP, ele poderá selecionar uma durante o iniciar sessão. Se essas configurações tiverem domínios distintos, o usuário é roteado automaticamente para o IdP relevante.

![sso-screenshot.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/22437449166610_sso-screenshot.png)
*Visualização de vários IdPs ao iniciar sessão*
