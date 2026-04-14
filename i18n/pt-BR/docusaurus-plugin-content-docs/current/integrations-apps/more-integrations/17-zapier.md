---
title: Zapier
article_id: 360025942994
translation_id: 360025942994
locale: pt-br
sidebar_position: 18
created_at: '2019-07-04T17:26:16Z'
updated_at: '2025-02-26T12:10:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Conecte seus aplicativos favoritos ao Miro via Zapier, expandindo a lista de possibilidades para automatizar suas tarefas diárias. Mova informações entre seus aplicativos e boards automaticamente para que você possa se concentrar no trabalho mais crucial.

> **Disponível em:** planos Free, Starter, Business e Enterprise

## Criando um Zap com Miro

Para conectar o Miro a outros aplicativos via Zapier, você precisa ter uma conta Zapier.

Para criar um Zap, clique no botão correspondente no [painel do Zapier](https://zapier.com/app/dashboard).

![Criar_Zap.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017005247378_Create%20Zap.jpg)
*Botão Criar Zap*

O Zapier cria um fluxo de trabalho automatizado entre aplicativos com **gatilhos** e **ações**.

:::warning
Agorao Miro só pode funcionar como uma **Ação** no Zapier.
:::

**Acionar**

Um gatilho é um evento em um aplicativo que inicia o Zap. Depois de configurar um Zap, o Zapier monitorará o aplicativo em busca desse evento. No exemplo "Salvar novos eventos no Google Agenda nos widgets de cartão do Miro ", o Zap é acionado somente quando um novo evento é criado no Google Agenda.

![novo_gatilho_de_evento.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017005250578_new%20event%20trigger.jpg)
*Configurando um evento Trigger no Zap*

**Ação**

Uma Ação é um evento que completa o Zap. No exemplo anterior "Salvar novos eventos no Google Agenda nos widgets de cartão Miro ", novos cartões Miro se comportarão como uma Ação.

:::warning
Agorao Miro funciona apenas como uma Ação no Zapier.
:::

Encontre Miro e escolha uma das três Ações: Copiar board, Criar board, Criar widget de cartão.

![criando_um_Zap_com_Miro_como_uma_ação.gif](../../../../../../docs/integrations-apps/more-integrations/images/21016967717138_creating%20a%20Zap%20with%20Miro%20as%20an%20action.gif)
*Criando seu próprio Zap com Miro como ação*

### Ação do board de cópia

É uma ação projetada para criar uma cópia de um board específico. Você precisará selecionar um time onde a cópia do board será criada.

![instalar_Zapier.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21016967717522_install%20Zapier.jpg)
*Selecionando uma time Miro*

Na próxima etapa, escolha os seguintes parâmetros:

- board original - escolha um board da time para fazer uma cópia. Você pode pesquisar o board pelo seu nome ou ID *(*por exemplo *o9J_rxLXasqA).*Se você não encontrar um board na lista, tente recarregar os dados e verifique novamente
- Título - insira um nome de título para a cópia do board . Se você deixar o campo em branco, o board será criado com o nome **Untitled**
- Descrição - insira o texto para a descrição do board
- Acesso da Team - você pode escolher entre os tipos de acesso da time ao board **Privado**, **Visualizar**, **Comentar** e **Editar**
- Acesso via link - crie regras para compartilhar este board com um link. Você pode definir grupos de acesso **Privado**, **Visualizar** e **Comentar**

![configuração_ação.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21016967719058_set%20up%20action.jpg)   *Configurando o evento de ação do board de cópia*

### Criar ação do board

Esta ação criará um board com um título, descrição e configurações de acesso específicos.

- Título - insira um nome de título para o novo board. Se você deixar o campo em branco, o board será criado com o nome **Untitled**
- Descrição - insira o texto para a descrição do board
- Acesso à Team - você pode escolher entre os tipos de acesso **Privado**, **Visualizar**, **Comentar** e **Editar** para sua time
- Acesso via link - crie regras para compartilhar este board com um link. Você pode definir o acesso **Privado**, **Visualizar** ou **Comentar** por meio de um link público

![criar_ação_do_quadro.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21016967720338_create%20board%20action.jpg)
*Configurando o evento de ação Criar board*

### Criar ação de widget de cartão

Esta ação permite que você transfira informações (mensagens do Slack, por exemplo) como um widget [de cartão](../../using-miro/essential-tools/02-cards.md)diretamente dentro de um [quadro](../../using-miro/essential-tools/07-frames.md) específico em um board da Miro com regras personalizadas.

- board - escolha um board da time que você deseja usar. Você pode pesquisar o board pelo seu nome ou ID *(*por exemplo, *o9J_rxLXasqA)**.* Se você não encontrar um board na lista, tente recarregar os dados e verifique novamente
- quadro - selecione uma quadro do board que você escolheu. Você pode pesquisar o quadro pelo nome e, se não conseguir encontrá-lo, tente recarregar os dados e verifique novamente
- Título do cartão - insira um título para o seu cartão
- Link do título do cartão - aqui você pode inserir um link do aplicativo conectado (por exemplo, você pode criar um cartão com um link para uma tarefa recém-criada no Asana)
- Descrição do cartão - crie uma descrição para seu cartão
- Data de vencimento do cartão - defina uma data de vencimento para o cartão
- Cor da borda do cartão - escolha uma cor personalizada para as bordas do seu cartão (por exemplo, **#ff0000** neste campo definirá a cor do cartão como vermelho).

![criar_cartão_ação.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017005262610_create%20card%20action.jpg)
*Configurando o evento de ação Criar cartão*

## Desabilitar integração Zapier

Para remover a integração Zapier da sua time Miro , abra [Configurações da Team](../../administration/get-started-as-a-miro-admin/06-manage-starter-and-education-plan.md)**> Aplicativos e integrações > Zapier**e clique em **Desinstalar***.*

![desinstalar_Zapier.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017005263890_uninstall%20Zapier.jpg)
*Opções de desinstalação do Zapier*

## Perguntas frequentes

1. *Preciso ter uma conta empresarial Zapier para usá-lo com o Miro?*
   - Não, não é obrigatório. A integração do Miro pode ser criada com qualquer plano Zapier.
2. *Onde meus dados do Zapier são armazenados?*
   - Esta é uma integração oficial mantida Miro e todas as práticas de armazenamento de dados no Miro também se aplicam aqui.
3. *Preciso ser o admin do time no Miro para definir a integração com o Zapier?*
   - Depende das configurações de admin no Miro e no Zapier. Por padrão, até mesmo membros do time não administradores podem configurar a integração.
4. *Os cartões (Trello, Asana, etc.) sincronizam com os cartões importados para os boards da Miro?*
   - Não, o Zapier não fornece sincronização no momento. Por exemplo, se você mover seu cartão Trello de "fazendo" para "feito", isso não será refletido no lado do Miro.
5. *Não consigo vincular o Gmail ao Miro via Zapier. Por quê?*
   - Por favor, verifique seu e-mail. No momento, os usuários com conta do Gmail que termina *@gmail.com*ou*@googlemail.com* não podem vincular o Gmail ao Miro, pois o Zapier pode enviar informações do Gmail para um número limitado de aplicativos.
