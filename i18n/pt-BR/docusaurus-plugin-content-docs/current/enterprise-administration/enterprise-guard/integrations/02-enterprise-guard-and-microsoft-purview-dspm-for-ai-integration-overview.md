---
title: "Vis\xE3o geral da integra\xE7\xE3o do Enterprise Guard e do Microsoft Purview\
  \ DSPM para IA (Beta)"
article_id: 28617278171154
translation_id: 28617278171154
locale: pt-br
sidebar_position: 0
created_at: '2025-08-07T15:17:38Z'
updated_at: '2026-01-12T11:27:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Para organizações que usam o Microsoft Entra ID (anteriormente Azure AD) como seu provedor de identidade, o Enterprise Guard encaminha com segurança os prompts e respostas de IA para o Microsoft Purview Data Security Posture Management (DSPM) para conformidade e times de segurança. Estas equipes podem então monitorar, auditar e controlar o uso de IA generativa de uma única plataforma confiável, reduzindo a sobrecarga operacional, mitigando riscos como vazamento e uso indevido de dados e fortalecendo a governança de IA de nível empresarial da Miro.

:::note
A versão Beta oferece suporte aos formatos da Miro AI, incluindo diagramas, mapas mentais, Documentos, protótipos, notas adesivas e Tabelas, mas não imagens. Estamos trabalhando para adicionar suporte a imagens e mais funcionalidades de IA nos próximos lançamentos.
:::

## **Para quem é**

Esta funcionalidade está disponível na versão Beta para clientes do Enterprise Guard que gerenciam a Miro e o Microsoft Entra ID (anteriormente Azure AD)/Microsoft Purview.

## **O que você ganha**

- **Visibilidade centralizada:** Visualizar o uso da Miro AI no hub de IA do Microsoft Purview.
- **Auditabilidade:** Os prompts (entradas do usuário) e as respostas (saídas de IA) são registrados para revisão.
- **Alinhamento de governança:** Use seus fluxos de trabalho do Purview existentes para monitoramento, alertas e retenção.

## **Requisitos**

### **Miro**

- Plano Enterprise com **Enterprise Guard** habilitado.
- Você é um **Admin da empresa**.
- Microsoft **Entra ID** configurado como provedor de logon único na Miro.
- Acesso à página de **Integrações Enterprise** (se você não conseguir vê-la, peça a um **Admin da empresa** para conceder acesso).
- Para habilitar esta funcionalidade na Beta, entre em contato com o seu Gerente de Sucesso do Cliente.

### **Microsoft**

- Licença ativa do **Microsoft Purview**.
- Seu **ID do locatário do Microsoft Entra ID** (o mesmo locatário usado para logon único na Miro; o GUID que identifica sua organização/locatário do Microsoft).
- Uma função do Entra que pode **conceder consentimento do administrador em nível de locatário** a um aplicativo.

## **Como funciona**

1. Um admin da Miro conecta seu locatário do Microsoft Entra a partir da página de **Integrações Enterprise** na Miro.
2. Isso instala o aplicativo de **governança Miro AI** no seu locatário Microsoft (via consentimento do administrador em nível de locatário).
3. Quando os usuários fizerem login na Miro através desse locatário e usarem o Miro AI, a Miro encaminha o prompt/resposta para o Microsoft Purview.
4. As atividades aparecem no **DSPM for AI → Activity explorer** (visualização do Purview que lista atividades de IA) no Microsoft Purview (considerar tempo de ingestão).

## **Visibilidade de dados & latência**

- Dados registrados: **Prompts e respostas de IA** gerados na Miro por usuários que fazem login via logon único para o locatário configurado.
- Onde ver: **Microsoft Purview → DSPM para IA → Explorador de atividades** (a visualização do Purview que lista as atividades de IA). Você também pode visualizar informações nos logs de auditoria.
  **Observação:** Todos os prompts e respostas baseados em texto nas funcionalidades da Miro AI são encaminhados para o Purview. Atualmente, o conteúdo de imagem não é encaminhado para o Microsoft Purview.
- Latência: Os registros geralmente aparecem **dentro de 10 a 30 minutos** após a ação da IA na Miro.

## **Limitações conhecidas**

- A versão Beta oferece suporte aos formatos da Miro AI, incluindo diagramas, mapas mentais, documentos, protótipos, notas adesivas e tabelas, mas não imagens. Estamos trabalhando para adicionar suporte a imagens e mais funcionalidades de IA nos próximos lançamentos.
- Você pode configurar **um ID de locatário do Microsoft Entra** na Miro por vez.
- Em ambientes com múltiplos IdP ou múltiplos locatários, **somente** atividades de usuários que fazem login na Miro pelo **locatário configurado** são registradas no Microsoft Purview.

## **Segurança e privacidade**

Miro encaminha prompts e respostas de IA para **seu tenant da Microsoft** para que possam ser monitorados no Purview. **Governança, retenção e controles de acesso** são gerenciados no seu ambiente Microsoft.

##

## **Perguntas frequentes**

- **P: Quais funcionalidades da Miro AI são registradas?**
  **R:** Todos os prompts baseados em texto e respostas de funcionalidades da Miro AI são encaminhados para o Purview. Atualmente, conteúdos de imagem não são encaminhados para o Microsoft Purview.
- **P: Isso cobre todos os usuários?**
  **R:** Apenas usuários que se autenticam na Miro usando o tenant da Microsoft Entra configurado estão cobertos.
- **P: Posso exportar logs da Miro?**
  **R:** Use o Microsoft Purview para exportação e retenção. A Miro encaminha atividades para o seu tenant da Microsoft, onde são regidas pelas suas políticas.
- **P: E quanto à segurança e privacidade?**
  **R:** A Miro encaminha prompts e respostas de IA para **seu tenant da Microsoft** para que possam ser monitorados no Purview. **Governança, retenção e controles de acesso** são gerenciados no seu ambiente Microsoft.

## **Suporte e recursos**

- Para os pré-requisitos de consentimento do Entra, consulte a documentação da Microsoft sobre **conceder consentimento de administrador para todo o tenant** a um aplicativo.
- Para instruções de configuração do Enterprise Guard, consulte [esta documentação](../../enterprise-subscription-management/integrations/03-set-up-microsoft-purview-dspm-for-miro-ai.md).
