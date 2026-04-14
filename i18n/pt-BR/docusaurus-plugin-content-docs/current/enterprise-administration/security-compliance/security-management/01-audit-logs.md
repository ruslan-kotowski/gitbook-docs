---
title: Logs de auditoria
article_id: 360017571434
translation_id: 360017571434
locale: pt-br
sidebar_position: 1
created_at: '2019-02-11T10:09:04Z'
updated_at: '2026-03-12T09:21:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponível para: Enterprise Configurado por: Admins da empresa'
---

Os logs de auditoria permitem que admins da organização com privilégios relevantes acompanhem a atividade dos usuários na organização Miro. Os logs são extremamente úteis ao investigar um problema ou obter um relatório detalhado de eventos importantes (por exemplo, alterações nas configurações globais de segurança, convites de novos usuários ou novos boards criados).

:::note
Atualmente, os eventos são registrados a partir do momento da criação da assinatura Enterprise e são armazenados por 180 dias por padrão:
a) Se você fizer upgrade para Enterprise a partir de um plano diferente, os eventos serão registrados a partir do momento do upgrade.
b) Se você migrar alguns times para a assinatura Enterprise, os dados deles serão registrados apenas quando se tornarem parte da assinatura.
:::

## Acessando os logs de auditoria

Para acessar os logs de auditoria, siga as seguintes etapas:

1. Vá para **Configurações da empresa**.
2. No painel esquerdo, clique em **Segurança** > **Logs de auditoria**.
3. Você pode filtrar os logs de auditoria escolhendo um **Período de data**, um **Autor**, uma **Categoria de evento** e um **Evento** específico.

Clique no botão Visualizar eventos para visualizar os eventos que correspondem aos seus critérios de filtragem. O horário é exibido no formato **ISO 8601**, no fuso horário **local**. Você pode ver os detalhes de um evento específico clicando nos três pontos na coluna **Detalhes**.

:::note
Apenas eventos ocorridos nos últimos 90 dias estão disponíveis para visualização.
:::

## Exportar logs de auditoria

Você pode exportar logs no formato de arquivo **CSV**.

No arquivo de exportação CSV, a data e hora do evento são fornecidas no formato ISO 8601, no fuso horário UTC. Não há limite para o número de registros a serem exportados de uma vez; no entanto, quanto mais dados você exportar, maior será o tempo necessário para preparar o arquivo para download. Além disso, esteja ciente de que aplicativos populares para trabalhar com tabelas têm seus limites quanto ao volume de dados que podem abrir.

Para exportar logs, clique no botão **Exportar para CSV**.

A barra com os detalhes do arquivo de exportação aparecerá abaixo. Quando o arquivo estiver pronto para download, você poderá clicar no botão Baixar CSV. O arquivo estará disponível para download por 24 horas.

:::note
Atualmente, apenas um arquivo de exportação está disponível para download por organização de cada vez. Clicar no botão **Export to CSV** irá substituir o arquivo de exportação atual.
:::

## Acessar logs de auditoria via API

Admins podem utilizar a [API de Log de Auditoria](https://developers.miro.com/reference/audit-logs) ou as [Integrações de SIEM](https://help.miro.com/hc/sections/4404757427090-Security-information-and-event-management-SIEM) suportadas para acessar e coletar programaticamente os dados de logs de auditoria.

## Exclusão de logs de auditoria

Admins podem definir uma política de retenção para os logs de auditoria. Você pode escolher entre 30, 90, 180 ou 365 dias.

:::warning
Uma vez que os logs de auditoria são excluídos, eles não podem ser recuperados.
:::

:::note
A retenção indefinida para logs de auditoria foi obsoleta.
:::

Para definir um período de exclusão, faça o seguinte:

1. Vá para **Configurações da empresa**.
2. No painel à esquerda, clique em **Segurança** > **Logs de auditoria**.
3. Em **Logs de auditoria**, clique na guia **Configurações**.
4. Escolha uma opção na lista suspensa. Você será solicitado a confirmar sua escolha.

## Eventos nos logs de auditoria

Os logs de auditoria incluem registros sobre as seguintes categorias de eventos:

**Administração**

- Alterar nome da empresa
- Alterar, remover logotipo da empresa
- Solicitação de acesso criada
- Solicitação de acesso recusada
- Ativar, desativar métricas de atividade do usuário na Análise
- Ativar, desativar ou alterar configurações de logon único/SAML
- Ativar, desativar SCIM
- Gerar token para API SCIM
- Ativar, desativar notificações SCIM
- Ativar, desativar, alterar [lista de permissão](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Ativar, desativar compartilhamento com convidados fora dos domínios permitidos
- Ativar, desativar compartilhamento [via link público](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Ativar, desativar compartilhamento [via link público para edição](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Ativar, desativar [a privacidade do time](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Ativar, desativar, atualizar as configurações de [controle de domínio](../../canvas-25-admin-features/domain-control/01-domain-control.md)
- Ativar, desativar [Bloquear usuários desativados](../../user-management/02-block-deactivated-users.md)
- Alterar as [configurações de gerenciamento de solicitações](../../user-management/09-request-management-on-enterprise-plan.md) (incluindo alteração do e-mail do ServiceNow ou URL do service desk)
- Criar, excluir um time
- Alterar nome do time
- Alterar, remover logotipo do time
- Alterar as [configurações de convite do time](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Alterar [visibilidade do time](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Habilitar, desabilitar [convidados para um time](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Alterar as [configurações de compartilhamento padrão do board](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Alterar [as configurações padrão de compartilhamento de projeto](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Instalar, desinstalar um aplicativo
- [Aprovar, restringir um aplicativo](../../../integrations-apps/integrations-basics/04-how-to-install-apps.md)
- [Moderação do Miro AI](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md)

**Gerenciamento de usuários**

- Convidar um novo membro do time
- Converter um membro em convidado
- Converter um usuário para membro com acesso total
- Promover um usuário a Admin da empresa, revogar Admin da empresa
- Promover um usuário a admin do time, revogar admin do time
- Excluir um usuário de um time ou de uma empresa (se um usuário sair de um time, ele age tanto como ator quanto como objeto afetado)
- Revogar convite
- Desativar, reativar um usuário
- Usuário entra em um time/empresa

**Boards**

- Abrir um board
- Criar, excluir, restaurar um board
- Renomear um board
- Alterar a descrição do board
- Alterar a capa do board
- Mover um board para outro time
- Adicionar um board a um projeto, remover de um projeto, mover para outro projeto
- Mudar o titular do board
- Compartilhar um board com um visualizador/comentarista/editor
- Remover um usuário de um board
- Ativar, desativar, alterar [link público do board](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartilhar-boards-por-meio-de-um-link-publico)
- Ativar, desativar, alterar [senha de um board público](../../../using-miro/sharing-boards/13-password-protection-for-public-boards.md)
- Ativar, desativar, alterar [compartilhamento com a Empresa](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Ativar, desativar, alterar [compartilhamento com o time](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Exportar um board, baixar um arquivo de um board.
- Status criado
- Status atualizado
- Status excluído
- Carregar um arquivo (obsoleto, disponível em [Log de conteúdo](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md))

Por favor, note que o log de auditoria **não** registra informações relacionadas a mudanças em boards.

**Templates**

- Abrir um template
- Criar, excluir, restaurar um template
- Renomear um template
- Alterar o titular do template
- Status criado
- Status atualizado
- Status excluído

**Projetos**

- Criar, excluir um projeto
- Renomear um projeto
- Compartilhar um projeto com um usuário, remover um participante do projeto
- Ativar, desabilitar compartilhamento de time para um projeto
- Alterar um titular do projeto

**Logins**

- Entrar
- Falha ao entrar
- Sair
- Perfil bloqueado, desbloqueado

:::warning
Eventos de login incluirão a atividade de [usuários desativados](../../user-management/01-deactivated-users.md).
:::

**Detalhes do perfil**

- Alterar detalhes do perfil
- Solicitar alteração de endereço de e-mail
- Alterar endereço de e-mail

**Planos de ação**

- Criar um Plano de ação
- Excluir um Plano de ação
- Criar uma seção de Plano de ação
- Excluir uma seção de Plano de ação
- Alterar o titular de um Plano de ação

**Miro AI**

- Usar a funcionalidade da Miro AI

### Perguntas frequentes

Existe uma maneira de puxar automaticamente os logs de auditoria?

Sim, você pode configurar o [app da Miro para Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md) para acessar logs da Miro a partir do Splunk.
