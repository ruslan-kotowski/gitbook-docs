---
title: "Classifica\xE7\xE3o de dados"
article_id: 4417739162258
translation_id: 4417739162258
locale: pt-br
sidebar_position: 2
created_at: '2022-02-07T10:01:21Z'
updated_at: '2025-02-26T12:17:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

A classificação de dados permite que usuários do plano Enterprise atribuam rótulos aos seus boards para especificar o nível de sensibilidade do conteúdo do board .

> **Disponível para:** Plano Enterprise
> **Disponível em**: desktop, tablet
> **Quem pode fazer isso:** Admins da empresa

Você pode encontrar as configurações de classificação de dados no console de admin do Enterprise . Vá para **Configurações**e selecione **Classificação**.

:::note
Para clientes com Enterprise Guard, você pode encontrar **a Classificação** no console de admin em **Enterprise Guard**. Acesse **Configurações** > **Enterprise Guard** > **Classificação**.
:::

Certifique-se de entender os seguintes pontos-chave sobre classificação de dados:

- A classificação de dados é umaetiqueta internoe não tem impacto nas configurações de compartilhamento do board , o que significa que os boards podem ser compartilhados além de sua classificação.
- Os boards que foram criados antes do recurso ser habilitado serão marcados como não classificados.
- [Duplicar um board](../../../using-miro/managing-boards/03-how-to-duplicate-a-board.md) copiará o etiqueta de classificação de dados atual na nova cópia do board .
- Atualmente, os rótulos não são exibidos no [modo de apresentação](https://help.miro.com/hc/articles/360017731073), no [modo de reuniões inteligentes](https://help.miro.com/hc/articles/4408834812690)e em dispositivos móveis.

## Como configurar rótulos de classificação

Em **Configurações**, selecione **Classificação**. Para ativar rótulos de classificação para sua organização Enterprise , selecione **Configurar classificação.**

## Como adicionar novos rótulos de classificação

Os Admins da empresa podem criar e personalizar até 30 rótulos de classificação e definir um etiqueta padrão para todos os novos boards na organização.

Nas configurações **de Classificação** , quatro rótulos já foram criados, os quais você pode personalizar. Você também pode criar novos rótulos para atender às necessidades da sua organização.

Para criar uma nova classificação:

1. Selecione **Editar níveis de classificação**.
2. Clique em **Adicionar nível**.
3. Defina o **Nível**de classificação, adicione um **Nome**, adicione uma **Descrição**e altere a **cor do Emblema**.
4. Se você quiser adicionar uma referência para usuários do board , adicione um **Link para diretrizes**.
5. (Opcional) Selecione **Visualizar** para ver como sua etiqueta aparecerá na produção.
6. Selecione **Concluído**.
7. (Opcional) Para reordenar seus rótulos de classificação, clique nas setas para cima (**Ʌ**) ou para baixo (**V**).
8. Clique em **Publicar** para finalizar as alterações.

:::note
Quando você cria ou edita um etiqueta de classificação, suas alterações são salvas como rascunho e não são publicadas até que você clique no botão **Publicar** . Isso significa que você pode sair da configuração de classificação e retornar a ela a qualquer momento.
:::

Você também pode adicionar um link para as diretrizes de classificação da sua empresa, onde os colaboradores podem aprender mais sobre aspolíticas de classificação de dados existentes.

![](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921802487570_image.png)

*Link para diretrizes de classificação*

## Como personalizar rascunhos de classificação

Para editar uma classificação **sem** um rascunho salvo:

1. Clique no botão **Editar níveis de classificação** .
2. Clique no ícone de lápis **Editar** .
3. Faça suas alterações e clique em **Concluído**.
4. Clique em **Publicar** para finalizar as alterações.

Para editar uma classificação **com** um rascunho salvo:

1. No painel Classificação de dados, clique em **Retomar configuração**.
2. Clique no ícone de lápis **Editar** .
3. Faça suas alterações e clique em **Concluído**.
4. Clique em **Publicar** para finalizar as alterações.

## Como excluir um etiqueta de classificação

Para excluir um etiqueta, clique no ícone da lixeira. Observe que você não pode excluir o etiqueta padrão.

![data_classification_delete_label.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017013528978_data_classification_delete_label.png)
*Excluindo um etiqueta*

### Adicionando o etiqueta padrão no nível da empresa

Escolha um etiqueta de classificação padrão para os boards recém-criados. Cada novo board criado na organização Enterprise recebe o etiqueta padrão .

Para configurar um etiqueta padrão para sua organização, marque **etiqueta de classificação padrão** ao adicionar ou editar um etiqueta de classificação.

![Configurando etiqueta padrão de classificação de dados](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921802487570_image.png)

*Configurando o etiqueta de classificação padrão*

### Adicionando o etiqueta padrão no nível da Team

> **Configurado por:** Admins da empresa, admins do time

Os admins do time podem habilitar a **opção Substituir etiqueta padrão** e definir um etiqueta padrão no nível da time : cada novo board criado na time receberá esse novo etiqueta padrão, substituindo o etiqueta padrão definido no nível da empresa.

Para habilitar essa configuração, navegue até Configurações da Team > **Permissões** e role para baixo.

Observe que você pode definir o etiqueta de substituição da time somente se a configuração de classificação de dados estiver habilitada no nível da empresa.

Para [times recém-criadas,](../../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md) essa configuração será desabilitada se você escolher as configurações padrão ao criar um time.

### Adicionar rótulos de classificação aos boards

> **Configurado por:** [titulares do board](../../../using-miro/sharing-boards/01-board-access-rights.md), [cotitulares do board](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md), editores que são membros da time, Admins da empresa com [permissões de admins de conteúdo](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md)

Se a classificação de dados estiver habilitada nas configurações da sua empresa, os usuários poderão ver e alterar os rótulos dos board . O etiqueta de classificação de dados aparece como um emblema ao lado do nome do board . Ao passar o mouse sobre o emblema, os colaboradores podem ver uma dica de ferramenta com o nome e a descrição do etiqueta .

O titular do board , [os cotitulares do board](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md), os editores que são membros da time e os Admins da empresa com [permissões de admins de conteúdo](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) podem atualizar o etiqueta de classificação clicando no emblema de classificação ou nos detalhes do board . Selecione um etiqueta e clique em **Atualizar**. Se o Admin da empresa adicionou um link para diretrizes nas configurações, o usuário pode seguir o link no pop-up para obter mais detalhes.

![data_classification_adding_labels_to_boards.gif](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017043043090_data_classification_adding_labels_to_boards.gif)
*Alterando o etiqueta de classificação de dados no board*

### Filtro de classificação de dados no painel

Usuários no plano Enterprise com classificação de dados habilitada podem filtrar seus boards por rótulos no painel. **Qualquer classificação** é selecionada por padrão.

![data_classification_classification_filter.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017043043986_data_classification_classification_filter.png)
*Filtro de classificação de board no painel*
