---
title: Obsoleto – Configurar e desabilitar cartões do Jira usando OAuth 1.0
article_id: 360019501754
translation_id: 14537291781906
locale: pt-br
sidebar_position: 14
created_at: '2023-10-19T15:22:39Z'
updated_at: '2025-11-25T16:03:58Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Disponível para: Jira Cloud, servidor do Jira (no local) e Datacenter (também
    protegido por LDAP) Configurado por: Admin do time da Miro e administrador do
    sistema Jira com permissões administrativas de projeto'
---

:::note
O método de autenticação OAuth1.0 não será mais compatível com a Miro a partir de 31 de julho de 2025. OAuth1.0 é um [protocolo de autenticação obsoleto no Jira](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively.) e não deve ser usado. Esta mudança faz parte de uma transição mais ampla para o OAuth2.0, que é recomendado em consonância com as melhores práticas de segurança. Os usuários são aconselhados a migrar para o OAuth2.0 para garantir suporte contínuo e compatibilidade com os serviços da Miro.
:::

## Configurando a Miro no Jira

:::warning
Se surgirem quaisquer problemas técnicos, consulte nosso artigo sobre [Possíveis problemas e como resolvê-los](https://help.miro.com/hc/articles/360017572654).
:::

:::tip
Saiba mais sobre cartões do Jira nos artigos [Perguntas Frequentes sobre cartões do Jira](https://help.miro.com/hc/articles/360013463739) e [Como configurar webhooks para cartões do Jira](https://help.miro.com/hc/articles/360017731113).
:::

Configuração do Jira Cloud Servidor Jira e Jira Data Center

:::note
Observe queos menus do Jira podem variardependendo da versão do Jira que você está usando, no entanto, o fluxo geral deve ser o mesmo. As instruções abaixo também podem ser encontradas no [Suporte Atlassian](https://confluence.atlassian.com/adminjiraserver071/using-applinks-to-link-to-other-applications-802592232.html).
:::

### Etapa 1 - Link do aplicativo

Primeiro, crie um link de aplicativo e configure-o.

1. Vá para **Configurações do Jira** > **Produtos** > **Integrações** > **Links de aplicativos** > **Criar link:
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)***Observe que a interface do Jira pode diferir dependendo da sua versão do Jira*
2. Escolha **Link de aplicação direta** e insira `https://miro.com/` no campo **URL do Aplicativo**.
   Importante: você deve inserir o URL exatamente neste formato. Clique em **Continuar**.
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)
    *Criando o link*
3. No próximo menu, basta clicar em **Continuar** novamente.
4. No menu **Link de revisão**, verifique se o URL ainda é exatamente `https://miro.com/` e insira o **nome do aplicativo** de sua escolha. Role para baixo e, no final, marque a caixa **Criar link de entrada**. *Pule o restante dos campos* e clique em **Continuar**.
   ![mceclip3.png](../../../../../../docs/integrations-apps/atlassian/images/21017004819346_mceclip3.png)  *Apenas o campo Nome da Aplicação deve ser preenchido*
5. Aqui você verá os campos para os valores da Miro. Para obter os valores, faça login na Miro.
   - Para integração no nível do time, vá para **[Configurações do time](https://help.miro.com/hc/articles/360021841280)**>**Apps e integrações**>**Cartões do Jira.**
   - Para integração no nível da organização, acesse [**Configurações da empresa**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **Apps** > **Gerenciar apps** > **Cartões do Jira** > **Configurações**.
     > Se você não tiver cartões do Jira na sua lista de aplicativos, role até o topo da seção, clique em **Instalar aplicativos** e prossiga para instalar o aplicativo do Marketplace da Miro. Depois de ver os cartões do Jira na lista, clique para abri-lo.


     A guia do plugin será aberta, e você poderá ver **Passo 1** para obter os valores necessários:

     ![Jira_Cards_values.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017515668626_Jira Cards values.jpg)*Valores dos cartões do Jira*
     Copie os valores e adicione-os ao menu **Review Link** da Atlassian.
6. Você verá a mensagem de processamento por um ou dois momentos:
   ![mceclip4.png](../../../../../../docs/integrations-apps/atlassian/images/21017528655634_mceclip4.png)
    *A última etapa da criação do link*

Isso conclui as etapas do lado da Atlassian. O link aparecerá na lista dos seus links de Aplicações.

### Etapa 2 - Conexão

Volte para as configurações do seu cartão do Jira na Miro, e choose uma das duas opções: crie um webhook manualmente ou automaticamente. Se você escolher manualmente, desmarque a opção. Por favor, veja mais informações [neste artigo](https://help.miro.com/hc/articles/360017731113). Recomendamos fortemente o uso do webhook automático, assim você não precisa redefini-lo em caso de grandes atualizações no plugin.

Por fim, insira seu URL do Jira e clique em **Conectar:**

![step_2.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017528650898_step%202.jpg)*Conectando cartões do Jira*

Para obter a URL do Jira, copie o URL base da sua instância do Jira. Aceitamos os seguintes formatos:

`https://your-server.example.com/`
[https://your-server.example.com/
https://your-ip-address/](https://your-server.example.com/)[https://your-ip-address/](https://your-server.example.com/)

Se o seu URL do Jira não for aceito, consulte [este artigo.](https://help.miro.com/hc/articles/360017572654) Também verifique se a Miro tem acesso suficiente ao seu Jira para [estabelecer a conexão.](https://help.miro.com/hc/articles/360017572694)

Agora você conectou sua instância do Jira ao seu time na Miro.

:::warning
Embora a Atlassian tenha descontinuado o suporte para o Jira Server a partir de fevereiro de 2024, a Miro continuará a oferecer suporte à integração com os cartões do Jira para o Jira Server por tempo indeterminado.
:::

1. Vá para `https://your-jira-server/plugins/servlet/applinks/listApplicationLinks`[.](https://your-jira-server/plugins/servlet/applinks/listApplicationLinks) Se "Links de aplicação" não estiver selecionado, clique nele. ![jira_server_create_application_links.png](../../../../../../docs/integrations-apps/atlassian/images/21017515683858_jira_server_create_application_links.png)*Links de Aplicativos do Jira Server*
2. Clique em **Criar link**. Selecione "Atlassian product" e forneça o **Application URL**, "https://miro.com". Clique em **Continuar**. ![jira_server_create_link.png](../../../../../../docs/integrations-apps/atlassian/images/21017528656274_jira_server_create_link.png)*Configurando o URL da Aplicação*
3. Você será levado para a caixa de diálogo "Vincular aplicativos". Adicione um **Nome do Aplicativo** (ou seja, Miro cartão do Jira), e selecione "Aplicativo Genérico" para **Tipo de Aplicativo**.
   Você deve ver a URL do seu aplicativo Jira em "Você está criando um link de:", e deve ver `https://miro.com` em "Para este aplicativo:". Clique em **Continuar**.![jira_server_link_applications.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017528658834_jira_server_link_applications.jpg)*Configurando os detalhes do aplicativo Link*
4. A configuração do link será processada. Quando isso terminar, você verá seu novo link na área "Application links" do Jira Server. ![jira_server_application_links_created.png](../../../../../../docs/integrations-apps/atlassian/images/21017515685522_jira_server_application_links_created.png)*Seu aplicativo configurado no Jira Server*
5. Em seguida, você precisará configurar os detalhes do seu aplicativo. Clique no ícone de lápis do seu aplicativo para editar os detalhes do aplicativo.
6. Na caixa de diálogo Configurar, clique na opção **Autenticação de entrada**. Preencha o **Consumer Key, Consumer Name, Public Key** e, opcionalmente, uma descrição.
   - Para integração no nível do time, esta informação está disponível em [**Configurações do time**](https://help.miro.com/hc/articles/360021841280) > **Apps e Integrações** > **Cartões do Jira**.
   - Para integração em nível de organização, esta informação está disponível em [**Company settings**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **Apps** > **Gerenciar apps** > **Cartões do Jira** > **Configurações**.
     ![jira_server_config_oauth.png](../../../../../../docs/integrations-apps/atlassian/images/21017528687506_jira_server_config_oauth.png)*Configurando detalhes de autenticação de entrada no Jira Server*
     ![jira_webhooks_jira_server_config.png](../../../../../../docs/integrations-apps/atlassian/images/21017515686418_jira_webhooks_jira_server_config.png)*Detalhes do link de aplicação do Jira na Miro*
7. Role até o final das opções de autenticação de entrada e clique em **Salvar**. Seu status de verificação agora deve estar confirmado, e este servidor do Jira agora pode ser usado dentro da Miro para uso com cartões do Jira. Certifique-se de escolher "Jira Server" e "OAuth 1.0" no lado da Miro.![jira_server_welcome_to_jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017515690258_jira_server_welcome_to_jira.png)

### Autorização do usuário

Após a integração ser conectada, cada um dos seus usuários finais precisa conectar seu perfil pessoal do Jira para estabelecer as permissões adequadas - isso garante que o acesso de cada usuário na Miro seja *exatamente o mesmo que na sua instância do Jira*. Quando os usuários finais tentarem importar ou editar um cartão do Jira pela primeira vez, será solicitado que façam login no Jira usando suas credenciais individuais.

Depois disso, os usuários podem adicionar tarefas como cartões na lousa. Todas as alterações feitas no Jira são refletidas nos cartões do Jira no board.

:::note
Se um usuário não tiver credenciais do Jira e tiver acesso ao board no qual o cartão foi adicionado, ele verá o título do cartão, tipo de item, prioridade, responsável e todos os atributos configurados para serem mostrados no cartão do Jira. No entanto, não poderão expandir o cartão para ver outros atributos e editá-lo, a menos que autorizem. Se o usuário não se conectar às suas credenciais do Jira, ele não verá o avatar do responsável e a aparência geral do cartão será diferente.
:::

### Usando uma instância do Jira para vários times da Miro

Você pode instalar Cartões no nível do time ou da organização. Se você tiver vários times, poderá aproveitar as configurações no nível da organização para evitar repetir o procedimento de configuração para cada time. O link de aplicativo existente é usado para todos os times.

Após conectar seu time ou organização a uma instância do Jira, um novo WebHook é criado nos seus WebHooks do Jira para esse time ou organização da Miro. Criar um webhook estabelece um canal para solicitações de atualização.

Se você especificar configurações no nível da organização, times que já estão conectados mantêm suas configurações atuais. No entanto, eles podem mudar para as configurações ao nível da organização a qualquer momento.

Além disso, se necessário, os times podem substituir as configurações no nível da organização para se conectar a uma instância diferente do Jira.

Se você é um cliente Enterprise que deseja migrar várias conexões em nível de time para a conexão padrão em nível de organização, entre em contato com seu time responsável pela conta.

:::warning
Se você deseja conectar vários times de forma separada, recomendamos dar ao webhook de cada time um nome único. Vá para a página de WebHooks do seu Jira e edite cada webhook recém-criado.
:::

Conectar várias instâncias do Jira a um time da Miro não é compatível.

## Desabilitar o plugin

Para integração a nível de time, vá para **Configurações do time** > **Aplicativos e integrações** > **Cartões do Jira**. Em seguida, selecione **Remover para o time**.

Para integração em nível de organização, para restringir o uso do aplicativo Jira, vá para **Configurações da empresa** > **Aplicativos** > **Gerenciar aplicativos** > **Cartões do Jira**. Em seguida, mova a opção para a posição desligada.

:::warning
Se você desabilitar o Jira para a organização, os usuários de todos os times Enterprise não poderão usar os cartões do Jira. Para saber mais sobre o gerenciamento e a restrição de aplicativos, consulte [Gerenciamento do aplicativo](https://help.miro.com/hc/articles/4404659741458).
:::

**Mais informações:** Veja [Como usar cartões do Jira](https://help.miro.com/hc/articles/360017572434).
