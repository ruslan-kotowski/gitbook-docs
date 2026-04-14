---
title: CA Agile Central (Rally)
article_id: 360017731133
translation_id: 360017731133
locale: pt-br
sidebar_position: 4
created_at: '2019-02-11T10:13:34Z'
updated_at: '2025-11-25T16:02:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: rally-cards
---

Aproveite as vantagens do CA, software e metodologia ágil líderes do setor, diretamente no board. Converta suas tarefas do CA Agile Central em cartões úteis e aproveite a priorização de backlog, o mapeamento de histórias e outras atividades em equipe que ajudam seu time a desenvolver rápido projetos consistentes com alta qualidade.

> **Disponível para:** [Plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)

## Conexão do CA Agile

A autorização do CA Agile é realizada por meio do protocolo OAuth 2.0 (concessão do código de autorização) e todas as solicitações são feitas por SSL. Há dois níveis de conexão entre seus dados da Miro e sua conta do CA Agile Central: nível de perfil do usuário e nível de time.

É importante observar que a conexão com o CA Agile é apenas unidirecional: CA Agile --> Miro. Você pode importar os cartões para um board da Miro e editá-los por meio do botão Fonte, conforme descrito abaixo na seção Edição de cartões. Você não pode editar os cartões do CA Agile diretamente na Miro.

### Nível do time

> **Configurado por:** Admins do time

:::warning
É importante ressaltar que, para cada time na Miro, você deve usar contas de usuário diferentes do Rally para conectar a mesma instância do Rally.
:::

Para estabelecer a conexão no nível do time, o admin do time deve encontrar o aplicativo **CA Agile** no [Marketplace da Miro](https://miro.com/marketplace/) e instalá-lo para o time: clique em **Get app (Obter aplicativo)**, selecione um time e clique em **Install & authorize (Instalar e autorizar)**.

![install_Rally_for_a_team.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416392594_install%20Rally%20for%20a%20team.jpg)
*Como instalar o Rally para um time*

Você também pode instalar o aplicativo diretamente de um board:

1. Na barra de criação, selecione **Ferramentas, mídia e integrações** (**+**).O painel **Ferramentas, mídia e integrações** será exibido.
2. Na guia **Ferramentas,** pesquise e selecione CA Agile.
   O painel do **CA Agile** será exibido.

![ca-agile-entry-point.png](../../../../../../docs/integrations-apps/more-integrations/images/21537455155858_ca-agile-entry-point.png)
*Instale o aplicativo a partir de um board*

Em seguida, abra as **Configurações do time > Aplicativos e integrações** e **Conecte**a integração daí. Se sua conexão não for autorizada no Rally, será solicitado que faça login na sua conta do Rally.

![connect_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416393874_connect%20Rally.jpg)
*Como conectar a integração no nível do time*

Durante esta configuração, um webhook é criado no lado do Rally, que envia atualizações à Miro para os cartões importados.

Quando a integração é configurada no nível do time, qualquer membro do time pode visualizar os cartões do Rally importados por outros participantes nos boards, além do estado atual dos cartões.

Vale ressaltar que a conta do Rally usada ao configurar a integração no nível do time deve ter acesso a todos os projetos do Rally a partir dos quais os cartões serão importados. Se qualquer projeto do Rally não estiver acessível para essa conta, os cartões importados desse projeto não serão atualizados no board e serão exibidos como congelados para todos os usuários do time.

### Nível de perfil

> **Configurado por:** cada usuário

:::warning
Antes de conectar a integração, certifique-se de fazer login no Rally em uma guia separada do navegador.
:::

Se um usuário quiser importar os cartões do Rally no board por conta própria, também deverá configurar a integração no nível de perfil. Para conectar seu perfil da Miro, abra as [Configurações de perfil](https://miro.com/app/account/profile/), vá até **Integrações**, encontre o **CA Agile Central (Rally)** e clique em **Conectar**:

![connect_Rally_on_profile_level.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429433746_connect%20Rally%20on%20profile%20level.jpg)
*Como conectar a integração no nível de perfil*

Quando a conexão no nível de perfil é estabelecida, o usuário pode usar o ícone do Rally na barra de ferramentas e abrir o seletor da galeria do Rally. O usuário pode ver todos os elementos do Rally (histórias de usuários, tarefas, defeitos) disponíveis para a conta do Rally usada para configurar a integração no nível do perfil. Em outras palavras, ao usar o seletor do Rally, o usuário poderá importar apenas os itens que estão disponíveis para essa conta no Rally.

## Como adicionar os cartões do CA Agile ao board

Para adicionar um cartão ao board, basta copiar o endereço URL da tarefa e colá-lo no board (as [combinações de atalho](https://help.realtimeboard.com/support/solutions/articles/1000206698-shortcuts-hotkeys) padrão também funcionam).

Para filtrar tarefas ou adicionar cartões em massa, escolha o**CA Agile**na barra de ferramentas de criação.

Você verá o seletor do CA Agile Central, onde poderá definir os filtros de pesquisa, como Project (Projeto), Type (Tipo), Iteration (Iteração), Release (Versão), etc. Escolha um ou vários e clique em **Export (Exportar)**:

![Rally_picker.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416397714_Rally%20picker.jpg)
*Seletor do CA Agile Central*

As tarefas serão adicionadas automaticamente ao board. Se o nome da tarefa for longo, arraste a parte inferior do cartão para vê-lo por extenso.

*![Rally_cards_on_the_board.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398482_Rally%20cards%20on%20the%20board.jpg)
Cartões do Rally no board*

> Observe que a integração do Rally da Miro não oferece a possibilidade de criar ou editar diretamente os cartões do Rally na Miro.

## Edição de cartões

Para editar o conteúdo do cartão, clique no link da fonte no cartão:

![Rally_card_source.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398866_Rally%20card%20source.jpg)
*O ícone de edição no cartão*

A tarefa da fonte será aberta em uma nova guia, onde poderá ser editada. Todas as alterações são aplicadas ao cartão no mesmo instante.

## Como desabilitar a integração

Para remover a conexão com suas iterações do Rally, você deve **Desabilitar**a integração e **Desinstalá-la** nas **Configurações do time > Aplicativos e integrações**.

![uninstall_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429436562_uninstall%20Rally.jpg)
*A opção para desabilitar a integração*

## Possíveis problemas e como resolvê-los

1. *O seletor da Miro-Rally não está mostrando alguns dos meus projetos.*
   - Nossa integração com o Rally usa o [seletor do SDK do Rally](https://rally1.rallydev.com/docs/saas/apps/2.1/doc/index.html#!/api/Rally.ui.picker.project.ProjectPicker) para preencher os dados e só funciona com projetos de estado Open (Aberto). Infelizmente, isso não é personalizável. Para exibir um projeto na Miro, altere seu status para Open (Aberto).
2. *As atualizações dos cartões ou campos de alguns cartões não estão em sincronia com a Miro.*- Se você estiver usando a integração dos cartões do Rally com vários times da Miro, verifique se todos os times estão conectados à sua instância do Rally usando uma conta de usuário *diferente* do Rally. É possível que o problema com as atualizações do time escolhido esteja ocorrendo, porque as credenciais de conexão já estão sendo usadas em outro time da Miro. Reconecte a integração usando um ID de usuário diferente do Rally, se necessário.
3. *Carregamento interminável ao tentar abrir o seletor do Rally na Miro.*- Siga as etapas de solução de problemas abaixo.

   1. Abra o menu Subscription (Assinatura) ([https://rally1.rallydev.com/#/assinatura](https://rally1.rallydev.com/#/subscription)).

   2. Clique no menu suspenso **Actions (Ações)** e escolha **Edit (Editar)**.

   3. Role para baixo até o campo **CORS Allowed Origins (Origens permitidas do CORS)**.

   4. Digite `https://miro.com,https://*.miro.com` (`http://miro.com`) no campo.

   5. Clique em **Save & Close (Salvar e fechar)**.
