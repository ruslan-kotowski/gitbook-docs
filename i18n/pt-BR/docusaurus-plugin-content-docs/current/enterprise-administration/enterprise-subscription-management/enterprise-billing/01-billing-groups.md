---
title: "Grupos de cobran\xE7a"
article_id: 6574185673874
translation_id: 6574185673874
locale: pt-br
sidebar_position: 1
created_at: '2022-07-12T12:53:45Z'
updated_at: '2026-02-19T10:50:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: billing-groups
---

Os grupos de cobrança permitem aos Admins da empresa mapear usuários para orçamentos internos. Como cada usuário pode ser atribuído a apenas um grupo, os admins podem facilmente rastrear o número de licenças usadas por cada centro de custo. Admins também podem definir uma cota flexível de licenças disponíveis para cada grupo de cobrança. Isso simplifica processos como ajuste de licenças, renovações e cobranças por equipes.

> **Disponível para:** Plano Enterprise
> **Quem pode fazer:** Admins da empresa

## Configurações de grupo de cobrança

As suas configurações de grupos de cobrança mostram uma visão abrangente do uso de licenças. Por exemplo, os detalhes de todos os grupos de cobrança existentes, incluindo a contagem de usuários, o número de cada tipo de licença e, se atribuído, a [cota flexível](02-billing-groups-soft-quotas.md) de licenças alocadas por grupo. Use o campo de pesquisa para encontrar rapidamente um grupo de cobrança específico.

### Onde encontrar seus grupos de cobrança

Para encontrar suas configurações de grupos de cobrança, vá para **Configurações** **da empresa** > **Assinatura** > **Grupos de cobrança.**

:::note
Usuários não atribuídos a um grupo de cobrança são automaticamente colocados no grupo de cobrança padrão da empresa. Você pode ver o número de usuários ativos atribuídos no banner no topo de suas configurações de grupos de cobrança.
:::

## Como criar um grupo de cobrança

1. Vá para **Configurações** **da empresa** > **Assinatura** > **Grupos de cobrança**.
2. Clique em **Criar um grupo de cobrança**.
3. Adicione o nome do grupo de cobrança.
4. (Opcional) Para definir uma cota flexível nas licenças atribuídas a este grupo de cobrança, selecione Adicionar cota para licenças Standard ou Adicionar cota para licenças Advanced e insira um número.
   Para saber mais sobre cotas flexíveis, consulte as perguntas frequentes no final deste artigo.
5. Para adicionar novos usuários ao grupo de cobrança, você pode carregar um arquivo CSV com a lista de endereços de e-mail dos usuários ou atribuir usuários posteriormente.
6. (Opcional) Atribua um contato para o grupo de cobrança. O contato pode ser consultado para informações sobre o uso de licenças.
7. Clique **Criar grupo de cobrança**.

## Como editar um grupo de cobrança

Você pode editar o nome do grupo de cobrança, definir ou atualizar uma cota flexível, alterar o contato do grupo de cobrança e adicionar usuários ao grupo de cobrança.

:::note
Adicionar usuários a um novo grupo de cobrança os transfere automaticamente do grupo anterior.
:::

1. Vá para **Configurações da empresa** > **Assinatura** > **Grupos de cobrança**.
2. Clique nos três pontos ao lado de um grupo de cobrança e escolha **Editar**.
3. Edite qualquer uma das propriedades do grupo de cobrança. Para adicionar usuários ao grupo de cobrança, carregue um arquivo CSV com a lista de endereços de e-mail dos usuários, ou atribua usuários mais tarde.
4. Clique em **Salvar**.

## Como excluir um grupo de cobrança

1. Vá para **Configurações da empresa** > **Assinatura** > **Grupos de cobrança**.
2. Clique nos três pontos ao lado de um grupo de cobrança e escolha **Excluir**.
3. Confirme a exclusão.
4. Todos os usuários que estavam neste grupo de cobrança serão atribuídos de volta à conta principal e não farão mais parte de nenhum grupo de cobrança.

## Como atribuir um usuário a um grupo de cobrança

Um usuário pode ser membro de apenas um grupo de cobrança dentro da organização.

1. Vá para as configurações da **Empresa** > **Usuários ativos**.
2. Clique nos três pontos ao lado de um usuário.
3. Escolha **Alterar grupo de cobrança**.
4. Selecione um grupo de cobrança e clique em **Atribuir usuário**. O usuário será adicionado ao novo grupo de cobrança.

## Como atribuir usuários em massa a um grupo de cobrança

Atribua múltiplos usuários a um grupo de cobrança de uma vez.

1. Acesse as configurações da **Empresa** > **Usuários ativos**.
2. Selecione usuários manualmente ou aplique filtros e selecione até 50 usuários de uma só vez.
3. Clique em **Ações em massa** e selecione **Atribuir grupo de cobrança**.
4. Escolha um grupo e clique em **Atribuir usuários**. Se alguns usuários já forem membros de outros grupos de cobrança, será possível desmarcá-los ou alterar a atribuição de grupo de cobrança.

## Como verificar quais usuários estão em um grupo de cobrança

Verifique quem está em um grupo de cobrança para gerenciar de forma mais eficaz o acesso dos usuários e a cobrança.

1. Acesse as configurações da **Empresa** > **Assinatura** > **Grupos de cobrança**.
2. Clique em um grupo de cobrança específico para ver os usuários atribuídos a ele.

## Como remover um usuário de um grupo de cobrança

Se um usuário não estiver atribuído a um grupo de cobrança específico ou for removido de um, ele será automaticamente designado ao grupo de cobrança padrão da conta da empresa.

1. Vá para as configurações da **Empresa** > **Usuários ativos**.
2. Clique nos três pontos ao lado de um usuário.
3. Escolha **Alterar grupo de cobrança**.
4. Selecione **Grupo de cobrança padrão da conta**. O usuário será removido do grupo de cobrança e passará a fazer parte do grupo de cobrança geral da empresa.

## Como atribuir usuários a um grupo de cobrança via arquivo CSV

Atribua vários usuários a um grupo de cobrança carregando um arquivo CSV com os e-mails dos usuários. Se um usuário já fizer parte de outro grupo de cobrança, ele será movido para o novo grupo designado.

:::note
Certifique-se de que seu arquivo CSV tenha apenas uma coluna com o cabeçalho ‘e-mail’. Esta coluna deve incluir sua lista de e-mails a serem adicionados ao grupo de cobrança. Verifique se seu CSV usa vírgulas para separar os valores. Informações em colunas adicionais não serão processadas. A Miro não salva os arquivos CSV.
:::

1. Vá para as configurações da **empresa** > **Assinatura** > **Grupos de cobrança**.
2. Clique nos três pontos ao lado de um grupo de cobrança e escolha **Editar**.
3. Carregue um arquivo CSV com a lista de endereços de e-mail dos usuários.
4. Clique em **Salvar**.

## Como atribuir usuários a um grupo de cobrança via SCIM

Configure o [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) para alocar automaticamente os usuários a um grupo de cobrança de acordo com um centro de custo.

#### Passo 1: Configure seu provedor de identidade (IdP)

Garanta que seu provedor de identidade (IdP) esteja configurado para adicionar o centro de custo à Miro. Veja os guias para:

- [Configurar provisionamento automatizado com o OKTA](../../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md)
- [Configurar provisionamento automatizado com o Azure AD](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)

#### Passo 2: Atribua centros de custo ao seu grupo de cobrança

Adicione um ou mais centros de custo a um grupo de cobrança. Todos os usuários atuais e futuros desses centros de custo entrarão automaticamente no grupo de cobrança.

**Como adicionar um centro de custo**

1. Abra a página **Editar grupo de cobrança**.
2. Insira seu centro de custo no campo **Inserir centro de custo**.
3. Pressione **Enter** no teclado.
4. Adicione quantos centros de custo adicionais forem necessários.
5. Clique em **Salvar**.

:::note
*A Miro não verifica as informações do centro de custo inseridas. Certifique-se de inserir informações precisas para os nomes dos centros de custo. Este campo não diferencia maiúsculas de minúsculas.*
:::

### Gerenciado por selo SCIM

Usuários com um centro de custo atribuído vinculado a um grupo de cobrança são rotulados como **Gerenciado por SCIM**. Você verá este selo ao lado do nome do usuário.

Esses usuários não podem ser adicionados manualmente aos grupos de cobrança e podem ser designados a um centro de custo apenas por meio de uma atualização SCIM.

### Diretrizes para centro de custo e grupo de cobrança

- Um grupo de cobrança pode conter vários centros de custo, mas um único centro de custo pode estar vinculado a apenas um grupo de cobrança.
- Para reatribuir um centro de custo, primeiro você precisa remover o centro de custo de seu grupo de cobrança atual.
- Usuários que são atribuídos a um grupo de cobrança com base em seu centro de custo não podem ser atribuídos manualmente a outro grupo de cobrança.
- Remover um centro de custo de seu grupo de cobrança também removerá todos os usuários provisionados por SCIM desse grupo de cobrança.
- Usuários não provisionados por SCIM podem ser atribuídos manualmente a qualquer grupo de cobrança.

### Como remover um centro de custo de um grupo de cobrança

1. Abra a página de **Editar grupo de cobrança**.
2. Clique no **X** ao lado do centro de custo que você deseja remover.
3. Clique em **Salvar**.

## Como exportar dados do grupo de cobrança

Os admins da empresa podem exportar um arquivo CSV com a lista de usuários em **Configurações da empresa** > **Usuários ativos**. Você pode então usar o atributo dos grupos de cobrança na planilha CSV exportada para filtrar orçamentos.

## Perguntas frequentes

O que acontece quando meus usuários mudam de centros de custo no lado do provedor de identidade?

Após uma atualização SCIM:

- se este novo centro de custo for atribuído a um grupo de cobrança, o usuário será automaticamente movido para este novo grupo de cobrança.
- se este novo centro de custo não for atribuído a um grupo de cobrança ou o centro de custo foi removido do usuário no provedor de identidade, o usuário será automaticamente movido para o grupo de cobrança padrão da empresa.

O que acontece com os usuários que foram atribuídos manualmente a um grupo de cobrança após a implementação do SCIM para grupos de cobrança?

Eles são automaticamente atribuídos a um novo grupo de cobrança de acordo com seu centro de custo, enquanto aqueles sem um centro de custo correspondente ou sem qualquer centro de custo permanecem em seu grupo de cobrança atual.

Por que não consigo mais atribuir manualmente um usuário aos grupos de cobrança?

Usuários atribuídos a um grupo de cobrança via seu centro de custo SCIM não podem ser movidos manualmente para outro grupo.

O que acontece se o meu IdP parar de sincronizar o atributo de centro de custo com a Miro?

Novos usuários não serão atribuídos automaticamente a um grupo de cobrança sem centros de custo sincronizados, mas podem ser atribuídos manualmente até que a sincronização seja retomada.

O que é uma cota flexível para grupo de cobrança?

Uma cota flexível permite que você defina opcionalmente um limite nas licenças Avançadas, Padrão ou Completas (legado) disponíveis para um grupo de cobrança.

Ao criar ou editar um grupo de cobrança, você pode ativar **Adicionar cota para licenças Padrão** ou **Adicionar cota para licenças Avançadas** e inserir um número.

A cota flexível aparece, como o número que você definiu e uma barra de progresso que indica o consumo, na parte superior da visão geral do grupo de cobrança.

Para saber mais sobre cotas flexíveis, veja [Cotas flexíveis para grupos de cobrança](02-billing-groups-soft-quotas.md).
