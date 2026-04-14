---
title: "Revisar boards com informa\xE7\xF5es relacionadas \xE0 privacidade"
article_id: 15431051181458
translation_id: 15431051181458
locale: pt-br
sidebar_position: 15
created_at: '2023-11-29T16:31:14Z'
updated_at: '2025-11-25T15:39:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

O painel de Descoberta de Dados permite que [Admins de Conteúdo Sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) revisem ocorrências de dados relacionados à privacidade detectados pela descoberta de dados e validem os resultados.

:::note
Para revisar boards com dados relacionados à privacidade, você deve ter a [função de admin de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, fale com seu Admin da empresa.
:::

Para revisar um board com dados relacionados à privacidade, execute as seguintes etapas:

1. Vá para as suas [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard**, clique em **Descoberta de dados**.
3. Na página **Visão geral** de **descoberta de dados**, role até a seção abaixo das métricas e, em seguida, clique na contagem de boards para a categoria de boards que deseja revisar.
   Uma nova página aparece com a lista de boards e suas informações.
4. Clique no board que você deseja revisar.
   Um painel deslizante será exibido à direita da tela.
5. O painel deslizante permite que você execute as seguintes ações:
   - **Mostrar ou ocultar** **informações relacionadas à privacidade****:** Por padrão. informações relacionadas à privacidade são ocultadas. Caso queira visualizar informações relacionadas à privacidade, clique no botão **Mostrar informações confidenciais** para ativá-lo.
   Quando informações relacionadas à privacidade estiverem visíveis, você pode ocultar as informações relacionadas à privacidade clicando na opção **Mostrar informações confidenciais** para desativá-la.

   - **Filtrar** **informações relacionadas à privacidade** **com base na categoria de dados:** Para visualizar informações relacionadas à privacidade que pertencem a uma etiqueta específica, clique na guia **Informações relacionadas à privacidade** e, em seguida, clique na etiqueta de sensibilidade apropriada abaixo da guia.

   **- Suprimir correspondências falso-positivas:** No processo de descoberta de dados relacionados à privacidade, podem ocorrer situações em que o sistema gera correspondências que, embora tecnicamente precisas, podem não ser relevantes ou consideradas dados confidenciais com base em várias políticas de segurança e necessidades específicas de uma organização. Suprimir uma correspondência que não represente um risco de segurança ou de privacidade torna-se crucial para adequar o processo de descoberta de dados aos requisitos específicos de segurança de dados e privacidade de uma organização.

   Também pode haver situações em que o sistema sinalize erroneamente dados nos seus boards como provavelmente confidenciais (falso positivo). Vários fatores contribuem para essas ocorrências, incluindo a proximidade de termos correlatos ou a formatação de dados relacionados à privacidade. Você também pode suprimir as correspondências falso-positivas.

   Ao suprimir uma correspondência, os dados são atualizados em tempo real. A classificação do board e as proteções aplicadas também são atualizadas de acordo com a configuração da classificação automática e das proteções inteligentes.

   Para suprimir uma correspondência falso-positiva, clique nas reticências ao lado da correspondência de dados relacionados à privacidade que você deseja suprimir e selecione **Ocultar correspondência**. Vale ressaltar que as atualizações ocorrem em tempo real. A classificação do board e as proteções aplicadas também são atualizadas de acordo com a configuração da classificação automática e das proteções inteligentes.
6. Clique no próximo board em que deseja trabalhar na lista de resultados do Buscador de conteúdo e realize as ações necessárias, ou feche o painel deslizante clicando no botão **Fechar** no canto superior direito do painel.
