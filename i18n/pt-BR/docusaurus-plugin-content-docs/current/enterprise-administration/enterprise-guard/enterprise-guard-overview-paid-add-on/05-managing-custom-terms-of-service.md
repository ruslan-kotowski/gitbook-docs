---
title: "Gerenciando Termos de Servi\xE7o personalizados"
article_id: 27621616452882
translation_id: 27621616452882
locale: pt-br
sidebar_position: 3
created_at: '2025-06-24T23:29:13Z'
updated_at: '2025-11-04T14:10:40Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

## Criando Termos de Serviço personalizados

:::note
Notas:

- Os admins devem ter os seguintes privilégios do Enterprise Guard para visualizar e gerenciar os Termos de Serviço personalizados:
  - O admin de conteúdo sensível tem permissões integradas.
  - As funções de admin personalizadas devem incluir:
    - Visualizar Termos de Serviço personalizados
    - Gerenciar Termos de Serviço personalizados
- Convidados e usuários externos são excluídos.
- A Miro não armazena os termos, apenas o link e os metadados.
:::

1. Vá para **Configurações** > **Enterprise Guard** > **Termos de Serviço Personalizados**.
2. Se você estiver criando Termos de Serviço personalizados pela primeira vez, clique em **Adicionar Termos de Serviço**.
   Se você já possui uma configuração existente e deseja adicionar outra, clique em **Criar novo** na visualização de lista.
3. Em **Configurar** → **Condições**:
   - **Gatilho**: Escolha entre **Login bem-sucedido** ou **Uso de IA**.
     **Login bem-sucedido**

     - O diálogo aparece imediatamente após o iniciar sessão.
     - Os usuários podem clicar em **Continuar** para aceitar e prosseguir, ou em **Sair**.

     **Uso de IA**

     - O diálogo aparece quando o usuário interage com o Miro AI, como ao alternar o layout do AI, abrir o painel lateral do AI ou iniciar uma ferramenta ou ação de AI (por exemplo, Assistente de IA).
     - Os usuários podem clicar em **Continuar** para aceitar e usar as funcionalidades de AI. Se os usuários clicarem em **Cancelar**, permanecem conectados e podem continuar usando todas as funcionalidades não relacionadas ao AI.
   - **Âmbito**: **Todos os usuários e admins na organização**.
   - **Período de recorrência**: insira um número e selecione **Dias**, **Semanas** ou **Meses**.Padrão: duas semanas.
     Os usuários não serão solicitados novamente até que o período de recorrência termine ou os termos sejam atualizados.
4. Em **Configurar** → **Conteúdo**:
   - **Título** (máximo de 32 caracteres)
   - **Descrição** (máximo de 200 caracteres)
   - **Link:** Links de política (hospedados externamente). Para incluir links adicionais, clique em +Adicionar link. Até três links são suportados. Cada URL de link deve ser única.
   - **Texto do link** (máximo de 60 caracteres). Cada texto do link deve ser único.
5. Clique em **Mostrar visualização** (canto superior direito) para revisar o conteúdo da caixa de diálogo dos termos de serviço personalizados. Faça ajustes no conteúdo dos termos de serviço personalizados, se necessário.
6. Depois de concluir o conteúdo dos Termos de Serviço personalizados, clique em **Avançar**.
7. Revise os Termos de Serviço personalizados, confirme suas configurações e conteúdo, e depois clique em **Publicar**.
   A aplicação é imediata para o gatilho selecionado.

## Editando Termos de Serviço personalizados

1. Abra **Configurações** > **Enterprise Guard** > **Termos de Serviço Personalizados**.
2. Na lista, selecione a configuração de termos de serviço personalizados que deseja atualizar, então clique em **Editar**.
3. Atualize os campos conforme necessário em **Condições** e **Conteúdo**.
4. Se quiser atualizar os termos de serviço personalizados e redefinir imediatamente todas as aceitações dos usuários, clique em **Publicar imediatamente.**
   Se quiser atualizar os termos de serviço personalizados e solicitar aos usuários novamente após o término do período de recorrência configurado, clique na seta para baixo, selecione **Publicar no próximo ciclo** e então clique em **Publicar no próximo ciclo**.

## Excluindo Termos de Serviço personalizados

A exclusão desabilita os Termos de Serviço personalizados imediatamente e não pode ser desfeita.

1. Abra **Configurações** > **Enterprise Guard** > **Termos de Serviço personalizados**.
2. Na lista, selecione a configuração dos Termos de Serviço personalizados que deseja remover e clique em **Excluir**.
3. Para excluir permanentemente os Termos de Serviço personalizados selecionados, clique em **Excluir termos**.
