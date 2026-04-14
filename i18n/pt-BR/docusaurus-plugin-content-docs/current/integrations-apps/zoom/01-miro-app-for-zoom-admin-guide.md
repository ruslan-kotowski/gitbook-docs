---
title: aplicativo da Miro para Zoom (guia de admin )
article_id: 360022039379
translation_id: 360022039379
locale: pt-br
sidebar_position: 1
created_at: '2021-05-28T04:43:09Z'
updated_at: '2025-02-26T11:51:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: zoom
---

O aplicativo da Miro para Zoom permite que times criem uma sala de reunião digital completa e colaborem efetivamente durante reuniões e workshops usando o Miro dentro do Zoom. O aplicativo fornece os funcionalidades de colaboração do Miro dentro do Zoom e torna a integração de usuários convidado especialmente fácil. Para iniciantes no Miro , oferecemos quadro branco com acesso sem necessidade de registro.

Este guia pode ser usado por admins do Zoom e do Miro para habilitar a experiência para seus usuários.

:::note
Confira o [Guia do usuário do aplicativo da Miro para Zoom](02-miro-app-for-zoom-user-guide.md).
:::

> **Disponível para:** todos os planos Miro , todos os planos do Zoom
> *Para os planos Zoom Business e Enterprise , o admin pode precisar pré-aprovar o aplicativo da Miro
> **Disponível em**: versão desktop

## Como habilitar a experiência do aplicativo no Zoom

### Habilitar descoberta de aplicativos

1. Entre no portal da web do Zoom como admin com o privilégio de editar as configurações da conta.
2. No painel de navegação, clique em **Gerenciamento de conta** e depois **em Configurações da conta**.
3. Clique na aba**Aplicativos do Zoom** .
4. Verifique se **o botão de inicialização rápida do Zoom Apps** está habilitado. Isso permite que os usuários da sua conta vejam o botão Zoom Apps ![mceclip0.png](../../../../../../docs/integrations-apps/zoom/images/21017682787474_mceclip0.png) no cliente de desktop.
5. Se a configuração estiver desabilitada, clique no botão para habilitá-la. Se uma caixa de diálogo de verificação for exibida, clique em **Ligue** para verificar a alteração.

Além disso, o Zoom tem documentação adicional sobre como habilitar aplicativos do Zoom apenas para grupos ou usuários específicos. Para mais informações, visite o Central de ajuda do Zoom [aqui](https://support.zoom.us/hc/articles/360061555152).

![Zoom_apps_início_rápido.jpg](../../../../../../docs/integrations-apps/zoom/images/21017682788114_Zoom%20apps%20quick%20launch.jpg)
*Habilitando o botão de inicialização rápida do Zoom Apps*

Isso habilitará os aplicativos do Zoom na barra superior do cliente principal do Zoom e na barra inferior dos clientes de reunião para usuários da sua conta.

### Como pré-aprovar o aplicativo no Zoom

Se você for um admin do Zoom para um plano Zoom Business ou Enterprise , talvez seja necessário pré-aprovar o aplicativo da Miro [aqui](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) para que os usuários tenham acesso a ele.

![pre-approve_Miro_app.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653155474_pre-approve%20Miro%20app.jpg)*Pré-aprovando o aplicativo da Miro*

### Selecionando usuários na conta que podem instalar o aplicativo

Além de pré-aprovar o aplicativo da Miro, você pode selecionar quais usuários ou grupos podem instalá-lo.

![permitir_que_os_usuários_instalem_o_aplicativo.jpg](../../../../../../docs/integrations-apps/zoom/images/21017682790418_allow%20users%20to%20install%20the%20app.jpg)
*Selecionando usuários e grupos que podem instalar o aplicativo da Miro*

Depois de aprovar o aplicativo da Miro e instalá-lo na conta da sua empresa, os usuários poderão acessar e instalar a partir do cliente Zoom.

Consulte [a documentação do Zoom](https://support.zoom.us/hc/articles/360061555152) para obter mais informações.

## Como habilitar a experiência do aplicativo no Miro

> **Configurado por:** Admins da empresa no plano Enterprise

Se você estiver no [plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) e tiver limitado a instalação apenas para aplicativos aprovados, certifique-se de incluir o aplicativo da Miro para Zoom na sua lista de aplicativos aprovados em **Configurações da empresa > Aplicativos > Gerenciar aplicativos**. Você pode fazer isso colando o clientID 3074457354625507111 na pesquisa e habilitando o aplicativo para instalação.

![aprovar_Zoom_no_plano_empresarial.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653161874_approve%20Zoom%20on%20Enterprise%20plan.jpg)
*Aplicativos aprovados nas configurações da empresa*

## Como os usuários podem instalar o aplicativo

Os usuários podem encontrar o aplicativo da Miro para Zoom no [Zoom Marketplace](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) ou no [Marketplace da Miro](https://miro.com/marketplace/zoom-app/).

O primeiro passo no processo de instalação é autorizar o aplicativo da Miro para Zoom.

![instalar_aplicativo_Miro_para_Zoom.jpg](../../../../../../docs/integrations-apps/zoom/images/21017317899410_install%20Miro%20app%20for%20Zoom.jpg)
*Permitir que Miro acesse sua conta Zoom*

Uma vez autorizado, o aplicativo redirecionará os usuários para o aplicativo Zoom para desktop e mostrará o aplicativo da Miro recém-instalado. **Observe que eles precisarão estar logados em suas contas do Zoom para adicionar o aplicativo**.

Os usuários do Miro precisarão fazer **login** para ver seus boards. Isso os redirecionará para o navegador do sistema, onde solicitaremos que eles façam login no Miro ou autorizem diretamente o aplicativo no Miro. Eles podem escolher instalar o aplicativo para qualquer time à qual tenham acesso.

![instalar_Zoom_para_uma_equipe_Miro.jpg](../../../../../../docs/integrations-apps/zoom/images/21017682793362_install%20Zoom%20for%20a%20Miro%20team.jpg)
*Instale o aplicativo para uma de suas times Miro*

Os usuários serão redirecionados de volta para o aplicativo Zoom para desktop, onde verão o painel do Miro , incluindo todas as suas times e boards existentes.

![Miro_dashboard_in_Zoom.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653159442_Miro%20dashboard%20in%20Zoom.jpg)*Os usuários poderão selecionar um board em seu painel e abri-lo no Zoom*

## Compreendendo as configurações de acesso ao compartilhamento do board

Os usuários podem definir as permissões apropriadas para compartilhar um board em uma reunião do Zoom. Eles podem escolher entre quatro opções: **Qualquer pessoa no Zoom pode editar/ comentar/ visualizar** ou **Privar** (o que significa que as configurações de compartilhamento serão as mesmas definidas no Miro ).

![board_embed_sharing_settings.jpg](../../../../../../docs/integrations-apps/zoom/images/21017682795154_board%20embed%20sharing%20settings.jpg)

*Configurando as configurações de acesso para sua board*

As opções de configuração de acesso seguirão os controles de acesso de toda a organização. Se você restringiu o compartilhamento de links públicos para incorporações de board no [plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), essa opção não estará disponível para os usuários. Para mais informações, leia o artigo Como permitir ou restringir a inserção de boards da Miro em aplicativos compatíveis[.](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)

![publi_editing_is_turned_off.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653160722_publi%20editing%20is%20turned%20off.jpg)
Edição pública desativada pelo Administrador da empresa

## Perguntas frequentes

1. *Quais dados o aplicativo da Miro para Zoom está acessando?*
   - O aplicativo da Miro para Zoom está solicitando informações do perfil do usuário para associar um board a um determinado usuário. Nosso aplicativo **não** acessa o conteúdo da reunião, como vídeo, áudio, bate-papo e/ou arquivos de reunião e, portanto, não aparece no Notificador de aplicativos ativos do Zoom.
2. *O aplicativo pode ser instalado em tablets ou dispositivos móveis?*
   - Não, o aplicativo da Miro para Zoom está disponível apenas para desktop.
3. *Em qual sistema operacional o Zoom Apps funciona?*
   - Mac OS e Windows.
4. *Qual versão do Zoom é necessária para usar os aplicativos Zoom?*
   Versão: 5.7.3.
