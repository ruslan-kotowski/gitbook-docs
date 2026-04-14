---
title: Incorporar um board da Miro
article_id: 360016335640
translation_id: 360016335640
locale: pt-br
sidebar_position: 2
created_at: '2020-09-09T07:54:13Z'
updated_at: '2025-09-19T09:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Pessoas: Editores do board Planos: Todos os planos Plataformas: Web, Desktop,
    Mobile'
---

Você pode incorporar qualquer board da Miro ou um item específico (quadro ou formato) do board em aplicativos e sites compatíveis, permitindo que seus colegas de time trabalhem em contexto sem trocar de ferramentas.

Os embeds herdam as [configurações de compartilhamento](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) do board:

- **Link público ativado** — qualquer pessoa com o link pode visualizar (ou, em Planos pagos e Education, comentar ou editar).
- **Link público desativado** — apenas colaboradores convidados podem abrir o embed após fazer login.

Os [admins Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md) podem gerenciar a disponibilidade do link público nas [configurações de segurança](../../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Escolha o seu método de incorporação

A Miro oferece duas maneiras de inserir boards:

- **Usando aplicativos suportados**:

  - Trabalhar em plataformas como Zoom, Teams, Confluence, Jira ou Notion.
  - Você deseja funcionalidades de integração nativas e fluxo de trabalho contínuo.
  - Usuários interagirão principalmente através dessa plataforma específica.
  - Você precisa do processo de configuração mais simples.
- **Usando código de incorporação**:

  - Incorporar em sites, blogs ou plataformas personalizadas.
  - Trabalhar com WordPress, Webflow ou outros criadores de sites.
  - Você precisa de mais controle sobre tamanhos e aparência.
  - A plataforma suporta iFrames, mas não tem uma integração nativa com Miro.

## Inserir um board em aplicativos suportados

A Miro é compatível com vários aplicativos, onde você pode compartilhar facilmente os seus boards da Miro. Os aplicativos suportados incluem:

- [Zoom](../../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md)
- [Webex](../../../integrations-apps/more-integrations/10-miro-for-webex.md)
- [Microsoft Teams](../../../integrations-apps/microsoft/microsoft-teams/02-miro-for-microsoft-teams-user-guide.md)
- [Jira](../../../integrations-apps/atlassian/02-miro-for-jira-cloud.md)
- [Confluence](../../../integrations-apps/atlassian/01-miro-for-confluence.md)
- [Notion](https://miro.com/marketplace/notion-embed/)
- [Coda](https://miro.com/marketplace/coda-embed/)
- [Productboard](https://miro.com/marketplace/productboard-embed/)
- Média

Quando você insere um board da Miro em outro aplicativo, pode definir os direitos de acesso específicos para os usuários do aplicativo e permitir que eles visualizem, comentem ou editem o board a partir desse aplicativo. O acesso ao board pelo site da Miro não será afetado. Saiba como [o compartilhamento e as permissões funcionam para boards incorporados](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

Para inserir um board em um dos aplicativos compatíveis:

1. No aplicativo de destino, digite **/miro** ou escolha **Miro** no menu de inserção.
2. Selecione o board.
3. Selecione a **Visualização inicial**:
   - **Board completo** — todo o canvas.
   - **Item específico**, como quadro ou formato (Doc, Diagrama, Tabela, Linha do tempo ou Slides).
4. Ative o **modo foco** para criar uma inserção sem distrações. Deixe desativado para permitir interação completa.
5. Selecione as **configurações de acesso** para todos os visitantes:
   - **Pode visualizar** — qualquer pessoa que visualizar a inserção pode ver o board.
   - **Requer acesso** — qualquer pessoa que visualizar a inserção deve ter acesso para visualizar, comentar ou editar o board.
6. Selecione **Inserir board**.

A inserção respeita as configurações de compartilhamento do board. Em dispositivos móveis, todas as inserções são somente para visualização.

## Incorporar um board com código de incorporação

Use esta opção para qualquer plataforma que suporte iFrame, como **WordPress** ou **Webflow**.

1. Abra o painel de **compartilhamento** usando um destes métodos:
   - No canto superior direito, selecione **Compartilhar** > **Inserir**, ou
   - No menu principal do board, selecione **Board** > **Exportar** > **Inserir**, ou
   - No canvas, selecione o item que você deseja inserir (quadro ou formato). Por exemplo, um Documento. Abra o menu de contexto de três pontos e selecione **Inserir este documento**.
2. Selecione a **Visualização inicial**:
   - **Board** — toda a canvas.
   - **Item específico**, como quadro ou formato (Documento, Diagrama, Tabela, Linha do tempo ou Slides).
3. (Opcional) **Definir área inicial** — arraste para delimitar uma região exata do board.
4. Decida sobre a interação:
   - Selecionar **Apenas visualizar** para bloquear a visualização.
   - Desmarcar **Apenas visualizar** para permitir que os visualizadores desloquem, ampliem, comentem ou editem (se tiverem permissão).
5. Selecionar **Copiar código** e colar onde precisar.
   Se o destino aceitar apenas URLs, selecione **Copiar link** em vez disso.

Você pode criar várias incorporações para o mesmo board, cada uma com sua própria visualização inicial, área inicial ou objeto de foco.

### Reproduzir slides automaticamente

Para reproduzir automaticamente uma incorporação de Slides, defina o **Intervalo automático de slides** de 1 a 30 segundos na guia **Incorporar**. A reprodução automática é ignorada quando você insere um board dentro de outro board.

## Como as incorporações aparecem

- O nome do board não é clicável.
- O mini-mapa, as [notas](../../essential-tools/17-visual-notes.md) e os pop-ups estão fechados por padrão.
- Algumas opções de menu, como **Definir visualizar inicial**, estão ocultas.
- Todos os embeds são apenas para visualização em dispositivos móveis.
- Bloqueadores de cookies de terceiros podem impedir que os embeds sejam carregados corretamente.

## Perguntas frequentes

**Qual é a diferença entre uma visualizar inicial e o modo foco?**
 Uma visualizar inicial define a posição inicial, mas os visualizadores ainda podem explorar o board. O modo foco oculta tudo, exceto o objeto selecionado, e é sempre apenas para visualização.

**Posso fazer um embed em modo foco ser editável?**
 Não. Para habilitar a colaboração, desmarque **Apenas para ver** e conceda direitos de edição nas configurações de compartilhamento do board.

**Quais widgets são suportados?**
 Documentos, Diagramas, Tabelas, Linhas do tempo, Slides e qualquer quadro.

**Posso remover o logotipo da Miro?**
 Não. A remoção da marca não está disponível.

**Posso incorporar um board dentro de outro board?**
 Sim. Copie o código de inserção e cole-o no board de destino com **Colar código iFrame**.
