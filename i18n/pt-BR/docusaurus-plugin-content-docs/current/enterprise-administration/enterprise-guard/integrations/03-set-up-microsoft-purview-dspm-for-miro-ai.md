---
title: Configurar Microsoft Purview DSPM para Miro AI (Beta)
article_id: 28698434922386
translation_id: 28698434922386
locale: pt-br
sidebar_position: 8
created_at: '2025-08-11T19:20:50Z'
updated_at: '2026-01-12T11:28:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Use este procedimento para configurar o Microsoft Purview Data Security Posture Management (DSPM) para Miro AI, de modo que prompts e respostas da Miro apareçam no DSPM para IA do Microsoft Purview. Após a configuração, você validará os eventos e aprenderá a gerir a integração.

## **Pré-requisitos**

### **Miro**

- Plano Enterprise com **Enterprise Guard** ativado.
- Você é um **Admin da empresa**.
- **Microsoft Entra ID** está configurado como um **provedor de SSO** na Miro.
- Para habilitar esta funcionalidade em Beta, entre em contato com seu Gerente de Sucesso do Cliente.

### **Microsoft**

- Licença ativa do Microsoft Purview com suporte para DSPM para AI.
- ID do locatário do Microsoft Entra ID usado para logon único no Miro (o GUID que identifica sua organização/locatário da Microsoft).
- Uma função Entra que pode conceder consentimento administrativo para toda a organização a um aplicativo.

## **Configurar a integração na Miro**

1. Na Miro, abra **Configurações Enterprise → Integrações Enterprise**.
2. Role para baixo e clique para ativar o **Microsoft Purview DSPM para AI.**
3. No campo ID do Locatário, insira seu **ID do locatário Microsoft Entra**.
4. Clique em **Conectar**.
5. Quando solicitado, faça login no Microsoft Entra com uma conta que possa conceder **consentimento administrativo para todo o locatário**.
6. Revise o consentimento para o aplicativo **governança do Miro AI** e clique em **Aceitar**.
7. Retorne à Miro e verifique se a integração mostra **Conectado.**

## **Validar atividade no Microsoft Purview**

1. Na Miro, execute uma ação simples de IA (por exemplo, **resuma** notas adesivas em um board).
2. Aguarde **até 10–30 minutos** para a ingestão.
3. No Microsoft Purview, vá para **Microsoft Purview → DSPM para IA → Explorador de atividades** (a visualização do Purview que lista as atividades de IA). Você também pode visualizar informações nos logs de auditoria.
   Nota: Todos os prompts baseados em texto e respostas de funcionalidades do Miro AI são encaminhados para o Purview. Atualmente, conteúdos de imagem não são encaminhados para o Microsoft Purview.
4. Filtre por eventos **Recentes** e localize atividades da Miro (por exemplo, prompt e resposta).

## **Gerenciar a integração**

- **Desconectar**: No Miro, vá para **Integrações corporativas → Microsoft Purview para AI → Desconectar**.
- **Mudar inquilino**: **Desconecte** primeiro, depois **Conecte-se** novamente usando um **ID de inquilino** diferente.

## **Resolução de problemas**

- **Opção de integração ausente**: Certifique-se de que sua organização possui **Enterprise Guard** e que sua conta pode acessar **Integrações corporativas**. Peça a um **Admin da empresa** para conceder acesso.
- **ID de inquilino inválido ou erro de conexão**: O ID de inquilino deve **corresponder exatamente** ao inquilino Microsoft Entra usado para **SSO** no Miro.
- **Consentimento falhou ou loop de autenticação**: Faça login com uma conta que possa conceder **consentimento do admin para todo o inquilino** (trabalhe com seu administrador Microsoft).
- **Nenhuma atividade visível**: Verifique se uma ação de IA teste foi executada por um usuário que acessa a Miro por meio do **tenant configurado**; permita **10 a 30 minutos**; confirme sua **licença do Purview**; e cheque o **DSPM para AI → Explorador de atividades**.
- **Múltiplos tenants/IdPs**: Apenas **um tenant** pode ser configurado na Miro. Atividades de usuários que fazem logon único por SSO em outros tenants/IdPs **não** são encaminhadas.

## **Limitações conhecidas**

Para mais informações, consulte a [seção de limitações conhecidas na documentação de visão geral](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).
