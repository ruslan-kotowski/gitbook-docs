---
title: "Definir as prote\xE7\xF5es"
article_id: 16494716849810
translation_id: 16494716849810
locale: pt-br
sidebar_position: 4
created_at: '2024-01-19T19:01:45Z'
updated_at: '2025-11-25T15:40:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Definir proteções é o terceiro passo do fluxo de configuração de classificação automática e proteções. Nesta etapa do fluxo, você irá configurar as proteções, que são as restrições aplicáveis para cada nível de classificação, como bloquear o compartilhamento público, bloquear o compartilhamento com times, bloquear o compartilhamento com a organização ou bloquear a replicação de conteúdo. Por exemplo, você pode configurar proteções para bloquear o compartilhamento público, bloquear o compartilhamento com times, bloquear o compartilhamento com a organização e bloquear a replicação de conteúdo para usuários de boards classificados como CONFIDENCIAL.

### Pré-requisitos

- Você deve completar a primeira e a segunda etapa do fluxo de classificação automática e proteções, [1: Defina os níveis de classificação](07-define-classification-levels.md) e [2: Definir a classificação automática](07-define-classification-levels.md).
- Você deve conhecer as proteções que deseja atribuir a cada nível de classificação com base nos seus requisitos de segurança e governança.
- Você deve ter a [função de admin de conteúdo sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, entre em contato com seu Admin da empresa.

Os Admins têm duas opções para implementar Proteções Inteligentes em sua organização:
**Modo padrão:** Por padrão, as proteções não afetam as opções de compartilhamento ativas nos boards para evitar interrupções na colaboração em andamento, inclusive quando os boards são reclassificados durante a auto-classificação.

**Modo restrito:** Quando a opção Aplicar proteções no modo restrito está ativada, as proteções substituem todas as opções de compartilhamento ativas. Isso fornece aos Admins os níveis mais rigorosos de controle, mas também pode resultar em alguns usuários perdendo imediatamente o acesso aos boards.

![proteções.png](images/26201264700818_guardrails.png)

## Atribuir proteções

Para atribuir proteções a um nível de classificação, siga as seguintes etapas:

1. Na página **Definir proteções**, clique no ícone **Editar** do nível de classificação para o qual você deseja atribuir as proteções. Por exemplo, se você deseja atribuir proteções para o nível de classificação CONFIDENCIAL, clique no ícone de editar na linha do nível de classificação CONFIDENCIAL.
2. Marque a caixa de seleção para cada etiqueta de guardrail que deseja atribuir a este nível de classificação. Por exemplo, se você quiser bloquear o compartilhamento público, bloquear o compartilhamento com times, bloquear o compartilhamento com a organização, bloquear a replicação de conteúdo para os usuários de boards classificados como CONFIDENTIAIS, bloquear o compartilhamento fora de domínios permitidos e bloquear o uso do Miro AI, selecione as seguintes caixas de seleção:
   - **Bloquear a replicação de conteúdo**- **Bloquear uso da Miro AI (Beta)**
   - **Bloquear o compartilhamento público**
   - **Bloquear o compartilhamento com os times**
   - **Bloquear o compartilhamento com a organização**
   **- Bloquear o compartilhamento fora de domínios permitidos (Beta)**
   Após selecionar esta caixa de seleção, você deve adicionar os domínios que deseja permitir digitando e selecionando da lista de domínios permitidos na organização, ou digitando um novo domínio na caixa e clicando em + **Adicionar**.
   Para mais informações sobre cada conteúdo e proteções de compartilhamento, veja [Visão geral e cenários de Intelligent Guardrails](01-intelligent-guardrails-overview.md).
3. Por padrão, as proteções não afetam as opções de compartilhamento ativas nos boards para evitar interromper a colaboração em andamento, inclusive quando os boards são reclassificados durante a classificação automática.

   Se você deseja aplicar proteções e substituir todas as opções de compartilhamento ativas, ative o botão **Aplicar proteções no modo restrito**. Os usuários poderão perder o acesso aos boards. Isso fornece aos Admins os níveis mais rigorosos de controle, mas também pode resultar na perda imediata de acesso ao board por parte de alguns usuários.
   ![proteções.png](images/26201264700818_guardrails.png)
4. Clique em **Concluído**.
   Sua configuração está salva, mas só terá efeito após você clicar em **Publicar** na página [**Revisar impacto**](06-review-impact.md).
5. Quando terminar de definir as proteções para vários níveis de classificação, prossiga para [Completar configuração de proteções](05-define-guardrails.md).

## Configuração completa das proteções

Depois de terminar de atribuir proteções para diferentes níveis de classificação, clique em **Avançar**. Sua configuração está salva, mas só terá efeito após você clicar em **Publicar** na página [Rever impacto](06-review-impact.md).
