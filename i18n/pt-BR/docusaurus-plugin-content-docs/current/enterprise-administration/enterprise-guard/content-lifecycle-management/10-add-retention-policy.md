---
title: "Adicionar pol\xEDtica de reten\xE7\xE3o"
article_id: 19205113739282
translation_id: 19205113739282
locale: pt-br
sidebar_position: 10
created_at: '2024-05-28T18:00:55Z'
updated_at: '2025-12-08T16:05:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Para adicionar políticas de retenção, você deve ter a [função de admin de governança de dados](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de governança de dados, entre em contato com o Admin da empresa.
:::

Para adicionar uma política de retenção, siga os seguintes passos:

1. Vá para suas [configurações do Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Ciclo de vida do conteúdo**.
3. Clique na guia **Retenção**.
   A página de **políticas de retenção** aparece.
4. Clique em **Adicionar política de retenção**.
   A página **Definir critérios** aparece.
5. Adicione ou selecione as informações apropriadas para cada campo. A tabela a seguir mostra cada campo e sua descrição.

   |  |  |
   | --- | --- |
   | **Campo** | **Descrição** |
   | **Nome**  **(obrigatório)** | Nome da política de retenção.  Tamanho máximo: 60 caracteres. |
   | **Descrição**  **(opcional)** | Descrição desta política de retenção.  Tamanho máximo: 300 caracteres. |
   | **Período de retenção**  **(obrigatório)** | Evite que boards sejam excluídos permanentemente por um período específico com base em um dos seguintes critérios: **Último acesso**, **Última modificação** ou **Criado em**. Selecione um número, escolha **Meses** ou **Anos**, e depois escolha a partir de qual evento o período de retenção será calculado.  Se especificar o período de retenção em meses, selecione um período de retenção entre 1 e 120 meses.  Se especificar o período de retenção em anos, selecione um período de retenção entre 1 e 10 anos. |
   | **Escopo**  **(obrigatório)** | Selecione o escopo desta política de retenção. O escopo indica a quais boards esta política de retenção se aplica. Você pode definir o escopo de uma política de retenção para todos os boards de uma organização ou para níveis específicos de classificação do board.  **Definir a política de retenção para todos os boards da organização** Se você deseja definir o escopo da política de retenção para todos os boards da organização, na lista **Escopo**, selecione **Todos os boards da organização**.  **Definir a política de retenção para um ou mais times da organização** Se você deseja definir o escopo da política de retenção para um ou mais times da organização, execute as seguintes etapas:  1. Na lista **Âmbito**, selecione **Time**. 2. Clique na caixa de entrada de time e selecione cada time ao qual você deseja aplicar a política de retenção. Um sinal de verificação aparece ao lado do time que você selecionou para associar à política de retenção.   ✏️ - Você pode selecionar vários times para uma política de retenção. No entanto, qualquer time só pode estar associado a uma política de retenção por vez.  - Você pode selecionar qualquer time, incluindo times excluídos, como escopo ao definir a política de retenção.   - Um time selecionado como escopo para uma política de retenção não pode ser excluído permanentemente até que o time seja removido do escopo.  **Defina a política de retenção para um nível de classificação de board**  ✏️ Para definir o escopo da política de retenção para um nível de classificação específico do board, você deve garantir que a funcionalidade Classificação de dados esteja ativada. Quando uma política de retenção utiliza um nível de classificação de board, não é possível desativar a funcionalidade Classificação de dados. Para mais informações, consulte a documentação sobre [Classificação de dados](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Se deseja definir o escopo da política de retenção para um nível de classificação específico de board, siga os passos abaixo:  1. Na lista de **Escopo**, selecione **Classificação**. 2. Clique na lista ao lado da lista de **Classificação** e selecione os níveis de classificação aos quais deseja aplicar a política de retenção. Você também pode pesquisar os níveis de Classificação e depois selecioná-los.  Uma marca de seleção aparece ao lado dos níveis de classificação que você selecionou para associar à política de retenção.  ✏️ **Notas:** - Você pode selecionar múltiplos níveis de classificação de uma só vez. - Não é possível definir o mesmo nível de classificação para diferentes políticas de retenção. Se um nível de classificação específico já estiver associado a uma política de retenção, o nível de classificação aparecerá esmaecido.  - Após a aplicação de uma política de retenção a um nível de classificação do board, não é mais possível desabilitar a funcionalidade Classificação de dados.  -Depois que um nível de classificação estiver associado a uma política de retenção, não será possível excluir esse nível de classificação específico. - Quando um board está sujeito tanto a políticas de retenção de todos os boards no escopo da organização quanto no escopo da classificação, aplica-se a política com o período de retenção mais longo. |
6. Clique em **Próximo**.
   A página **Revisar impacto** aparece.
7. Revise o impacto da política de retenção. A página Revisar impacto mostra as seguintes informações:
   - **Resumo:** configuração da política de retenção, como nome da política, período de retenção e escopo.
   - **Impacto da política:** número de boards que serão regidos pela política. A política de retenção também se aplica a boards na lixeira e eles estão incluídos no cálculo da revisão de impacto.

   > ✏️ Quando um board é regido por uma política de retenção baseada em tempo e outra baseada em classificação, a política com o período de retenção mais longo é aplicável.
8. Para salvar a configuração e aplicar a política de retenção, clique em **Publicar**.

:::note
Criar, atualizar ou excluir uma política aciona o processo de políticas de retenção, que pode levar até 24 horas para ser concluído. No entanto, a atualização do nome ou da descrição de uma política ocorre imediatamente, pois essas ações não acionam o processo de políticas de retenção.
:::

#
