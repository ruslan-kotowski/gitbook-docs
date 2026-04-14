---
title: Conector Netskope para Miro Enterprise
article_id: 4415711060498
translation_id: 4415711060498
locale: pt-br
sidebar_position: 6
created_at: '2022-01-19T06:23:42Z'
updated_at: '2025-02-26T11:27:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

O conector personalizado Miro para Netskope permite visibilidade sobre eventos relacionados a vazamento de dados e permite gerenciar o seguinte tráfego dentro do Miro:

- Como baixar o backup do board

Este guia fornece etapas para configurar o Netskope para o plano Miro Enterprise e descreve a experiência do usuário .

> **Disponível para:** [Plano Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md)

### Crie um novo aplicativo da Miro no Netskope

Dentro da sua instância Netskope, vá para **Configurações > Security Cloud Platform > Definição de aplicativo** e clique em **NOVO APLICATIVO DE NUVEM**:

![novo_aplicativo_de_nuvem.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016020258834_new%20cloud%20app.jpg)
*Criando um aplicativo em nuvem no Netskope![](blob:https://miro.atlassian.net/8cb061a4-e184-4bd6-bb95-774cd34fc8e7#media-blob-url=true&id=78b7a8cb-792a-41da-bf16-b26ca4480059&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.08.43.png&size=181298&height=513&width=1028&alt=)*

Para criar um novo aplicativo dentro do Netskope, você será solicitado a importar o seguinte arquivo JSON **miro-activities-for-netskope.json**:

```
Versão: 0.0.0.1.

"nome_de_domínio": "miro.com",
"uri_path": "/api/v1/ boards/.+/",
"método_http": OBTER
"uri_param": [{ "chave": "arquivo", "valor": "verdadeiro" }],
"código_resp": 200.
"padrão": "",
"nome_da_atividade": baixar


"nome_de_domínio": "miro.com",
"uri_path": "/api/v1/ boards/.+/recursos/.+/arquivos/original",
"método_http": OBTER
"uri_param": [],
"código_resp": 307.
"padrão": "",
"nome_da_atividade": baixar
```

Insira o nome do aplicativo, selecione a opção **Conector personalizado** e clique em **IMPORTAR DO ARQUIVO > Adicionar à lista de atividades** para carregar o arquivo **miro-activities-for-netskope.json** baixado na etapa anterior**.**

![carregando_o_arquivo.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016033728530_uploading%20the%20file.jpg)![](blob:https://miro.atlassian.net/f4beb3ad-27a3-49c8-baee-aa660161e315#media-blob-url=true&id=337f93cd-b545-47df-8f27-ca4fa5667a3f&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.14.30.png&size=207190&height=630&width=1039&alt=)
*Carregando o arquivo*

Após importar o arquivo **miro-activities-for-netskope.json,** as atividades registradas serão exibidas. Agora você pode clicar em **SALVAR** e criar o aplicativo da Miro.

![salvar_o_aplicativo.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016020260242_save%20the%20app.jpg)
*Salvando o aplicativo![](blob:https://miro.atlassian.net/b9da4e19-b3b1-4c25-aed3-762f458fd639#media-blob-url=true&id=f7549007-0265-42e1-b946-a3e167124f12&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.26.58.png&size=209044&height=693&width=1028&alt=)*

Depois que o aplicativo for criado, você precisa selecioná-lo e clicar em **APLICAR ALTERAÇÕES.**

*![aplicar_alterações.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016020260626_apply%20changes.jpg)**A opção de aplicar alterações ao aplicativo da Miro*

![](blob:https://miro.atlassian.net/82b8ac6e-1952-44e7-a62f-cefb7dbee6ab#media-blob-url=true&id=975f42e8-de5d-4bbb-ae07-c243cce9bb2f&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.32.06.png&size=257154&height=575&width=1780&alt=)

### Crie uma nova política para seu aplicativo da Miro no Netskope

Depois que o aplicativo for criado, você pode prosseguir para criar uma política. Para isso, você pode navegar até **Política >****Proteção em tempo real** e clicar em **NOVA POLÍTICA > Acesso a aplicativos na nuvem.**

![criar_uma_política.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016033731218_create%20a%20policy.jpg)
*Criando uma política para seu aplicativo da Miro![](blob:https://miro.atlassian.net/d2ae8479-8f5c-4417-8b09-2b57ee344d90#media-blob-url=true&id=e9c82ee5-cdea-4b33-8491-9613a848be81&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.39.02.png&size=107320&height=321&width=635&alt=)*

Aqui em **Destino,** você precisa fornecer o aplicativo da Miro criado na etapa anterior, configurar um **Nome de Política** e clicar em **SALVAR.**

*![salve_a_politica.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016020261906_save%20the%20policy.jpg)**Salvando a política*

![](blob:https://miro.atlassian.net/abf26593-27ad-40f4-b3e5-731a9e58d062#media-blob-url=true&id=0edd2e23-2762-4173-8f3f-9a7bb74bf217&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.45.14.png&size=200430&height=722&width=1575&alt=)Em seguida, você pode selecionar onde prefere colocar a apólice e clicar em **SALVAR.**

![](blob:https://miro.atlassian.net/370ad8f1-d9ac-40a2-a218-d132dde62914#media-blob-url=true&id=2db9fc4c-fd8d-47cf-a77b-f1fc02edbb15&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2019.27.01.png&size=77286&height=404&width=729&alt=)![move_policy.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016020262674_move%20policy.jpg)
*Selecionando onde você prefere colocar a apólice*

Por fim, você pode aplicar as alterações clicando no botão **APLICAR ALTERAÇÕES** .

![aplicando_alterações.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016020268434_applying%20changes.jpg)
*Aplicando alterações*

![](blob:https://miro.atlassian.net/41cdf802-aa1c-4f9a-bd22-950ea6ad755e#media-blob-url=true&id=7f85d987-6550-4271-90da-c9273a0cbc9a&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2019.29.17.png&size=157218&height=490&width=1576&alt=)

### Visualização de eventos

Depois que tudo estiver pronto, você pode visualizar o tráfego navegando até **o Skope IT**, filtrando pelo aplicativo da Miro personalizado e clicando em **Ver eventos** como segue.

![ver_eventos.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016033740306_see%20events.jpg)
*A opção de ver eventos de trânsito*

### Experiência do usuário

Os usuários para os quais as atividades de download devem ser bloqueadas precisam ter o cliente Netskope instalado em sua máquina. Quando os usuários tentam executar uma operação de backup de download, o Netskope bloqueia a ação e exibe um pop-up do sistema operacional nativo com uma mensagem.

![alerta.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21016033746578_alert.jpg)
*Uma mensagem mostrada aos usuários que não têm permissão para baixar um backup de uma board da Miro*
