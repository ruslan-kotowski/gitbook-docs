---
title: "Cart\xF5es do Asana (Legado)"
article_id: 360039492573
translation_id: 360039492573
locale: pt-br
sidebar_position: 1
created_at: '2019-11-25T10:03:42Z'
updated_at: '2025-11-25T16:05:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: asana-cards
---

:::warning
Esta página descreve nossa integração legada com o Asana. Para a nova integração, consulte a [documentação do Asana (Beta)](asana).
:::

**Principais Funcionalidades**

- Importe tarefas do Asana para os boards do Miro para visualizar o progresso da sua equipe
- Encontre tarefas específicas para importar diretamente do Miro usando filtros do Asana ou buscando pelo nome da tarefa
- Sincronização automática: todas as alterações feitas nas tarefas do Asana são automaticamente refletidas nos cartões do Asana no Miro

> **Disponível para**: Starter, Business, Enterprise planos. *Os administradores podem precisar autorizar o uso do Asana para seu time Miro. Os membros do time podem usar o aplicativo Asana Cards apenas se ele estiver instalado no nível do time.*

### Como instalar os cartões Asana

1. Primeiro, você precisará de uma conta ativa na Miro e uma conta ativa na Asana. Se você não tem um perfil Miro, cadastre-se [aqui](https://miro.com/signup/).
2. No Marketplace da Miro, abra [Cartões Asana](https://miro.com/marketplace/asana-cards/?backUrl=%2Fmarketplace%2F)*.* Clique no botão **Obter aplicativo**.
   Você será solicitado a selecionar o time em que deseja instalar o Asana. Selecione um time e clique em **Instalar e autorizar**.
   > ⚠️ Os usuários que não são admins não podem instalar o aplicativo, se isso não for permitido nas configurações.

![install_Asana_cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020254087442_install%20Asana%20cards.jpg)
*Autorização dos cartões Asana*

3. O próximo passo é clicar em **Conectar** nas configurações do aplicativo Cartões Asana.

![connect_Asana_and_Miro.jpg](../../../../../../docs/integrations-apps/asana/images/21020265147410_connect%20Asana%20and%20Miro.jpg)
*Configurações do aplicativo Cartões Asana nas configurações do time*
Outros membros do time encontrarão o ícone dos Cartões Asana na barra de ferramentas de criação do board e poderão conectar suas contas Asana a partir daí.

![Asana_cards_on_the_toolbar.jpg](../../../../../../docs/integrations-apps/asana/images/21020254085010_Asana%20cards%20on%20the%20toolbar.jpg)
*Cartões Asana na barra de ferramentas*

4. Permita que o Asana Connect acesse sua conta Asana. Se você não estiver logado no aplicativo no momento, será solicitado a autorizar-se no Asana.

**![grant_permission_to_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21020254090386_grant%20permission%20to%20Asana.jpg)*****Permitindo que a Miro acesse a conta Asana***

### Como importar e usar Cartões Asana

1. Depois de conectar a Miro com sua conta Asana, sinta-se à vontade para adicionar Cartões Asana aos seus boards da Miro. Para abrir o seletor, na barra de Criação selecione **Ferramentas, Mídia e Integrações** (**+**).Um painel se abrirá. Pesquise e selecione Cartões Asana.
2. O seletor oferecerá uma opção para filtrar tarefas. Primeiro, escolha um espaço de trabalho e depois filtre os cartões por Projetos, Tags ou Responsáveis. A lista de Projetos é ordenada por data de criação.

   > ⚠️ O seletor exibirá apenas as tarefas às quais você tem acesso no Asana. Se um usuário do Miro abrir a página de origem de uma tarefa à qual não tem acesso, verá uma mensagem de inacessibilidade.

   ![Asana_picker.gif](../../../../../../docs/integrations-apps/asana/images/21020254098578_Asana%20picker.gif)
   **Importando Cartões do Asana para um board**

Clique no botão **origem** para abrir o cartão no Asana.
![go_to_source.jpg](../../../../../../docs/integrations-apps/asana/images/21020265150226_go%20to%20source.jpg)
**Botão de origem do cartão**

Fique à vontade para adicionar seus cartões do Asana a frameworks de [Kanban](../../using-miro/advanced-tools/02-columns-formerly-kanban.md) e [mapa de histórias do usuário](../../using-miro/advanced-tools/07-user-story-mapping.md) simplesmente arrastando-os.

:::warning
Embora ainda não haja opção para criar ou editar Cartões do Asana no lado da Miro, todas as alterações feitas no Asana são sincronizadas na Miro (note que pode haver um pequeno atraso na atualização do cartão).
:::

![Asana_cards_and_kanban.gif](../../../../../../docs/integrations-apps/asana/images/21020254093074_Asana%20cards%20and%20kanban.gif)
*Adicionando Cartões do Asana ao Kanban*

### Alterar a cor de um cartão

Para alterar a cor de um cartão, clique no cartão ou cartões e escolha **cor de preenchimento** no menu de contexto. Se você duplicar o cartão, a nova cor será aplicada à cópia. ![asana_card_color.png](../../../../../../docs/integrations-apps/asana/images/21020254100242_asana_card_color.png)
*Alterando a cor de preenchimento de um cartão*

### Como desinstalar os cartões Asana

Para desinstalar os cartões Asana no nível de time, abra Configurações do time **> Aplicativos e Integrações > Cartões Asana**, role para baixo e clique em **Desinstalar para o time.**

**Se você deseja desinstalar o aplicativo no nível individual, clique em** **Desinstalar para mim.**

![uninstall_Asna_Cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020265153426_uninstall%20Asna%20Cards.jpg)
*Desinstalando os cartões Asana*

### Perguntas frequentes

1. *Quais IPs devem ser colocados na lista de permissões para os cartões Asana?*
   *-*18.203.61.162, 54.220.74.201, 54.216.81.236, 54.73.153.141, 52.215.228.26, 52.16.47.17, 54.217.180.21.
