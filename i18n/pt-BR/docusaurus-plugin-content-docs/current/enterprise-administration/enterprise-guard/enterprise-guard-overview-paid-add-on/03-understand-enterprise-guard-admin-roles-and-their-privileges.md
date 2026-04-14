---
title: "Entenda as fun\xE7\xF5es de admin do Enterprise Guard e seus privil\xE9gios"
article_id: 15695755655954
translation_id: 15695755655954
locale: pt-br
sidebar_position: 1
created_at: '2023-12-11T18:33:53Z'
updated_at: '2026-03-12T22:21:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

As funcionalidades do Enterprise Guard são controladas através de privilégios de admin. Esses privilégios podem ser concedidos por meio de funções de admin predefinidas ou por meio de funções de admin personalizadas configuradas com os privilégios necessários.

A tabela a seguir lista os privilégios disponíveis para cada funcionalidade e mostra quais funções de admin predefinidas os incluem por padrão. Ao criar funções de admin personalizadas, Admins da empresa podem atribuir esses privilégios para conceder acesso a funcionalidades específicas do Enterprise Guard.

A tabela a seguir lista os privilégios detalhados e a matriz de funções de admin para cada funcionalidade.

|  |  |  |  |
| --- | --- | --- | --- |
| **Gerenciamento do ciclo de vida do conteúdo** | | | |
| **Privilégio** | **Admin de governança de dados** | **Admin de conteúdo sensível** | **Admin de eDiscovery** |
| Ver configurações da lixeira | ✅ | ❌ | ❌ |
| Editar configurações da lixeira | ✅ | ❌ | ❌ |
| Adicionar política de retenção | ✅ | ❌ | ❌ |
| Editar política de retenção | ✅ | ❌ | ❌ |
| Excluir política de retenção | ✅ | ❌ | ❌ |
| Adicionar política de disposição | ✅ | ❌ | ❌ |
| Editar política de disposição | ✅ | ❌ | ❌ |
| Excluir política de disposição | ✅ | ❌ | ❌ |
| **Classificação de dados** | | | |
| **Privilégio** | **Admin de Governança de Dados** | **Admin de Conteúdo Sensível** | **Admin de eDiscovery** |
| Visualizar configurações de classificação de dados | ❌ | ✅ | ❌ |
| Editar níveis de classificação | ❌ | ✅ | ❌ |
| Editar configurações de auto-classificação | ❌ | ✅ | ❌ |
| Editar configurações de proteções de classificação | ❌ | ✅ | ❌ |
| Editar nível de classificação padrão | ❌ | ✅ | ❌ |
| **Descoberta de dados** | | | |
| **Privilégio** | **Admin de Governança de Dados** | **Admin de Conteúdo Sensível** | **Admin de eDiscovery** |
| Ver etiquetas de privacidade | ❌ | ✅ | ❌ |
| Habilitar/desabilitar detecção de dados de privacidade | ❌ | ✅ | ❌ |
| Visualizar contagem de correspondências — etiquetas de privacidade | ❌ | ✅ | ❌ |
| Visualizar correspondências editadas — etiquetas de privacidade | ❌ | ✅ | ❌ |
| Visualizar correspondências completas — etiquetas de privacidade | ❌ | ✅ | ❌ |
| **eDiscovery** | | | |
| **Privilégio** | **Admin de Governança de Dados** | **Admin de Conteúdo Sensível** | **Admin de eDiscovery** |
| Gerenciar configurações de retenção legal | ❌ | ❌ | ✅ |
| Visualizar configurações de retenção legal | ❌ | ❌ | ✅ |

*Matriz detalhada de privilégios e funções de administrador predefinidas para cada funcionalidade*

> **NOTA:** As funcionalidades do Enterprise Guard podem ser concedidas por meio de funções de administrador predefinidas ou por funções de administrador personalizadas configuradas com os privilégios necessários.

## Atribuir uma função de Admin do Enterprise Guard

:::note
Para atribuir uma função de Admin do Enterprise Guard a um usuário, você deve ser um **Admin da empresa**.
:::

1. Vá para suas **configurações de perfil**:

   - A partir de um board: **Menu principal > Preferências > Configurações de perfil**.
   - A partir do painel: Clique no seu **avatar** no canto superior direito e clique em **Configurações**.
   - Pela URL: Acesse `https://miro.com/app/settings` e escolha sua **Empresa** na lista no canto superior esquerdo.
2. Em **Gerenciamento de Usuários**, clique em **Funções de Admin**.
3. No painel à direita, encontre a função de admin que você deseja atribuir (por exemplo, **Admin de Governança de Dados**, **Admin de Conteúdo Sensível** ou **Admin de eDiscovery**).
4. Clique no **elipses (… )** ao lado da função e selecione **Atribuir função**.
5. Escolha o usuário a quem você deseja atribuir a função.
6. Role até o final da janela e clique em **Atribuir**.

## Funções de admin personalizadas para o Enterprise Guard

As funções de admin personalizadas permitem que Admins da empresa concedam acesso a funcionalidades individuais do Enterprise Guard sem atribuir funções administrativas mais amplas. Isso permite que as organizações adaptem o acesso com base nas responsabilidades internas de governança, segurança ou conformidade.

Ao criar ou editar uma função de admin personalizada, os Admins da empresa podem selecionar as funcionalidades que determinam quais capacidades do Enterprise Guard a função poderá acessar e gerenciar. Essas funcionalidades abrangem vários domínios do Enterprise Guard, como Classificação de dados, Descoberta de dados, Gestão de ciclo de vida de conteúdo, e eDiscovery.

Ao atribuir apenas as funcionalidades necessárias, as organizações podem delegar tarefas administrativas, como revisar descobertas de conteúdo sensível, gerenciar configurações de classificação, configurar políticas de ciclo de vida ou acessar ferramentas de eDiscovery, para as equipes apropriadas. A tabela abaixo lista as funcionalidades que podem ser atribuídas ao configurar funções de admin personalizadas.

|  |  |  |
| --- | --- | --- |
| **Capability** | **Privilege** | **Description** |
| **Classificação de dados** | Visualizar configurações de classificação de dados | Admins podem visualizar as configurações de classificação da organização. |
| Editar configurações de classificação automática | Admins podem editar as configurações de classificação automática da organização. |
| **Descoberta de dados** | Visualizar configurações de descoberta de dados | Admins podem visualizar as configurações de descoberta de dados da organização. |
| Gerenciar configurações de descoberta de dados | O admin pode gerenciar as configurações de descoberta de dados da organização. |
| Visualizar resultados de descoberta de dados | O admin pode visualizar resultados relacionados à descoberta de dados. |
| Gerenciar resultados de descoberta de dados | O admin pode gerenciar resultados relacionados à descoberta de dados. |
| **eDiscovery** | Visualizar configurações de retenção legal | O admin pode visualizar as retenções legais na página de configurações de casos de eDiscovery. |
| Gerenciar configurações de retenção legal | O admin pode gerenciar as retenções legais na página de configurações de casos de eDiscovery. |
| Visualizar exportações de board | Admins podem visualizar exportações de board do eDiscovery. |
| Gerenciar exportações de board | Admins podem gerenciar exportações de board do eDiscovery. |
| **Gestão do ciclo de vida do conteúdo** | Visualizar configurações de lixeira | Admins podem visualizar as configurações de lixeira do board da organização. |
| Gerenciar configurações de lixeira | Admins podem gerenciar o tempo de permanência e permissões da lixeira do board da organização. |
| Visualizar configurações de retenção do ciclo de vida do conteúdo | Admins podem visualizar a página de configurações de retenção do ciclo de vida do conteúdo. |
| Gerenciar configurações de retenção do ciclo de vida do conteúdo | Admins podem gerenciar a página de configurações de retenção do ciclo de vida do conteúdo. |
| Visualizar configurações de disposição do ciclo de vida do conteúdo | Admins podem visualizar a página de configurações de disposição do ciclo de vida do conteúdo. |
| Gerenciar configurações de disposição do ciclo de vida do conteúdo | Admins podem gerenciar a página de configurações de disposição do ciclo de vida do conteúdo. |
| Visualizar conteúdo sob retenção ou disposição | Permite ao usuário visualizar o conteúdo impactado por políticas de retenção ou disposição. |
