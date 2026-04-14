---
title: "Editar pol\xEDtica de disposi\xE7\xE3o"
article_id: 19551033354002
translation_id: 19551033354002
locale: pt-br
sidebar_position: 18
created_at: '2024-06-14T19:50:51Z'
updated_at: '2025-12-08T16:14:46Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Para editar políticas de disposição, você deve ter a [função de Admin de governança de dados](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de governança de dados, fale com seu Admin da empresa.
:::

Para editar uma política de disposição, realize as seguintes etapas:

1. Vá para as suas [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Ciclo de vida do conteúdo**.
3. Clique na guia **Disposição**.
   A **página de políticas de disposição** será exibida.
4. Na **página de políticas de disposição**, clique na política de disposição que deseja editar.
   A página com as informações relacionadas à política será aberta.
5. Clique em **Editar** no canto superior direito da página e edite os campos necessários. A tabela a seguir lista cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | **Nome**  **(obrigatório)** | Nome da política de disposição.  Tamanho máximo: 60 caracteres. |
   | **Descrição**  **(opcional)** | Descrição da política de disposição.  Tamanho máximo: 300 caracteres. |
   | **Período de disposição**  **(obrigatório)** | Especifique quando boards são movidos automaticamente para a lixeira. Escolha um número, selecione **Meses** ou **Anos**, e depois escolha se o período é calculado a partir da **última modificação** do board ou da **última visualização**.  Se quiser especificar o período da disposição em meses, você deve selecionar um período de disposição entre 1 e 120 meses.  Se quiser especificar o período da disposição em anos, você deve selecionar um período de disposição entre 1 e 10 anos.  Por exemplo, se desejar que os boards sejam movidos para a lixeira quando não tenham sido modificados por um ano, você pode selecionar 1 ano e escolher **Última modificação**. |
   | **Escopo**  **(obrigatório)** | Selecione o escopo para esta política de disposição. O escopo indica a quais boards esta política de disposição será aplicada. Você pode definir o escopo de uma política de disposição para todos os boards de uma organização ou para níveis específicos de classificação do board.  **Defina a política de disposição para todos os boards da organização** Se quiser definir o escopo da política de disposição para todos os boards da organização, na lista **Escopo**, selecione **Todos os boards da organização**.  **Defina a política de disposição para um ou mais times na organização** Se você deseja definir o escopo da política de disposição para um ou mais times na organização, execute as seguintes etapas:  1. Na lista de **Escopo**, selecione **Time**. 2. Clique na caixa **Introduzir time** e selecione cada time ao qual você deseja aplicar a política de disposição. Uma marca de seleção aparecerá ao lado do time que você escolheu associar à política de disposição.   ✏️ - Você pode selecionar múltiplos times para uma política de disposição. No entanto, qualquer time pode ser associado a apenas uma política de disposição por vez.  - Você pode selecionar qualquer time, incluindo times deletados, como escopo ao definir a política de disposição.   - Um time que é selecionado como escopo para uma política de disposição não pode ser permanentemente deletado até que o time seja removido do escopo.  **Definir a política de disposição para um nível de classificação do board**  ✏️ Para definir o escopo da política de disposição para um nível específico de classificação do board, você deve garantir que a funcionalidade Classificação de dados está ativada. Quando uma política de disposição usa um nível de classificação do board, não é possível desativar a funcionalidade Classificação de dados. Para mais informações, consulte a documentação sobre [Classificação de dados](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Se quiser definir o escopo da política de disposição para um nível específico de classificação do board, siga as seguintes etapas:  1. Na lista de **Escopo**, selecione **Classificação**. 2. Clique na lista ao lado da lista de **Classificação** e selecione os níveis de classificação aos quais deseja aplicar a política de disposição. Você também pode pesquisar os níveis de classificação e, em seguida, selecioná-los.  Uma marca de seleção aparece ao lado dos níveis de classificação selecionados para associá-los à política de disposição.  ✏️ **Notas:** - Você pode selecionar múltiplos níveis de classificação ao mesmo tempo. - Não é possível definir o mesmo nível de classificação para políticas de disposição diferentes. Se um nível de classificação específico já estiver associado a uma política de disposição, esse nível será mostrado como indisponível.  - Quando uma política de disposição usa um nível de classificação do board, não é possível desabilitar a funcionalidade Classificação de dados.  -Depois que um nível de classificação é associado a uma política de disposição, não é possível excluir esse nível de classificação específico. - Quando um board está sujeito às políticas de disposição com ambos os escopos de todos os boards da organização e de classificação, aplica-se a política com o período de disposição mais longo. |
6. Clique em **Próximo**.
   A página de **Revisão de impacto** aparece.
7. Revise o impacto da política de disposição. A página de revisão do impacto traz as seguintes informações:
   - **Resumo:** configuração da política de disposição, como o nome da política, o período de disposição e o escopo.
   - **Impacto da política:** número de boards que serão regidos por esta política.
8. Para salvar a configuração e aplicar a política de disposição, clique em **Publicar**.
   Se você não tiver as notificações de disposição ativadas, a caixa de diálogo **Ativar notificação de disposição** aparecerá.
9. **Notificações de disposição** permitem que os usuários recebam alertas antecipados antes que um board seja automaticamente movido para a lixeira devido à inatividade. Esses alertas ajudam os usuários a tomar medidas caso queiram manter seu conteúdo.

   Se você deseja ativar as notificações de disposição:

   a. Clique em **Notificar**.

   b. Configure quantos dias antes a notificação deve ser enviada — qualquer valor entre **1 e 30 dias**.

   Se ao ativar notificações **alguns boards forem imediatamente movidos para a lixeira** (porque já passaram do limite), será perguntado se deseja notificar os usuários sobre esses boards específicos. Você pode escolher:

   - **Sim** – para notificar os titulares e cotitulares do board, mesmo que o board esteja sendo movido para a lixeira imediatamente.

   - **Não** – para mover os boards sem enviar uma notificação para esta ação imediata.

   Uma vez ativada, os usuários com boards no escopo de qualquer política de disposição com notificações ativadas:

   - Receberão uma notificação no **feed de notificações** do Miro durante a janela de inspeção configurada.

   - Poderão abrir o board diretamente da notificação.

   - Ver um **banner** no board avisando sobre a auto-movimentação para a lixeira, com uma opção de **Manter board** caso desejem retê-lo.

:::note
Criar, atualizar ou excluir uma política aciona o processo de políticas de disposição, que pode levar até 24 horas para ser concluído. No entanto, a atualização do nome ou da descrição de uma política ocorre imediatamente, pois essas atualizações não acionam o processo de políticas de disposição.
:::

#
