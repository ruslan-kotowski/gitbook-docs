---
title: "Vis\xE3o geral dos Termos de Servi\xE7o personalizados"
article_id: 27375760557330
translation_id: 27375760557330
locale: pt-br
sidebar_position: 2
created_at: '2025-06-13T08:24:28Z'
updated_at: '2025-11-04T14:10:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

A funcionalidade de termos de serviço personalizados permite que os admins exibam um diálogo de Termos de Serviço personalizado para todos os membros internos de sua organização Miro. Isso garante que os usuários revisem e reconheçam os termos e políticas da sua organização antes de usar a Miro. Use essa funcionalidade para informar os usuários sobre as políticas de uso aceitável para as funcionalidades da Miro, incluindo o Miro AI. Os admins podem adicionar múltiplos links para políticas hospedadas externamente e configurar a recorrência para que os usuários sejam lembrados em um cronograma que atenda aos requisitos internos. Todas as ações relacionadas aos termos de serviço personalizados são registradas nos logs de auditoria para rastreabilidade.

:::note
Os Termos de Serviço Personalizados estão atualmente disponíveis apenas no aplicativo web e em navegadores.
:::

## Principais benefícios

- Exibir termos de serviço em toda a sua organização.
- Apresentar o diálogo de termos de serviço personalizados em pontos de uso relevantes: após login bem-sucedido ou ao interagir com o Miro AI.
- Impor a aceitação do usuário em um cronograma que você configura (dias, semanas ou meses) ou após atualizações.
- Vincular até três políticas hospedadas internamente ou externamente no idioma ou formato que preferir.
- Manter a auditabilidade nos logs de auditoria.

## Escopo

- Aplicável a: somente usuários internos, todos os membros da organização e admins.
- Excluídos: convidados e colaboradores externos.
- Disparadores:
  - Login realizado: exibido imediatamente após iniciar sessão.
  - Uso do Miro AI: exibido quando um usuário interage com o Miro AI (por exemplo, alternando o layout de IA, abrindo o painel lateral de IA ou iniciando uma ação de IA, como o Assistente de IA).
- Recorrência: configurável pelo admin em dias, semanas ou meses. Cada Termos de Serviço personalizado tem seu próprio status e recorrência. Padrão: duas semanas.
- Formato dos termos: o conteúdo deve ser hospedado externamente. A Miro referencia os links e não armazena o texto completo da política.
- Links: até três links de política, cada um com uma etiqueta clara.
- Configuração: você pode configurar um termo de serviço personalizado para cada gatilho (login bem-sucedido e uso do Miro AI). Cada termo de serviço personalizado tem seu próprio status e recorrência.

## Quem pode usar esta funcionalidade?

Os admins devem ter os seguintes privilégios do Enterprise Guard para visualizar e gerenciar os Termos de Serviço Personalizados:

- **Admin de conteúdo sensível:** possui permissões integradas.
- **Funções de admin personalizadas**, devem incluir:
  - Visualizar Termos de Serviço personalizados
  - Gerenciar Termos de Serviço personalizados

## Como funciona

1. **Configurar condições:** escolha o gatilho (login bem-sucedido ou uso de IA), escopo (membros internos) e recorrência.
2. **Adicionar conteúdo:** forneça um título conciso, descrição curta e até três links rotulados para políticas hospedadas externamente.
3. **Revisar e ativar:** visualize o diálogo final com o usuário e ative a configuração.
4. **Aplicação:**

- **Login bem-sucedido:** o diálogo não pode ser dispensado. Usuários devem aceitar para prosseguir ou sair.
- **Uso de IA:** o diálogo permite **Continuar** ou **Cancelar**. Cancelar mantém o usuário logado com funcionalidades de IA desabilitadas.

5. **Registro:** alterações de configuração e aceitações de usuários são registradas nos logs de auditoria.

### Experiência do usuário

- **Login bem-sucedido**

  - A janela de diálogo aparece imediatamente após iniciar sessão.
  - Os usuários podem clicar em **Continuar** para aceitar e prosseguir, ou em **Sair**.
- **Uso do Miro AI**

  - A janela de diálogo aparece quando o usuário interage com o Miro AI, como ao alternar o layout do AI, abrir o painel lateral do AI ou iniciar uma ferramenta ou ação de AI (por exemplo, Assistente de IA).
  - Os usuários podem clicar em **Continuar** para aceitar e usar as funcionalidades de AI. Se os usuários clicarem em **Cancelar**, eles permanecem logados e podem continuar usando todas as funcionalidades que não sejam de AI.
- Os usuários não são solicitados novamente até que o intervalo de recorrência termine ou os termos sejam atualizados.

## Comportamento de aceitação

- **Gatilho de login:** os usuários devem aceitar conforme a programação configurada ou serão desconectados. O diálogo não pode ser contornado.
- **Gatilho de uso de IA:** os usuários podem aceitar para ativar as funcionalidades de IA ou cancelar para manter as funcionalidades de IA desabilitadas. Cancelar mantém o usuário logado e capaz de usar funcionalidades não relacionadas à IA.
- **Recorrência e versões:** os usuários não serão solicitados novamente até que o período de recorrência termine ou uma nova versão seja publicada, conforme o gatilho configurado.

##

###
