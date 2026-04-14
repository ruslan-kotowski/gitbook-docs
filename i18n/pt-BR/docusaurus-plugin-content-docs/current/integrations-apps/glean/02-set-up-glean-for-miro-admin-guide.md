---
title: Configurar Glean na Miro (guia do admin)
article_id: 27581463837330
translation_id: 27581463837330
locale: pt-br
sidebar_position: 2
created_at: '2025-06-23T10:52:57Z'
updated_at: '2026-01-02T09:57:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Pré-requisitos

1. Você é um **Admin da Organização Miro** e um **Admin do Glean**.
2. No Glean, **registre um OAuth Client ID.** Leia a [documentação do Glean](https://developers.glean.com/api-info/client/authentication/oauth) para mais detalhes.
3. Ative a configuração de privacidade em nível de usuário **Permitir que o histórico de chat seja salvo por até 30 dias**.

## Instalar o app do Glean

Para começar, instale o app do Glean no Marketplace da Miro para os times relevantes em sua organização.

1. Vá para as configurações da sua **Empresa** e clique em **Aplicativos e Integrações**.
2. Na guia **Aplicativos**, clique em **Adicionar aplicativos** para abrir o Marketplace.
3. Pesquise por "Glean". Você também pode encontrá-lo copiando e colando seu ID de cliente na barra de pesquisa: `1202342442818548396`.
4. A partir do perfil do aplicativo, selecione onde adicionar o aplicativo: para **Todos os times** ou selecione **Times específicos...**.
5. Revise a página de permissões. O aplicativo Glean é desenvolvido e mantido pela Miro e não requer permissões específicas.
6. Selecione **Adicionar** para concluir a instalação.

## Configuração de Logon Único (Okta)

Se a sua organização usa Okta como fornecedor de Logon Único (SSO), você precisará criar uma aplicação Web Okta OpenID Connect (OIDC) antes de prosseguir para as próximas seções.

1. Crie um novo aplicativo Okta usando os passos mencionados na documentação [aqui](https://help.okta.com/en-us/content/topics/apps/apps_app_integration_wizard_oidc.htm).
   1. Selecione **OIDC - OpenID Connect** como o método de iniciar sessão.
   2. Selecione **Aplicação Web** como o tipo de aplicação.
   3. Certifique-se de que o **Token de Atualização** esteja habilitado nas configurações de **Tipo de concessão** > **Concessões principais**.
   4. Adicione `https://integrations.miro.com/api/external-auth/oauth2/callback` como os **URIs de redirecionamento para iniciar sessão**.
   5. Selecione **Salvar**.
2. Copie o **ClientId** e o **Client Secret** da seção de Credenciais do Cliente. Esses dados serão necessários nas próximas seções para completar a configuração da integração.

## Configure o logon único (SSO)

Siga estas etapas para configurar o aplicativo:

1. Na página **Apps & Integrations**, acesse **Gerenciar apps**.
2. Encontre "Glean" na sua lista de apps instalados e clique em **Configurações**. Se você não visualizar o app, pesquise-o pelo ID do cliente (`1202342442818548396`) e aprove-o primeiro.
\{1>OKTA<1\}3. Clique em **Salvar** para aplicar a configuração.

:::note
Se você estiver usando Azure, certifique-se de que seu admin do Microsoft Entra tenha selecionado "Consentir em nome da sua organização" para o app do Glean no centro de administração do Microsoft Entra, permitindo que os usuários autentiquem corretamente.
:::

## Configurar o console de admin do Glean

Antes de usar o Glean na Miro, você precisa configurar o acesso baseado em token OAuth no seu console de admin do Glean.

1. Abra seu **console de admin do Glean** e navegue para **Configurações** > **Acesso de terceiros (OAuth)**.
2. Na seção **OAuth Configurado-IDP**, ative **Ativar OAuth IDP para acesso API**.
3. Clique em **Gerenciar Configurações**, selecione seu **provedor SSO**.
4. Preencha os detalhes do provedor com base no seu provedor de logon único.
   - **Okta**
     - URL do Servidor de Autorização: `https://<subdomínio>.okta.com`
     - ID(s) de cliente permitido(s): ID do cliente do aplicativo Okta criado na seção anterior.
     - O restante dos campos do formulário pode ser deixado em branco.
   - **Azure**
     - Subdomínio do emissor: `https://login.microsoftonline.com/<tenant-id>/v2.0`
     - ID(s) do cliente permitido(s): `a49fdb25-3b5f-4d3b-bedf-6da7be2b4bf4`
   - **GSuite**
     - ID(s) do cliente permitido(s): `1062019541050-pf2ndc9f3o4lrmkupj3cj0fep5hkecns.apps.googleusercontent.com`
5. Selecione **Salvar** para aplicar as configurações.

> ⏰ **Nota:** Pode levar até 30 minutos para que as alterações entrem em vigor no console de admin do Glean.

## Use o app do Glean

Após a instalação e configuração do app, os usuários nos times designados poderão começar a usá-lo. Na primeira vez que um usuário abrir o app do Glean na Miro, será solicitado que ele se autentique.

1. Abra um board da Miro e clique no ícone do Glean na barra de ferramentas para abrir o painel lateral.
2. Clique em **Conectar Glean** para iniciar a autorização.
3. Um diálogo de autorização de logon único aparecerá.
4. Após a autenticação bem-sucedida, a interface do usuário do Glean aparecerá, pronta para uso.

## Segurança

Para mais informações sobre dados e segurança, consulte este [documento de segurança](https://docs.google.com/document/d/1lGLF7eASQb2uMRmMEAaH-GzFhyz4UKfwMeqSQOSYPdM/edit?tab=t.0#heading=h.gu9ng058yy7y).
