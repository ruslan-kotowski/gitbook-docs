---
title: Amazon Q (Beta)
article_id: 31347586131346
translation_id: 31347586131346
locale: pt-br
sidebar_position: 3
created_at: '2025-11-25T13:35:45Z'
updated_at: '2025-12-29T15:25:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: 'Quem pode fazer: Titulares de boards, Cotitulares de boards, Editores de
    boards, Membros do time, Admins do time, Admins de usuários, Admins de conteúdo,
    Admins da empresa (Configuração); Admin de Amazon Q Quais planos: Business, Enterprise
    Quais plataformas: Navegador, Desktop'
---

A integração com Amazon Q permite que os times recuperem o conhecimento da empresa na plataforma Miro AI por meio dos Assistentes de IA e fluxos. A inteligência empresarial é entregue e visualizada diretamente dentro do Miro.

:::note
Você só pode usar a integração Amazon Q com a plataforma Miro AI. [Crie sua conta aqui](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb) para obter acesso.  Você será notificado quando a plataforma Miro AI for ativada para sua organização.
:::

O conhecimento empresarial frequentemente se encontra disperso em várias ferramentas como Slack, Confluence, Salesforce, Google Drive e repositórios internos, o que obriga gerentes de produto, líderes de engenharia e equipes de tecnologia a gastar tempo valioso procurando detalhes cruciais e alinhando insights.

As seguintes funcionalidades do Miro e do Miro AI dão suporte à integração Amazon Q:

- [**Fluxos**](../../using-miro/miro-ai/04-flows-overview.md)
  Visualize fluxos de trabalho que transformam informações dispersas em entregas claras, ajudando os times a automatizar e padronizar como transformam insights em ações.
- [**Sidekicks**](../../using-miro/miro-ai/06-sidekicks-overview.md)
  Trabalhe em conjunto com agentes de IA que analisam o conteúdo do board e os dados empresariais para gerar novos artefatos, oferecer insights instantâneos e acelerar a ideação, documentação e design.

## Configurar a integração Amazon Q

Certifique-se de que você está [inscrito aqui](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb) e de que recebeu confirmação da Miro de que a plataforma Miro AI está ativada para sua organização. Em seguida, complete os dois procedimentos a seguir.

Para configurar a integração Amazon Q com a Miro, é necessário adicionar a Miro como acessor de dados no Amazon Q Business e, em seguida, conectar o índice do Amazon Q ao console de admin na Miro.

### Adicionar a Miro como acessor de dados no Amazon Q Business

1. No console do Amazon Q Business, no painel de navegação, clique em **Aplicações**.
2. Clique na aplicação onde deseja adicionar um acessor de dados.
3. No painel de navegação, clique em **Acessores de dados**.
4. Clique em **Adicionar acessor de dados**.
5. Em **Acessores de dados**, para **Miro**, clique no ícone de mais (**+**).
6. Para **ID Externo**, adicione o ID da organização do Miro.
   Para obter o ID da organização no Miro, acesse o console de admin Miro. Copie o ID da organização da barra de URL do navegador.
   ![](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/31367058137746_image.png)
   *Encontre o ID da sua organização no console de admin. Você pode copiar o ID da barra de URL do navegador.*
7. Clique em **Adicionar acessor de dados**.
8. Anote os seguintes detalhes. Você precisará de cada valor para completar a configuração no console de admin da Miro:
   - ID do aplicativo
   - ARN do Aplicativo IdC
   - ID do Recuperador
   - Região do aplicativo
   - Região do aplicativo IdC

### Conecte um índice Amazon Q ao console de admin na Miro

1. No Miro, vá para **Admin Console** > **Apps e integrações** > **Apps** > **Adicionar apps**.
2. Pesquise e localize Amazon Q.

   > ✏️ Se você não conseguir encontrar Amazon Q pelo nome, então procure pelo seguinte ID de cliente: `1601842442647206821`.
3. No perfil do app, selecione se deseja adicionar o app para **Todos os times** ou **Times específicos**.
4. Revise a página de permissões.

   > ✏️ O app Amazon Q é desenvolvido e mantido pela Miro, e não requer permissões específicas.
5. Clique em **Adicionar**.
6. Vá para **Apps** > **Gerenciar Apps**.
7. Procure e localize Amazon Q.
8. Clique em **Configurações**.
9. Adicione os detalhes do data accessor Amazon Q. Veja o passo final em Adicionar Miro como data accessor no Amazon Q Business.
10. Clique em **Salvar**.
    Sua configuração foi aplicada.
