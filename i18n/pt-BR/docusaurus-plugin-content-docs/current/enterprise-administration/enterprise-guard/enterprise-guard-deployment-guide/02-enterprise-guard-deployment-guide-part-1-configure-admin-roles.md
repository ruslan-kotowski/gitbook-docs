---
title: "Guia de implanta\xE7\xE3o do Enterprise Guard , parte 1: Configurar fun\xE7\
  \xF5es de admin"
article_id: 17120595534994
translation_id: 17120595534994
locale: pt-br
sidebar_position: 1
created_at: '2024-02-19T09:19:59Z'
updated_at: '2025-11-25T15:41:04Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Os Admins da empresa podem conceder a si mesmos e a outros funções admin adicionais quando o Enterprise Guard estiver habilitado. Como resultado, o número de Admins da empresa em sua organização deve ser reduzido ao mínimo. Considere cuidadosamente sua configuração de admin existente e mova os Admins da empresa para outras funções (como admin de time ou usuário ) quando apropriado para equilibrar segurança, conformidade e eficiência operacional.

Embora seja recomendado, uma reavaliação holística da sua configuração de admin não é necessária para implantar o Enterprise Guard. Passar para [Parte 2: Implantar Segurança de Dados](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md)a seu critério.

## Visão geral das funções de admin do Miro

Aqui está uma lista de funções admin disponíveis no Miro , incluindo uma descrição das responsabilidades e para quem elas são adequadas em uma organização típica.

:::note
Observações:
- Esta é uma lista em evolução de funções e privilégios. Consulte esta página periodicamente para ficar por dentro das atualizações.
- Para atribuir a função de admin de governança de dados ou admin de conteúdo sensível a um usuário, você deve ser um Admin da empresa.
:::

|  |  |  |
| --- | --- | --- |
| **Função de admin** | **Responsabilidades** | **Recomendado para** |
| **Admins da empresa** | Responsável pela gestão geral e delegação de responsabilidades específicas a outras funções admin . Deve ter um amplo entendimento das necessidades operacionais e obrigações de conformidade da organização. | - admins de TI seniores - Gerentes de Departamento - Gerentes de Projeto - Líderes de Team - Gerentes de Operações - Gerentes de Tecnologia Business - titular do produto Miro |
| **Admins do time** | Gerencie configurações específicas da equipe e o acesso do usuário dentro de suas respectivas times. Garante a autonomia da time ao mesmo tempo em que se alinha com políticas organizacionais mais amplas. | - Gerentes de Departamento - Gerentes de Projeto - Líderes de Team - Gerentes de Operações |
| **Admins de usuários** | Lidar com gerenciamento de usuário e licenças. Ideal para gerenciar acessos e contas de funcionários. Gerencie usuários com eficiência sem sobrecarregar os admins do time. | - Gerente de TI - admins de TI - Central de Serviço de TI |
| **admins de governança de dados (Enterprise Guard)** | Responsável pela conformidade e governança de dados. Deve entender o cenário legal e regulatório relevante para os dados da organização, incluindo as políticas de retenção e disposição da organização. | - Diretor de Conformidade (CCO) - Gerente de Governança de Dados - Gerente de conformidade - Gerente de Assuntos Regulatórios - Gerenciador de risco - Gerente de Registros - Analista de eDiscovery - Analista Forense |
| **admins de eDiscovery (Enterprise Guard)** | Gerencie as configurações de retenção legal para preservar boards relevantes para investigações em andamento ou processos legais. Isso inclui criar, modificar e liberar retenções ou casos legais para impedir a exclusão permanente de conteúdo, garantindo a conformidade com obrigações legais e regulatórias. Essa função é crucial para organizações que exigem preservação rigorosa de dados para dar suporte a procedimentos legais e mandatos de conformidade . | - Assessoria Jurídica - Especialistas em eDiscovery - Responsáveis pela conformidade - Gestores de Risco - Analistas Forenses - Diretor de Segurança da Informação (CISO) - Encarregado da Proteção de Dados (RPD) - Responsável pela privacidade/Gerente de privacidade |
| **admins de conteúdo sensível (Enterprise Guard)** | Responsável pela proteção de dados e privacidade. Crucial para classificar, gerenciar e proteger informações confidenciais em toda a organização. Importante para lidar com PII, PHI, PCI ou propriedade intelectual. | - Diretor de Segurança da Informação (CISO) - Encarregado da Proteção de Dados (RPD) - Responsável pela privacidade/Gerente de privacidade - Analista de Segurança Cibernética - Consultor de Segurança de TI |

:::tip
Saiba mais sobre [funções de admin e seus privilégios](../enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) no plano Enterprise .
:::

## Matriz detalhada de privilégios e funções de admin do Enterprise Guard

A tabela a seguir lista os privilégios detalhados e a matriz de funções de admin para cada recurso.

|  |  |  |  |
| --- | --- | --- | --- |
| **Gerenciamento do ciclo de vida do conteúdo** | | |  |
| **Privilégio** | **Admin de governança de dados** | **Admin de conteúdo sensível** | **Admin de eDiscovery** |
| Visualizar configurações da lixeira | ✅ | ❌ | ❌ |
| Editar configurações de lixeira | ✅ | ❌ | ❌ |
| Adicionar política de retenção | ✅ | ❌ | ❌ |
| Editar a política de retenção | ✅ | ❌ | ❌ |
| Excluir políticas de retenção | ✅ | ❌ | ❌ |
| Adicionar política de disposição | ✅ | ❌ | ❌ |
| Editar política de disposição | ✅ | ❌ | ❌ |
| Excluir a política de disposição | ✅ | ❌ | ❌ |
| **Classificação de dados** | | |  |
| **Privilégio** | **Admin de governança de dados** | Admin de conteúdo sensível | **Admin de eDiscovery** |
| Visualizar configurações de classificação de dados | ❌ | ✅ | ❌ |
| Editar níveis de classificação | ❌ | ✅ | ❌ |
| Editar configurações de classificação automática | ❌ | ✅ | ❌ |
| Editar configurações de proteção de classificação | ❌ | ✅ | ❌ |
| Editar nível de classificação padrão | ❌ | ✅ | ❌ |
| **Visibilidade de dados** | | |  |
| **Privilégio** | **Admin de governança de dados** | **Admin de conteúdo sensível** | **Admin de eDiscovery** |
| Visualizar etiquetas de privacidade | ❌ | ✅ | ❌ |
| Habilitar/desabilitar a detecção de dados de privacidade | ❌ | ✅ | ❌ |
| Visualizar contagem de correspondências — etiquetas de privacidade | ❌ | ✅ | ❌ |
| Visualizar correspondências editadas — etiquetas de privacidade | ❌ | ✅ | ❌ |
| Visualizar detalhes das correspondências — etiquetas de privacidade | ❌ | ✅ | ❌ |
| **eDiscovery** | | |  |
| **Privilégio** | **Admin de governança de dados** | **Admin de conteúdo sensível** | **Admin de eDiscovery** |
| Gerenciar configurações de retenção legal | ❌ | ❌ | ✅ |
| Visualizar configurações de retenção legal | ❌ | ❌ | ✅ |

*Tabela 2: Privilégios detalhados e matriz de funções de admin para cada recurso*

## Transição da sua configuração de admin

### Audite sua configuração de admin atual

Revise a lista de usuários que têm direitos de admin no Miro e suas responsabilidades. Use a Ferramenta de Avaliação de Configuração do admin para gerar um resumo do status atual.

- Filtre a lista de usuários da seção **Usuários ativos** das Configurações da empresa para visualizar os Admins da empresa.
- Visualize a lista de admins de usuários, admins de governança de dados e admins de conteúdo confidencial usando a seção **Função de admin** das configurações da empresa.

### Mapear uma nova configuração de admin

Compare sua configuração de admin atual com a tabela acima e as políticas da sua empresa. Use a Ferramenta de Avaliação de Configuração do admin para gerar uma nova configuração.

Considere questões como:

- Quem precisa da função de Governança de Dados?
- Quem precisa da função de Conteúdo Sensível?
- Quais Admins da empresa podem ser transferidos para admins de usuários?
- Quais Admins da empresa podem ser transferidos para admins do time?

### Reatribuir funções e informar os usuários

Os artigos da Central de ajuda abaixo mostram como atribuir as diversas funções. Para sua conveniência, personalize os templates de e-mail fornecidos para informar os usuários sobre as transições.

- [Como atribuir Admins da empresa e admins do time](../../../administration/user-management/06-how-to-manage-admin-roles.md)
- [Como atribuir admins de usuários, admins de governança de dados e admins de conteúdo sensível](../enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)

### Atribuir a função de admin de governança de dados

:::note
Para atribuir a função de admin de Governança de Dados a um usuário, você deve ser um Admin da empresa.
:::

1. Vá para as configurações do seu perfil.
   - De um board: **Menu principal > Preferências > Configurações do perfil**.- No painel: clique no seu avatar no canto superior direito e clique em **Configurações**.
   - Da URL `https://miro.com/app/settings`: Selecione sua empresa na lista no canto superior esquerdo.
2. Em “Gerenciamento de usuários”, clique em Funções de admin.
3. No painel direito, clique nas reticências do **admin de governança de dados** **(****…)**e selecione **Atribuir função**.
4. Escolha o usuário ao qual você deseja atribuir a função de admin de Governança de Dados, role até a parte inferior da janela e clique em **Atribuir**.

### Atribuir a função de admin de conteúdo sensível

:::note
Para atribuir a função de admin de conteúdo Sensível a um usuário, você deve ser um Admin da empresa.
:::

1. Vá para as configurações do seu perfil.
   - De um board: **Menu principal > Preferências > Configurações do perfil**.- No painel: clique no seu avatar no canto superior direito e clique em **Configurações**.
   - Da URL `https://miro.com/app/settings`: Selecione sua empresa na lista no canto superior esquerdo.
2. Em “Gerenciamento de usuários”, clique em Funções de admin.
3. Nopainel direito, clique nas reticências **admin de conteúdo sensível** **(****…)**e selecione **Atribuir função**.
4. Escolha o usuário ao qual você deseja atribuir a função de admin de conteúdo Sensível, role até a parte inferior da janela e clique em **Atribuir**.

### Atribuir a função de admin do eDiscovery

:::note
Para atribuir a função de admin do eDiscovery a um usuário, você deve ser um Admin da empresa.
:::

1. Vá para as configurações do seu perfil.
   - De um board: **Menu principal > Preferências > Configurações do perfil**.- No painel: clique no seu avatar no canto superior direito e clique em **Configurações**.
   - Da URL `https://miro.com/app/settings`: Selecione sua empresa na lista no canto superior esquerdo.
2. Em “Gerenciamento de usuários”, clique em Funções de admin.
3. Nopainel direito, clique nas reticências do **admin do eDiscovery** **(****…)**e selecione **Atribuir função**.
4. Escolha o usuário ao qual você deseja atribuir a função de admin do eDiscovery, role até a parte inferior da janela e clique em **Atribuir**.

### Recursos

- [Ferramenta de avaliação de configuração do admin](https://docs.google.com/spreadsheets/d/1a0WQc-fBpuVwfnoY8VCx66PjOXS76q7DJ__xDYcp8rk/edit?usp=sharing) (faça uma cópia)
- [templates de e-mail | Comunicações de configuração do admin](https://docs.google.com/document/d/18Kw4GNPq7GnAx8R8co5PaZ04peVogfVDgsdKK2MuARM/edit?usp=sharing) (faça uma cópia)
