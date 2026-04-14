---
title: 'Mover dados entre regiões: migração automática'
article_id: 24866660560402
translation_id: 24866660560402
locale: pt-br
sidebar_position: 5
created_at: '2025-02-24T08:47:08Z'
updated_at: '2025-10-29T14:40:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Quem pode fazê-lo: Admins da empresa Quais planos: Enterprise Quais plataformas:
    Navegador, Desktop'
---

:::note
A migração automática é feita mediante contratação de um serviço profissional. Para pedir um orçamento, fale com seu contato da Miro.
:::

Este artigo explica o processo de migração automática de dados. Para saber mais sobre outras opções de migração de dados entre regiões, consulte [Mover dados entre regiões](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Dados incluídos em uma migração automática entre regiões

A lista a seguir mostra quais dados uma migração automática entre regiões inclui:

- Boards, conteúdo dos boards e configurações de compartilhamento de boards
- Hierarquia de conteúdo, incluindo times, Espaços e seções de Espaços
- Configurações da organização, times e boards
- Usuários, perfis e configurações de usuários, incluindo convidados
- Logs de auditoria, classificação de dados e configurações de segurança de conteúdo

## Prepare-se para a migração de dados entre regiões

Para preparar-se para a migração de dados entre regiões, siga estas etapas:

1. Verifique todos os domínios que você possui com a verificação de DNS para garantir o gerenciamento de todos os usuários do seu domínio.
2. Habilite a política de controle de domínio **Bloquear assinaturas próprias**, para evitar que os usuários criem, sem querer, assinaturas Free da Miro na sua região antiga.
3. Consolide times e/ou organizações em uma única organização com uma única assinatura.
4. Identifique quais integrações sua organização usa e precisará na nova região, e monte um cronograma para reconfigurar cada uma delas.

## Como funciona uma migração de dados entre regiões e quanto tempo leva

Uma migração entre regiões inclui as cinco etapas abaixo:

- **Preparação**
  Normalmente de 4 a 8 semanas. Com o suporte da Miro, o Admin da empresa prepara a organização para a migração, agenda o período de inatividade da migração e comunica aos usuários finais.
- **Migração**
  Normalmente menos de 8 horas de inatividade. A organização e seus dados são migrados para a nova região.

  > ✏️ A equipe da Miro coordena com você para selecionar a data da migração. Se a migração não for bem-sucedida por qualquer motivo, o acesso à sua região de origem é restaurado e a Miro coordena uma nova data de migração com você para tentar novamente.
- **Verificação e configuração**
  Normalmente de 2 a 3 semanas. O admin deve reconfigurar algumas integrações na nova região, como o logon único. O admin e os usuários finais verificam se seus boards e dados foram transferidos para a nova região, conforme esperado.
- **Treinamento**
  Normalmente de 2 a 3 semanas. Os usuários finais recebem instruções sobre como acessar sua nova organização na Miro.
- **Conformidade**
  Em até 120 dias após a data da migração, a Miro verifica se os dados da organização foram excluídos da região de origem.

## O que fazer após uma migração de dados entre regiões

Após uma migração de dados entre regiões, faça o seguinte:

- Se for o caso, reconfigure imediatamente o logon único para os novos subdomínios regionais. Por exemplo, au.miro.com.

  > ✏️ Para que seus usuários consigam fazer login na nova região, é necessário reconfigurar o logon único no IDP.
- Reconfigure o SCIM para os novos subdomínios regionais. Por exemplo, au.miro.com.
- Confira se **Bloquear assinaturas próprias** nas configurações de controle de domínio está habilitado.
- Valide suas outras configurações de controle de domínio.
- Reinstale e configure os aplicativos e as integrações relevantes.

## Perguntas frequentes sobre migrações automáticas de dados entre regiões

**O que é uma migração de dados entre regiões?**

As migrações de dados entre regiões automatizam a transferência dos dados dos clientes de uma região geográfica para outra. Uma migração entre regiões significa que os dados dos clientes da Miro dentro do escopo, serão armazenados e tratados na nova região

**Como funciona e quanto tempo leva?**

Confira Como funciona uma migração de dados entre regiões e quanto tempo leva.

**Quem é elegível e quem não é?**

Para automatizar uma migração entre regiões, você deve ser cliente Enterprise. No entanto, os clientes Enterprise que usam o Enterprise Guard e o EKM não são elegíveis. Para mais informações, fale com seu contato da Miro.

**Quais dados são incluídos em uma migração automática de dados entre regiões?**

Para saber quais dados uma migração automática entre regiões inclui, confira Dados incluídos em uma migração automática entre regiões.

**Quais dados não estão incluídos em uma migração automática de dados entre regiões?**

Uma migração automática entre regiões não inclui os seguintes dados:

- Aplicativos e integrações, como logon único e SCIM, que devem ser reconfigurados para a nova região
- Talktracks
- As notificações no aplicativo são apagadas

**Sim. Uma migração automática entre regiões é um serviço pago oferecido pelos Serviços da Miro. Para mais informações, fale com seu contato da Miro.**

Sim. Uma migração automática entre regiões é um serviço pago oferecido pelos Serviços da Miro. Para mais informações, fale com seu contato da Miro.

**De que forma a Miro garante que vai excluir os dados da minha organização da região de origem?**

Para remover seus dados da região de origem após uma migração entre regiões, a Miro segue o seguinte protocolo:

- Para garantir um backup confiável, os dados permanecem na região de origem por 30 dias, caso haja um problema com a migração.
- Após 30 dias, a Miro começa a excluir seus dados da região de origem.
- Em até 120 dias após a data da migração inicial, a Miro finaliza a exclusão de todos os dados da região de origem.

**O que os usuários veem durante uma migração entre regiões?**

Para saber mais sobre a experiência do usuário durante uma migração, consulte [Experiência do usuário ao mover dados entre regiões](../../canvas-25-admin-features/data-residency/04-user-experience-while-moving-data-between-regions.md).

**O que acontece se a migração não for bem-sucedida?**

Se a migração não for bem-sucedida por qualquer motivo, a Miro restaura o acesso à sua região de origem e coordena uma nova data para tentar novamente a migração.
