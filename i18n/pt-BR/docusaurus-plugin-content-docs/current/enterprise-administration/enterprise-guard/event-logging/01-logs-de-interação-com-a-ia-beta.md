---
title: "Logs de intera\xE7\xE3o com a IA (Beta)"
article_id: 34049604547858
translation_id: 34049604547858
locale: pt-br
sidebar_position: 1
created_at: '2026-03-15T21:28:41Z'
updated_at: '2026-03-16T09:09:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Os logs de interação com IA permitem que admins com o complemento Enterprise Guard coletem e revisem registros do uso da Miro AI em toda a organização. Ao habilitar os logs de interação com IA, os admins podem oferecer às equipes de segurança, conformidade e governança maior visibilidade sobre como as funcionalidades de IA são usadas e quais informações são processadas pelos sistemas de IA.

Os logs de interação com IA ajudam as organizações a:

- Monitorar como as funcionalidades de IA são usadas na organização
- Apoiar revisões de governança, conformidade e segurança
- Fornecer visibilidade sobre informações compartilhadas com sistemas de IA
- Fortalecer a confiança e a adoção responsável de ferramentas de IA

Os logs de interação com a IA capturam registros das interações entre os usuários e funcionalidades com inteligência artificial na Miro. Esses registros ajudam as organizações a revisar como a IA é utilizada em toda a organização e a apoiar processos internos de auditoria, governança e conformidade.

Quando ativados, os logs de interação com a IA capturam:

- Prompts dos usuários submetidos às funcionalidades de IA
- Respostas geradas pela IA retornadas pelo sistema
- Contexto do sistema associado à interação

## Antes de começar

- Você deve ser um admin para habilitar ou configurar logs de interação com a IA.
- O complemento Enterprise Guard é necessário para usar esta funcionalidade.
- Os logs de interação com a IA devem ser habilitados antes que a coleta de dados comece.
- Apenas interações que ocorrem após a habilitação dos logs são registradas.

## Habilitar logs de interação com a IA

1. Vá para **Console do Admin**.
2. Selecione **Segurança**.
3. Clique em **Logs de auditoria**.
4. Abra a guia **Configurações**.
5. Na seção **Logs de interação de IA**, ative **Coletar logs de interação de IA**.
6. Selecione o **período de retenção dos logs**.
7. Salve suas alterações.

Após ativar esta configuração, a Miro começa a coletar logs de interação de IA para novas interações de IA.

## Configurar retenção de logs

Os admins podem configurar por quanto tempo os logs de interação com a IA são armazenados.

1. Vá para **Admin console > Segurança > Logs de auditoria**.
2. Na seção **Logs de interação com a IA**, selecione o **período de retenção** desejado.
3. Salve suas alterações.

Os logs são automaticamente excluídos quando o período de retenção configurado expira.

## Acessar logs de interação com a IA via APIs

Os logs de interação com a IA podem ser recuperados usando a API de logs de interação com a IA.

Isso permite que as organizações exportem e analisem os dados de interação com a IA usando seus sistemas existentes de governança, conformidade ou monitoramento de segurança.

Casos de uso comuns incluem:

- Governança e supervisão de IA
- Monitoramento de segurança
- Auditoria de conformidade
- Investigações internas

Para mais informações, consulte a [documentação para desenvolvedores](https://developers.miro.com/reference/enterprise-get-ai-interaction-logs).

## Restrições

A versão atual inclui a versão inicial de registro de interações de IA. As seguintes restrições se aplicam:

- Invocações de ferramentas de funcionalidades de IA não são registradas atualmente.
- Interações relacionadas a integrações MCP da Miro não são registradas atualmente.
- Eventos de moderação e bloqueios de prompts sensíveis não são registrados atualmente.
- Imagens não estão incluídas nos registros de interação de IA.
