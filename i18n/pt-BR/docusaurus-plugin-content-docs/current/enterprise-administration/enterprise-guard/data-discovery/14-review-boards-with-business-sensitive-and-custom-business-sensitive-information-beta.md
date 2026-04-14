---
title: "Revisar boards com informa\xE7\xF5es confidenciais e personalizadas da empresa\
  \ (Beta)"
article_id: 24090123693586
translation_id: 24090123693586
locale: pt-br
sidebar_position: 13
created_at: '2025-01-21T15:10:56Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Com o Buscador de conteúdo, os [admins de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) podem revisar as ocorrências de correspondências de dados sensíveis da empresa ou dados sensíveis personalizados da empresa.

:::note
- Para revisar boards com correspondências de dados sensíveis da empresa ou dados sensíveis personalizados, você deve possuir a [função de admin de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, fale com seu Admin da empresa.
- As correspondências de dados sensíveis da empresa são classificadas como CLIENTE, TECNOLOGIA ou ESTRATÉGIA e os resultados aparecem no topo da lista de resultados.

- As correspondências de dados confidenciais personalizados da empresa são classificadas com as etiquetas personalizadas apropriadas.
:::

Para revisar um board com correspondências de dados sensíveis da empresa ou dados confidenciais personalizados, siga as seguintes etapas:

1. Se você estiver na página do **Content Explorer**, pule para a etapa 2.
   Se você não estiver na página do **Content Explorer**:
   a. Vá para suas [configurações da Miro](https://miro.com/app/settings).
   b. No painel esquerdo, em **Enterprise Guard**, clique no **Content explorer**.
   c. Clique em **Data discovery**.
2. Na página **Buscador de conteúdo/Descoberta de dados**, clique no board que deseja revisar.
   Um painel deslizante aparece à direita da tela.
3. O painel deslizante permite que você execute as seguintes ações:

   - Somente para correspondências de dados confidenciais personalizados: **Mostrar ou ocultar** **informações sensíveis da empresa**
   Por padrão, as informações sensíveis da empresa personalizadas são ocultadas. Se desejar visualizar essas informações, clique no botão de alternância **Mostrar informações sensíveis** para ativá-lo.
   dados confidenciais da empresa estiverem visíveis, você pode ocultar os dados clicando na opção **Mostrar informações confidenciais** para desativá-la.

   > ✏️ - As correspondências de dados confidenciais da empresa são rotuladas como CLIENTE, TECNOLOGIA ou ESTRATÉGIA e os resultados são listados no topo da lista de resultados.
   > - As correspondências de dados confidenciais personalizados da empresa são classificadas com as etiquetas personalizadas apropriadas.

   - Para correspondências de dados confidenciais da empresa e dados confidenciais personalizados da empresa: **Filtrar informações com base na categoria de dados confidenciais da empresa**
   Para visualizar os dados confidenciais da empresa que pertencem a uma categoria específica, clique na guia **Informações confidenciais da empresa** e, em seguida, clique no botão de filtro adequado abaixo da guia.

   -Somente para correspondências de dados sensíveis da empresa: **Suprimir correspondências de falso positivo**
   Durante o processo de descoberta de dados sensíveis da empresa, podem ocorrer situações em que o sistema gera correspondências que, embora tecnicamente precisas, podem não ser relevantes ou consideradas dados confidenciais de acordo com várias políticas de segurança e necessidades específicas de uma organização. Suprimir uma correspondência que não represente um risco de segurança ou para os negócios é essencial para adequar o processo de descoberta de dados aos requisitos específicos de segurança de dados e negócios de uma organização.

   Também pode haver momentos em que o sistema sinalize incorretamente os dados dos seus boards como provavelmente confidenciais (falso-positivos). Vários fatores contribuem para essas ocorrências, incluindo a proximidade de termos correlatos ou a formatação de dados relacionados ao negócio. Você também pode suprimir as correspondências falso-positivas.

   Ao suprimir uma correspondência, os dados são atualizados em tempo real. A classificação do board e as proteções aplicadas também são atualizadas de acordo com a configuração da classificação automática e das proteções inteligentes.

   Para suprimir uma correspondência falsa positiva, clique nos três pontos ao lado da correspondência de dados sensíveis da empresa que você deseja suprimir e selecione **Ocultar correspondência**. Vale ressaltar que as atualizações ocorrem em tempo real. A classificação do board e as proteções aplicadas também são atualizadas de acordo com a configuração da classificação automática e das proteções inteligentes.
4. Clique no próximo board em que deseja trabalhar na lista de resultados do buscador de conteúdo e realize as ações necessárias ou feche o painel deslizante clicando no botão **Fechar** no canto superior direito do painel.
