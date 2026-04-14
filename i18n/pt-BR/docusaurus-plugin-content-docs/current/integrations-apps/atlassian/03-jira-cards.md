---
title: Cartões do Jira
article_id: 360017572434
translation_id: 13809093055634
locale: pt-br
sidebar_position: 5
created_at: '2023-09-18T15:23:58Z'
updated_at: '2025-11-25T15:59:45Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Planos: Starter, Business, Education, Enterprise Pessoas: Todos os usuários
    Plataformas: Navegador, Desktop, Mobile Jira: Jira Cloud, Jira Server (on-premise),
    Jira Data Center'
---

Os cartões do Jira permitem que você trabalhe com itens do Jira diretamente nos boards da Miro. Essa integração otimiza o fluxo de trabalho de sua equipe ao trazer itens do Jira para o seu espaço de trabalho colaborativo para retrospectivas, planejamento de histórias, priorização de backlog, mapeamento de histórias e outras atividades em equipe.

![Jira cards in user story mapping](../../../../../../docs/integrations-apps/atlassian/images/21017348097170_Jira%20cards%20in%20USM.png)

## Importar itens do Jira para o seu board

Você pode importar itens do Jira para o seu board de duas maneiras:

1. Copie o URL do item do Jira e cole-o no board.
2. Clique no ícone **Ferramentas, Mídia e Integrações** (**+**) na barra de criação, selecione **Cartões do Jira**, escolha um ou mais itens e clique em **Adicionar**.

Ao importar itens pela primeira vez, será necessário conectar sua conta do Jira:

1. Clique em **Autorizar** na caixa de diálogo que aparecer.
2. Faça login na sua conta do Jira com suas credenciais.
3. Autorize a conexão entre Miro e Jira.

Após a autorização, você verá todos os itens do Jira aos quais tem acesso no seletor de Cartões do Jira.

:::note
Usuários que não autorizaram suas contas do Jira verão uma visualização simplificada do cartão sem avatares de destinatários.
:::

## Criar novos itens do Jira

Você pode criar itens do Jira diretamente da Miro de duas maneiras.

### Criar usando o aplicativo do Jira

1. Clique no ícone **Ferramentas, Mídia e Integrações** (**+**) na barra de ferramentas de criação
2. Selecione **Cartões do Jira**.
3. Clique em **Criar item**.
4. Preencha os campos obrigatórios.
5. Clique em **Criar**.

### Converter itens existentes em itens do Jira

Você pode converter notas adesivas ou cartões existentes no seu board em itens do Jira.

1. Selecione até 50 notas adesivas ou cartões.
2. Clique em **Converter para** > **Jira** no menu de contexto.
3. Defina os valores padrão (tipo de item, prioridade, responsável, etc.).
4. Clique em **Converter**.

:::warning
Nota:

- Cartões na linha de Tarefas USM não podem ser convertidos em itens do Jira.
- Durante a conversão, as tags e a data de início dos cartões Miro não serão preservadas.
- As informações do responsável precisam ser definidas novamente após a conversão.
:::

## Visualizar e editar itens do Jira

:::warning
A edição de cartões do Jira não é suportada no aplicativo para desktop ou móvel.
:::

Você pode visualizar cartões do Jira de duas maneiras:

- Visualização lateral
- Visualização centralizada

### Editar itens no Miro

1. Clique no ícone **Abrir no painel lateral** ou **Abrir no painel central**.
2. Faça suas alterações.
3. Clique em **Atualizar** para salvar.

### Alterar status do item

1. Clique no ícone **Fluxo de Trabalho**.
2. Selecione o **Status** desejado e **Comentário**.
3. Clique em **Atualizar** para salvar.

### Editar no Jira

1. Selecione um cartão e clique no ícone **Fonte**.
2. Edite o item no Jira na nova guia do navegador.
3. As alterações serão sincronizadas automaticamente com o cartão Miro.

## Sincronização entre Miro e Jira

|  |  |
| --- | --- |
| **Atualização de instância do Jira vs atualização do cartão da Miro** | **Quando ocorre a atualização?** |
| Atualização no Jira via OAuth 1.0 e OAuth 2.0 | O cartão do Jira na Miro é atualizado imediatamente via [Webhook](https://help.miro.com/hc/articles/360017731113). |
| Atualização na Miro | O cartão do Jira é atualizado imediatamente e o item correspondente do Jira é atualizado simultaneamente. |

## Personalizar cartões do Jira

### Alterar cores dos cartões

1. Selecione um ou mais cartões do Jira.
2. Clique em **cor de preenchimento** no menu de contexto.
3. Escolha a cor desejada.

### Configurar campos personalizados

1. Clique no ícone **Ferramentas, Mídia e Integrações** (**+**) na barra de ferramentas de Criação
2. Selecione **Cartões Jira**.
3. Selecione **Configurar cartões**.
4. Selecione os campos que deseja exibir.
5. Clique em **Salvar**.

:::note
Notas importantes sobre campos:

- As configurações se aplicam apenas ao board atual.
- Campos padrão (Responsável, Tipo de item, Prioridade, Status) não podem ser removidos.
- Campos podem não aparecer se não tiverem valor ou não estiverem disponíveis para o tipo de item.
- Alguns tipos de campos (como campos personalizados de cores) não são suportados.
:::

## Pesquisar itens do Jira

O seletor de cartões do Jira mostra as tarefas recentes primeiro e oferece várias opções de classificação:

- Tipo de item
- Prioridade
- Chave
- Resumo
- Responsável
- Status

Use palavras-chave para encontrar itens específicos ou use **Jira Query Language** (JQL) para buscas complexas:

1. Selecione a opção **Pesquisa avançada** na barra de busca.
2. Digite sua consulta JQL.

Os resultados serão atualizados com base na sua consulta.

## Artigos relacionados

- [Perguntas frequentes sobre cartões do Jira](https://help.miro.com/hc/articles/360013463739)
- [Configurar e desinstalar cartões do Jira](https://help.miro.com/hc/articles/360019501754)
- [Configurar webhooks para cartões do Jira](https://help.miro.com/hc/articles/360017731113)
- [Solucionar problemas com cartões do Jira](https://help.miro.com/hc/articles/360017572654)
