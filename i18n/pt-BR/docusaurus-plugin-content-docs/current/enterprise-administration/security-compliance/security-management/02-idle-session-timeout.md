---
title: Tempo limite de sessão ociosa
article_id: 360017571454
translation_id: 360017571454
locale: pt-br
sidebar_position: 2
created_at: '2019-02-11T10:09:05Z'
updated_at: '2025-02-06T08:46:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponível para: plano Enterprise Função necessária: Admin da empresa'
---

O recurso de tempo de sessão ociosa permite que você defina um **limite** de tempo de inatividade para seus usuários finais. A configuração afeta todos os membros e [convidados](../../../using-miro/sharing-boards/07-collaboration-with-guests.md). Se a sessão do usuário atingir o limite e expirar, ele será desconectado automaticamente do perfil da Miro e precisará fazer logon novamente para poder acessar os dados do plano Enterprise.

:::warning
Tenha cuidado ao definir o tempo de sessão ociosa. Limites de tempo altamente seguros e de duração muito curta farão com que os usuários sejam continuamente desconectados de seus boards. Defina um limite de tempo de inatividade equilibrado e seguro e lembre-se de comunicar claramente os limites de tempo aos seus usuários.
:::

### Como ativar o tempo limite de sessão ociosa

1. Vá para Configurações **da empresa** > **Segurança** > **Autenticação** > **Tempo limite de sessão ociosa**
2. Ative **Desconectar usuários inativos automaticamente** e defina o **Período de inatividade.

   ![](../../../../../../../docs/enterprise-administration/security-compliance/security-management/images/23921804858002_idle-session-timeout.png)
*altidle-session-timeout.pngTempo de sessão ociosa ativado***

Ao ativar o recurso de tempo de sessão ociosa pela primeira vez, será aplicada a sessão padrão de um dia. O admin pode personalizar a duração e inserir um valor inteiro personalizado de 1 a 9999 e selecionar as unidades: minutos, horas ou dias. A duração mínima permitida é de 1 hora, e a duração máxima permitida é de 14 dias. Recomendamos que a duração não seja inferior a 8 horas.

Para o recurso Tempo de sessão ociosa, definimos inatividade como ausência das seguintes ações presentes em qualquer lugar do aplicativo durante o tempo definido:

- movimento do mouse (ou movimento da tela sensível ao toque)
- cliques do mouse (ou toques na tela sensível ao toque)
- uso do teclado

Antes do encerramento da sessão, os usuários receberão uma mensagem de aviso. Os usuários podem simplesmente mover o mouse ou pressionar qualquer tecla do teclado para permanecer conectados.

:::note
O valor padrão de tempo limite de sessão ociosa é 1 dia. As configurações podem variar de 1 hora a 14 dias.
:::

:::note
O Tempo de sessão ociosa funciona em qualquer lugar (acessando a atividade do usuário em diferentes dispositivos, integrações, etc.).
:::

:::note
Não serão afetados usuários visitantes de um board público salvo em um plano Enterprise e que não fazem parte do plano Enterprise que habilitou o tempo de sessão ociosa.
:::

:::note
Se o usuário pertencer a várias organizações que possuem diferentes intervalos de tempo limite de sessão ociosa, a duração mais curta prevalecerá. Por exemplo, o usuário pertence a uma organização com tempo de sessão ociosa de 6 horas e a outra organização com tempo de sessão ociosa de 30 minutos. Nesse caso, o tempo limite de todas as sessões ativas será expirado em 30 minutos.
:::
