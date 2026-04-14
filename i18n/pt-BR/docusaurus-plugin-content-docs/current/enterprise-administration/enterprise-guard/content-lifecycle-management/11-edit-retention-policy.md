---
title: "Editar a pol\xEDtica de reten\xE7\xE3o"
article_id: 19205184829330
translation_id: 19205184829330
locale: pt-br
sidebar_position: 11
created_at: '2024-05-28T18:01:39Z'
updated_at: '2025-12-08T16:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Para editar políticas de retenção, você deve ter a [função de admin de governança de dados](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de governança de dados, fale com seu Admin da empresa.
:::

Para editar uma política de retenção, siga esses passos:

1. Vá para as suas [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Ciclo de vida do conteúdo**.
3. Clique na guia **Retenção**.
4. Na página de **políticas de retenção**, clique na política de retenção que deseja editar.
   A página com as informações relacionadas à política será aberta.
5. Clique em **Editar** no canto superior direito da página e edite o campo necessário. A tabela a seguir mostra cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | **Nome**  **(obrigatório)** | Nome da política de retenção.  Tamanho máximo: 60 caracteres. |
   | **Descrição**  **(opcional)** | Descrição desta política de retenção.  Tamanho máximo: 300 caracteres. |
   | **Período de retenção**  **(obrigatório)** | Impedir que boards sejam excluídos permanentemente por um período específico com base em um dos seguintes critérios: **Último acesso**, **Última modificação** ou **Criado em**. Selecione um número, escolha **meses** ou **anos**, e em seguida escolha a partir de qual evento o período de retenção é calculado.  Se quiser especificar o período de retenção em meses, selecione entre 1 e 120 meses.  Se quiser especificar o período de retenção em anos, selecione entre 1 e 10 anos. |
   | **Escopo**  **(obrigatório)** | Selecione o escopo desta política de retenção. O escopo indica a quais boards esta política de retenção se aplica. Você pode definir o escopo de uma política de retenção para todos os boards de uma organização ou para níveis específicos de classificação do board.  **Defina a política de retenção para todos os boards na organização** Se desejar definir o escopo da política de retenção para todos os boards na organização, na lista **Escopo**, selecione **Todos os boards na organização**.  **Defina a política de retenção para um ou mais times na organização** Se desejar definir o escopo da política de retenção para um ou mais times na organização, execute as seguintes etapas:  1. Na lista de **Escopo**, selecione **Time**. 2. Clique na caixa Inserir time e selecione cada time para o qual deseja aplicar a política de retenção. Uma marca de seleção aparece ao lado do time que você selecionou para associar à política de retenção.   ✏️ - Você pode selecionar vários times para uma política de retenção. Entretanto, qualquer time só pode estar associado a uma política de retenção por vez. - Você pode selecionar qualquer time, incluindo times excluídos, como escopo ao definir a política de retenção.   - Um time selecionado como escopo para uma política de retenção não pode ser excluído permanentemente até ser removido do escopo.  **Definir a política de retenção para um nível de classificação de board**  ✏️ Para definir o escopo da política de retenção para um nível específico de classificação do board, você deve garantir que a funcionalidade Classificação de dados esteja ativada. Uma vez que uma política de retenção utiliza um nível de classificação de board, não é possível desativar a funcionalidade Classificação de dados. Para mais informações, consulte a documentação sobre [Classificação de dados](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Se você deseja definir o escopo da política de retenção para um nível de classificação específico do board, siga estas etapas:  1. Na lista **Escopo**, selecione **Classificação**. 2. Clique na lista ao lado da lista de **Classificação** e, em seguida, selecione os níveis de classificação aos quais deseja aplicar a política de retenção. Você também pode pesquisar os níveis de classificação e, em seguida, selecioná-los.  Uma marca de seleção aparece ao lado dos níveis de classificação associados à política de retenção.  ✏️ **Notas:** - Você pode selecionar múltiplos níveis de classificação de uma vez. - Não é possível definir o mesmo nível de classificação para diferentes políticas de retenção. Se um nível de classificação específico já estiver associado a uma política de retenção, o nível de classificação aparecerá esmaecido.  - Após a aplicação de uma política de retenção a um nível de classificação do board, não é mais possível desabilitar a funcionalidade Classificação de dados.  -Depois que um nível de classificação é associado a uma política de retenção, não é possível excluir esse nível de classificação específico.  - Quando um board é regido por políticas de retenção tanto do escopo de todos os boards da organização quanto do escopo de classificação, a política com o período de retenção mais longo é aplicada. |
6. Quando terminar, clique em **Avançar**.
   A **página de Revisão de Impacto** aparece.
7. Revise o impacto da política de retenção. A página Revisar impacto mostra as seguintes informações:
   - **Resumo:** configuração da política de retenção, como nome da política, período de retenção e escopo.
   - **Impacto da política:** número de boards que serão regidos por esta política. A política de retenção também se aplica a boards na lixeira e eles estão incluídos no cálculo da revisão de impacto.

   > ✏️ Quando um board é regido por uma política de retenção baseada em tempo e outra baseada em classificação, a política com o período de retenção mais longo é aplicável.
8. Para salvar a configuração e aplicar a política de retenção, clique em **Publicar**.

:::note
Criar, atualizar ou excluir uma política aciona o processo de políticas de retenção, que pode levar até 24 horas para ser concluído. No entanto, a atualização do nome ou da descrição de uma política ocorre imediatamente, pois essas ações não acionam o processo de políticas de retenção.
:::
