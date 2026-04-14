---
title: "Suprimir uma correspond\xEAncia de conte\xFAdo sens\xEDvel"
article_id: 17144258002962
translation_id: 17144258002962
locale: pt-br
sidebar_position: 10
created_at: '2024-02-20T00:16:59Z'
updated_at: '2025-11-25T15:41:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Durante o processo de descoberta de dados, você pode encontrar situações em que o sistema gera correspondências que, embora sejam tecnicamente precisas, podem não ser relevantes ou consideradas como dados confidenciais de acordo com várias políticas de segurança e requisitos específicos de uma organização. Suprimir uma correspondência que não represente um risco de segurança ou privacidade é essencial para adequar o processo de descoberta de dados aos requisitos específicos de segurança e privacidade de dados de uma organização.

Também pode haver situações em que o sistema sinaliza de forma incorreta os dados dos seus boards como provavelmente sensíveis (falso-positivo). Vários fatores contribuem para essas ocorrências, incluindo a proximidade de termos relacionados ou a formatação de dados confidenciais. Você também pode suprimir as correspondências falso-positivas.

Ao suprimir uma correspondência, os dados são atualizados em tempo real. A classificação do board e as proteções aplicadas também são atualizadas de acordo com a configuração da classificação automática e das proteções inteligentes.

:::note
Para suprimir uma correspondência de conteúdo sensível, você deve ter a [função de admin de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, entre em contato com seu Admin da empresa.
:::

Para suprimir uma correspondência de conteúdo sensível, siga as seguintes etapas:

1. Se você estiver na página **Buscador de conteúdo**, pule para a etapa 2.
   Se não estiver na página **Buscador de conteúdo**, faça o seguinte:
   a. Vá para as suas [configurações da Miro.](https://help.miro.com/hc/articles/https://miro.com/app/settings)
   b. No painel esquerdo, em **Segurança e conformidade**, clique em **Buscador de conteúdo**.
2. Na página **Buscador de conteúdo/Descoberta de dados**, clique no board que deseja revisar.
   Um painel deslizante é exibido à direita da tela.
   ![Figura 1: painel deslizante](images/21017529212690_slide_out_panel.png)*Figura 1: painel deslizante*
3. Clique nas reticências ao lado da correspondência de dados confidenciais que deseja suprimir e selecione **Ocultar correspondência**. Vale ressaltar que as atualizações ocorrem em tempo real. A classificação do board e as proteções aplicadas também são atualizadas de acordo com a configuração da classificação automática e das proteções inteligentes.

    Ao suprimir uma correspondência, os dados são atualizados em tempo real. A classificação do board e as proteções aplicadas também são atualizadas conforme a configuração da classificação automática e das proteções inteligentes.

   Repita esta etapa para cada correspondência de dados confidenciais que deseja suprimir.
4. Clique no próximo board em que deseja trabalhar na lista de resultados do buscador de conteúdo e realize as ações necessárias ou feche o painel deslizante clicando no botão **Fechar** no canto superior direito do painel.
