---
title: "Criar etiquetas e palavras-chave para informa\xE7\xF5es sens\xEDveis da empresa"
article_id: 21626517022610
translation_id: 21626517022610
locale: pt-br
sidebar_position: 11
created_at: '2024-09-26T21:36:45Z'
updated_at: '2026-03-04T22:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Crie etiquetas para definir condições, como palavras-chave ou widgets, que você deseja identificar e localizar nos boards da Miro. Você pode criar até 100 etiquetas personalizadas sensíveis da empresa. Para criar uma etiqueta, siga as seguintes etapas:

:::note
Para criar etiquetas personalizadas, você deve ter a [função de admin de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, fale com seu Admin da empresa.
:::

1. Vá para suas [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Descoberta de dados**.
3. Na página **Descoberta de dados**, clique na aba **Configuração**.
4. Na seção **Sensíveis da empresa personalizados**, clique no botão **Criar**.
5. Na página **Definir etiqueta personalizada**, adicione os detalhes da etiqueta.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | **Nome da etiqueta** | **Comprimento máximo:** 80 caracteres  Nome descritivo da etiqueta personalizada. Você pode usar o nome de um projeto interno da empresa, já que esta etiqueta não aparece nos logs.  **Nota:** O nome da etiqueta não fica visível nos logs de auditoria. Se você quiser pesquisar ou visualizar os logs de auditoria associados a esta etiqueta, pode usar o ID da etiqueta. |
   | **Nome abreviado** | **Tamanho máximo:** 10 caracteres, alfanumérico  Versão abreviada do nome da etiqueta. O nome abreviado é usado para se referir a esta etiqueta personalizada na descoberta de dados, no buscador de conteúdo e na classificação de dados. **Nota:** O nome abreviado não fica visível nos logs de auditoria. Se você quiser pesquisar ou visualizar os logs de auditoria associados a esta etiqueta, pode usar o ID da etiqueta. |
   | **Descrição** | **Tamanho máximo:** 500 caracteres  Descrição das informações detectadas por esta etiqueta. Essas informações são úteis para outros admins. |
   | **Condições** | Insira as palavras-chave e os tipos de widget que você deseja detectar e aplique esta etiqueta ao detectá-los em um board da Miro. Você deve adicionar pelo menos uma condição.  Se você adicionar apenas as palavras-chave e não marcar nenhuma caixa de seleção de widget, a descoberta de dados detectará todos os boards que contenham as correspondências exatas das palavras-chave fornecidas para todos os widgets compatíveis. A versão atual faz detecção de palavras-chave nos seguintes itens do board: nota adesiva, cartão, cartão do Jira, bloco de código, comentários, quadro, tabela, conector/linha, forma, bloco de texto, board Kanban e mapa da história do usuário.  Você também pode optar por detectar somente blocos de código, cartões do Jira, cartões do Azure ou telas de prototipagem, sem adicionar palavras-chave. A descoberta de dados detecta todos os boards que contêm esses widgets.  Se você adicionar as palavras-chave e os widgets como condições, esses dois critérios devem ser atendidos para que a descoberta de dados detecte o board. Isso possibilita que você refine sua pesquisa e identifique os boards com mais precisão usando as etiquetas personalizadas.  **Exemplos:**  - Digamos que queira restringir a detecção do board para detectar especificamente os boards relacionados ao desenvolvimento de produtos, sem incluir os de marketing, e que devem conter o nome do projeto *Enterprise* *Guard*, como também queira encontrar apenas os boards que contenham um cartão do Jira (por estarem relacionados ao desenvolvimento de produtos). Ao configurar esta etiqueta, inclua a palavra-chave *Enterprise* *Guard* e marque a caixa de seleção do cartão do Jira. Assim, a descoberta de dados localiza os boards que contenham a palavra-chave Enterprise Guard e um cartão do Jira. Além disso, a descoberta de dados detecta os boards que contêm cartões do Jira com a palavra-chave Enterprise Guard em seu título ou descrição. Se um board contiver apenas a palavra-chave *Enterprise* *Guard*, mas não incluir um cartão do Jira, ele não será detectado, pois não atende a ambas as condições especificadas.  - Se quiser detectar todos os boards que contenham a palavra *Enterprise* *Guard* em todos os tipos de widget compatíveis, independentemente dos widgets que o board contenha, na seção **Adicionar palavras-chave**, adicione a palavra-chave **Enterprise** **Guard**. Você não precisa adicionar nenhum tipo de widget neste caso.  - Se você quiser detectar todos os boards com cartões do Jira, independentemente de qualquer conteúdo específico, na seção **Adicionar tipo de widget**, marque a caixa de seleção do **cartão do Jira**. Você não precisa adicionar nenhuma palavra-chave neste caso.    **Para adicionar uma palavra-chave:**  1. Clique em **Adicionar palavras-chave**.  2. Insira ou cole as palavras-chave separadas por vírgulas. **Notas:**  - As palavras-chave podem ter caracteres alfanuméricos e Unicode. - Você pode adicionar até 100 palavras-chave ou frases. - Todos os espaços antes e depois das palavras-chave não são considerados. - A descoberta de dados detecta correspondências exatas das palavras-chave fornecidas, sem diferenciar entre letras maiúsculas e minúsculas. - Se você adicionar um espaço antes de uma palavra-chave, a descoberta de dados encontrará correspondências exatas que também tenham um espaço antes da palavra-chave. - A versão atual faz detecção de palavras-chave nos seguintes itens do board: nota adesiva, cartão, cartão do Jira, bloco de código, quadro, tabela, conector/linha, forma, bloco de texto, board Kanban e mapa da história do usuário. No momento, as notas e os comentários não estão incluídos nas verificações de descoberta de dados. Estamos trabalhando para incluir as notas e os comentários nos próximos lançamentos de melhorias de funcionalidades.  **Exemplo:** Para identificar e rotular os boards que contêm as palavras-chave *confidencial* ou *interno*, adicione as seguintes palavras-chave: *confidencial, interno* (use uma vírgula para separar cada palavra-chave). A descoberta de dados localiza todos os boards que incluam qualquer uma dessas palavras-chave.  **Para adicionar um tipo de widget:**  1. Clique em **Adicionar tipo de widget**.  2. Marque a caixa de seleção do tipo de widget que deseja detectar nos boards da Miro.  **Exemplo:** Se você quiser detectar e rotular os boards que contenham um cartão do Jira, marque a caixa de seleção do **cartão do Jira**. |
6. Clique em **Próximo**.
7. Revise os detalhes da etiqueta personalizada.

   Se você quiser editar os detalhes da etiqueta personalizada, clique no botão **Anterior**.

   Se os detalhes da etiqueta personalizada estiverem corretos, clique no botão **Criar etiqueta personalizada**.

   Depois de criar a etiqueta, a primeira verificação começa automaticamente. Os resultados que apresentem as condições selecionadas ficarão disponíveis após alguns minutos ou horas, dependendo da quantidade de boards da sua organização na Miro.
