---
title: Como configurar o ADFS SSO
article_id: 360022411353
translation_id: 360022411353
locale: pt-br
sidebar_position: 2
created_at: '2019-04-29T20:13:47Z'
updated_at: '2025-11-25T16:04:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Disponível para: planos Enterprise e Business** Configurado por: Admins
    da empresa'
---

O Miro oferece suporte a logins de logon único (SSO) por meio do SAML 2.0.

Um provedor de identidade (IDP) SAML 2.0 pode assumir muitas formas, incluindo um servidor ADFS (Active Directory Federation Services) auto-hospedado. O ADFS é um serviço fornecido pela Microsoft como uma função padrão para o Windows Server que fornece um login na Web usando credenciais existentes do Active Directory.

Este guia usa capturas de tela do **Server 2012R2**, mas etapas semelhantes devem ser possíveis em outras versões.

Primeiro, você precisa instalar o ADFS no seu servidor. A configuração e a instalação do ADFS estão além do escopo deste guia, mas são detalhadas neste [artigo da Microsoft](http://msdn.microsoft.com/library/gg188612.aspx).

Durante o teste, certifique-se de que a autenticação da sua estação de trabalho esteja definida para o mesmo e-mail de teste que você está usando para o teste, caso contrário, o ADFS não permitirá que você faça login, mesmo com a configuração e o perfil corretos.

> *💡 É altamente recomendável configurar o SSO em uma janela separada do modo anônimo do seu navegador.* Dessa forma, você mantém a sessão na janela padrão, permitindo que você desative a autorização SSO caso algo esteja mal configurado.

Se você deseja configurar uma instância de teste antes de habilitar o SSO na produção, solicite-o ao seu executivo de conta ou representante de Vendas . Somente aqueles que configurarem o SSO serão adicionados a esta instância de teste.

> **⚠️ Veja nosso artigo principal sobre SSO** [**aqui**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **para regras, recursos suportados e configuração opcional no Miro .**

## Etapa 1 - Adicionando uma Parte Confiável

1) Efetue login no servidor ADFS e inicie o **Console de gerenciamento do ADFS**.

2) Selecione a pasta**Relying Party Trusts**no**Gerenciamento do AD FS**e adicione um novo**Standard Relying Party Trust**na barra lateral**Ações**. Isso inicia o assistente de configuração para uma nova confiança.

![adicione_uma_parte_de_confiança.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941592082_add%20a%20party%20trust.jpg)
*Adicionando confiança partidária*

3) Na tela **Selecionar fonte de dados** , selecione a última opção, **Inserir dados sobre a parte manualmente.**

![passo_3.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928632850_step%203.jpg)
*Escolha **Inserir Dados Sobre a Parte Manualmente***

4) Insira um **nome de exibição** que você reconhecerá no futuro e quaisquer notas que queira fazer.

![nome_de_exibição.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941593362_display%20name.jpg)
*Adicionando um nome de exibição*

5) Selecione o botão **de perfil ADFS FS (ADFS 2.0)** .

![passo_5.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928636178_step%205.jpg)

![próximo.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941597458_next.jpg)
*Você será solicitado a procurar um Certificado para criptografar e descriptografar as declarações. Isso é opcional e pode ser ignorado pressionando **Avançar**.*

6) Marque a caixa**Habilitar Suporte para o protocolo SAML 2.0 WebSSO**.
A URL do serviço será https://miro.com/sso/saml.

**Observe** que não há barra final no URL.

![passo_6.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941598098_step%206.jpg)
*Habilitar Suporte para o protocolo SAML 2.0 WebSSO*

7) Adicione um **identificador de confiança da parte confiável** como `https://miro.com/`

![passo_7.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928638482_step%207.jpg)
*Adicionando um **identificador de confiança de parte confiável***

*Na próxima tela, você pode configurar a autenticação multifator, mas isso está além do escopo deste guia.*

![rejeitando_no_passo_7.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928640274_rejecting%20on%20step%207.jpg)
*Rejeitando a configuração* *da autenticação multifator*

8) Selecione o botão**Permitir que todos os usuários acessem esta parte confiável**.

![passo_8.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928642066_step%208.jpg)
*Permitir que todos os usuários acessem a parte confiável*

Nas próximas duas telas, o assistente exibirá uma visão geral das suas configurações.

Na tela final, use o botão**Fechar**para sair e abrir o editor **de Regras de Reivindicação** .

![etapa_final.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941603602_final%20step.jpg)
*Finalizando a adição de um Relying Party Trust*

Certifique-se também de que sua configuração inclui **Asserção Assinada**.

## Etapa 2 - Criação de regras de reivindicação

Depois que o trust da parte confiável for criado, você poderá criar as regras de reivindicação.
Por padrão, o editor de regras de reivindicação é aberto depois que você cria o trust.

1) Para criar uma nova regra, clique em**Adicionar regra**.

![adicionando_uma_regra.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928643858_adding%20a%20rule.jpg)
*Adicionando uma nova regra*

2) Crie uma regra**Enviar atributos LDAP como declarações**.

![modelo_de_regra_de_reivindicação.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928644370_claim%20rule%20template.jpg)
*Criando uma regra*

3) Na próxima tela, nomeie sua regra e, usando**o Active Directory**como seu armazenamento de atributos, mapeie da seguinte maneira:

| Atributo LDAP | Tipo de reivindicação de saída |
| --- | --- |
| Endereços de e-mail | Endereço de email |
| Nome dado | Primeiro nome |
| Sobrenome | Sobrenome |

![map_LDAP_attributes.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941606290_map%20LDAP%20attributes.jpg)
*mapeamento de atributos LDAP*

Clique em**OK**para salvar a nova regra.

4) Crie outra nova regra clicando**Adicione uma regra**, desta vez selecionando**Transformar uma reivindicação recebida**como template.

![adicionar_outra_regra.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941608594_add%20another%20rule.jpg)
*Selecionando **Transformar uma Reivindicação de Entrada** como template*

5) Em seguida, nomeie a regra e defina os seguintes parâmetros:

|  |  |
| --- | --- |
| **Tipo de reivindicação recebida** | Endereço de email |
| **Tipo de reivindicação de saída** | Nome ID |
| **Formato de ID de nome de saída** | E-mail |

![definir_parâmetros_de_regra.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928646546_set%20rule%20parameters.jpg)
*Definindo os parâmetros da regra*

Por fim, clique em**OK**para criar a regra de reivindicação e depois**em OK**novamente para finalizar a criação das regras.

Com isso a configuração do ADFS foi concluída! Depois disso, basta [habilitar o recurso SSO para seu plano Miro](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) e seus usuários finais poderão começar a usar SAML para autenticação no Miro.

## Testando a configuração do SSO no Miro

1. Conclua as etapas acima para configurar o SSO.
2. Clique no botão **Testar a configuração de SSO**.
3. Revise os resultados:

1. Se não houver nenhum problema, uma mensagem de confirmação **de que o teste de configuração do SSO foi bem-sucedido** será exibida.
2. Se forem encontrados problemas, uma mensagem de confirmação **de falha no teste de configuração do SSO** será exibida, seguida por mensagens de erro detalhadas para orientar você sobre o que precisa ser corrigido.

![teste-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Testando a configuração do SSO no Miro*
