---
title: 'Guia de implantação do Enterprise Guard , parte 2: Implantar Segurança de
  Dados'
article_id: 17121026396690
translation_id: 17121026396690
locale: pt-br
sidebar_position: 2
created_at: '2024-02-19T09:32:48Z'
updated_at: '2025-11-25T15:41:10Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: api-security
availability:
  notes: 'times relevantes: Exemplos de times com as quais você pode precisar fazer
    parceria para implantar recursos de segurança de dados incluem proteção de dados,
    prevenção contra perda de dados, governança e risco, segurança de aplicativos,
    informações digitais e segurança e/ou ameaças internas.'
---

## Visão geral da segurança de dados

Encontre, classifique e proteja conteúdo confidencial usando os recursos de segurança de dados do Enterprise Guard.

- **Descoberta de dados:** Descubra dados confidenciais , como informações de identificação pessoal (PII), informações pessoais de saúde (PHI) e dados do setor de cartões de pagamento (PCI) em apenas alguns cliques.
- **Classificação automática** defina critérios para que a Miro classifique automaticamente seus boards com base no conteúdo confidencial encontrado.
- **Proteções inteligentes:** Aplique regras de segurança em tempo real e restrinja o que os usuários podem fazer com um board com base na classificação manual ou automatizada do board .
- **Buscador de conteúdo:** Obtenha uma visualizar unificada de todos os boards da Miro com conteúdo sensível e a classificação do board .

![Enterprise-Guard-Data-Security.png](images/21016941894290_Enterprise-Guard-Data-Security.png)*Encontre, classifique e proteja dados confidenciais*

## Visão geral da implantação

Essa abordagem de implantação prioriza a proteção de dados confidenciais encontrados por meio do descoberta de dados do Enterprise Guard, ao mesmo tempo em que minimiza a interrupção da atividade do usuário final.

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="390" scrolling="no" src="https://miro.com/app/live-embed/uXjVNrjv8h8=/?moveToViewport=-3966,-1331,10269,3273&amp;embedId=881755370090" width="690"></iframe> *Visão geral da implantação do Enterprise Guard*

#### Etapas de configuração

1. Auditar dados sensíveis
2. Configurar classificação
3. Publicar a classificação
4. Implantar Guardrails
5. Afrouxar as restrições gerais

#### Etapas de comunicação e habilitação do usuário final

1. Crie um plano de implementação
2. Anúncio inicial do Enterprise Guard
3. Anúncio de implementação de classificações
4. Resolva ocorrências desnecessárias de dados confidenciais
5. Anúncio de lançamento de Guardrails

## Auditar dados sensíveis

Conclua a auditoria descrita nesta seção o mais cedo possível na sua implantação do Enterprise Guard . Não tem nenhum impacto sobre os usuários finais, mas permitirá que você avalie o escopo e a gravidade das ocorrências de dados confidenciais na sua instância do Miro .

Use os resultados da auditoria para criar um plano de implementação que equilibre o gerenciamento de mudanças do usuário final com as políticas de segurança da sua organização.

### Ativar descoberta de dados

O primeiro passo na configuração da sua framework de classificação de dados é habilitar o descoberta de dados na sua conta da Miro. O Miro então verificará todos os seus boards em busca de dados confidenciais de acordo com a Região e/ou Políticas de Regulamentação de Privacidade (rótulos) habilitados.

[Como habilitar a descoberta de dados em seu ambiente Miro](../../canvas-25-admin-features/data-discovery/13-activate-privacy-related-data-discovery.md)

Pode levar até 24 horas para que conteúdo sensível seja detectado. Depois que o Miro identificar o conteúdo sensível que corresponde a esses rótulos de sensibilidade (por exemplo, GDPR, PCI), o Buscador de conteúdo poderá ser usado para revisar os resultados com mais detalhes.

### Auditoria com o Buscador de conteúdo

O Buscador de conteúdo oferece aos admins de conteúdo sensível uma maneira de revisar ocorrências de dados confidenciais descobertas pelo Miro Enterprise Guard, revelando onde as ocorrências ocorreram (nome do board ), quem é o autor ( titular do board ), por que a ocorrência foi sinalizada ( etiqueta) e qual é o conteúdo.

Use os filtros no Buscador de conteúdo, como “Classificação = Confidencial”, para focar nas ocorrências mais importantes de dados confidenciais.

## Crie um plano de implementação

Depois que a descoberta de dados estiver habilitada e as ocorrências de conteúdo confidencial forem reveladas, é hora de criar um plano de implementação para Classificações e Guardrails de acordo com as políticas da sua organização, os requisitos, a gravidade das descobertas e os recursos disponíveis. As seções abaixo oferecem sugestões de práticas recomendadas de comunicação para informar os usuários finais e dar suporte ao seu processo de gerenciamento de mudanças.

### Anuncie as próximas mudanças

Antes de publicar sua framework de classificação no Miro, é recomendável informar os usuários sobre a decisão da sua organização de habilitar o Enterprise Guard em todo o conteúdo do Miro e fornecer contexto de acordo com as políticas e práticas de segurança de dados da sua organização.

Considere incluir as seguintes informações:

- O que é Enterprise Guard
- Por que é importante para sua organização
- Visão geral de quais aspectos da experiência do usuário final serão afetados
- Explicação da framework de classificação da sua organização
- Quais políticas de regulamentação de dados serão incluídas na descoberta de dados
- Cronograma das próximas mudanças
- Onde ir com perguntas e feedback

## Configurar classificação

### Adicionar estrutura de classificações

O estabelecimento de classificações de dados no Miro foi projetado para ser flexível e adaptável a qualquer frameworks de classificação de dados existente em sua organização.

Os níveis de classificação no Miro exibirão sua ordem de sensibilidade atual. Associe a ordem de sensibilidade à hierarquia de classificação da sua organização, onde a ordem de sensibilidade 1 é o nível de classificação menos sensível.

[Como configurar classificações](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md)

### Estruturas de classificação de achatamento

A estrutura de classificação do Miro Enterprise Guard foi projetada para se adaptar à sua política de classificação de dados existente.

Se a framework de classificação existente da sua organização tiver mais de uma camada de hierarquia (como níveis de subclassificação ou tags), pode ser necessário nivelar sua framework de classificação. O exemplo abaixo descreve uma framework de classificação com 3 tags que precisariam de 3 níveis de classificação separados por tag por nível.

É recomendável manter os níveis de classificação no mínimo.

![Enterprise-Guard-Flatten-Classification-Hierarchy.png](images/21016928922258_Enterprise-Guard-Flatten-Classification-Hierarchy.png)
*frameworks de classificação de achatamento*

### Vincular documentação e escrever descrições

Descrições e diretrizes claras de classificação informarão seus usuários finais sobre a política de classificação em escala. Enquanto os usuários finais estiverem no board, as descrições de classificação aparecerão ao lado do etiqueta de classificação. Os usuários finais verão um ponto de interrogação "saiba mais" em cada painel que leva à documentação de classificação.

|  |  |
| --- | --- |
| **Descrição da classificação** | Quando os usuários clicam no emblema de classificação do board , a descrição do nível de classificação atual é exibida.  Adicione uma descrição significativa que informe seus usuários sobre a sensibilidade deste board e as precauções ou ações recomendadas.  Classificação-descrição.png |
| **Link para as diretrizes** | Quando o usuário clica no ícone saiba mais (ícone de ponto de interrogação) ao lado do emblema de classificação do board , esta URL é carregada em uma nova aba do navegador.  Forneça aos seus usuários mais informações sobre os níveis de classificação do seu board e como trabalhar com eles.  Considere incluir:   - O que é Enterprise Guard - Por que é importante para sua organização - Visão geral de quais aspectos da experiência do usuário final serão afetados - Explicação da framework de classificação da sua organização - Quais políticas de regulamentação de dados serão incluídas na descoberta de dados - Onde ir com perguntas e feedback |

### Definir critérios de autoclassificação

O Miro aplicará classificações automaticamente aos boards onde for detectado conteúdo que corresponda à regulamentação de privacidade correspondente. Cada nível de classificação pode ser vinculado a vários[rótulos de sensibilidade](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md) , mas cada etiqueta de sensibilidade só pode ser vinculado a um único nível de classificação.

Se vários critérios forem atendidos, o nível de classificação mais sensível será aplicado.

[Como definir autoclassificações](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md)

### Configuração de pular guardrails

Conforme declarado anteriormente, este guia busca priorizar o gerenciamento de mudanças do usuário final, além de implantar o Enterprise Guard. Recomendamos publicar classificações sem barreiras. As classificações do board nesta configuração serão um indicador visual, mas não afetarão a experiência do usuário final.

Antes de adicionar barreiras às classificações, resolva ocorrências desnecessárias de dados confidenciais e integre os usuários à classificação manual para garantir uma transição suave sem interferir no trabalho crítico que acontece nos boards.

### Configurar Guardrails para Classificações Mais Elevadas

Usando as conclusões da sua auditoria inicial, você pode decidir implantar Guardrails sem demora. Considere aplicar Guardrails apenas às classificações mais sensíveis. Isso equilibra a urgência de proteger dados confidenciais sem afetar a grande maioria dos usuários finais.

## Publicar a classificação

Antes de publicar classificações automáticas, você terá a oportunidade de analisar seu impacto para seus usuários finais. Se você configurou os níveis de classificação sem Guardrails, não haverá impacto substancial para os usuários finais quando você publicar.

[Como publicar classificações](https://help.miro.com/hc/articles/16494764223378-Review-impact)

### Anúncio de classificação

Após publicar as classificações, envie um anúncio aos seus usuários finais.

Considere incluir as seguintes informações:

- Uma breve revisão do Enterprise Guard ou referência ao anúncio anterior
- Visão geral de quais aspectos da experiência do usuário final serão afetados
- Explicação da framework de classificação da sua organização
- Quais políticas de regulamentação de dados serão incluídas na descoberta de dados
- Cronograma das próximas mudanças
- Onde ir com perguntas e feedback

## Resolva ocorrências desnecessárias de dados confidenciais

Antes de lançar o Intelligent Guardrails, recomendamos comunicar-se com os titulares de board cujos boards contêm informações confidenciais. É possível que os dados confidenciais não sejam intencionais e possam ser removidos.

Informe aos usuários que os Intelligent Guardrails serão implementados em breve de acordo com as políticas de segurança da sua organização. Seus usuários finais podem aproveitar a oportunidade para remover dados confidenciais desnecessários de seus boards e evitar interrupções em seu trabalho.

## Usuários a bordo para classificação manual

Mesmo com a classificação automática ativada, muitos boards permanecerão sem classificação ou na classificação padrão se não forem reclassificados manualmente pelos usuários finais.

### Classificação manual Experiência do usuário final

O titular do board , [os cotitulares do board](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md), os editores que são membros da time e os Admins da empresa com [permissões de admins de conteúdo](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) podem atualizar o etiqueta de classificação clicando no emblema de classificação ou nos detalhes do board . Selecione um novo etiqueta e clique em atualizar.

Ao ajustar as classificações em níveis mais baixos na ordem de sensibilidade (por exemplo, de Confidencial para Público), os usuários precisarão fornecer uma justificativa que será registrada nos logs de auditoria da sua conta Miro .

### Comunicação com o usuário final

Após a implantação inicial do Enterprise Guard, é recomendável enviar comunicações regulares aos usuários finais que incentivem o uso de classificações em todos os board. Isso garantirá que o conjunto completo de proteções e classificações seja utilizado e, portanto, aumentará a segurança da sua instância do Miro .

Considere incluir as seguintes informações:

- Um lembrete para classificar os boards regularmente
- Instruções sobre como classificar boards
- Informações sobre como fornecer uma justificativa
- Vídeo | Classificação de board do usuário final (links para incorporar disponíveis abaixo)

<iframe allowfullscreen="" frameborder="0" height="315" src="//fast.wistia.com/embed/iframe/3ado2k4f6c" width="560"></iframe>
*Classificação do board em Miro*

### Recursos

- Vídeo | Classificações de board para usuários finais
  - [Link da Wistia](https://mirohq.wistia.com/medias/3ado2k4f6c)
  - Inserir código
    - ```
      <script src="https://fast.wistia.com/embed/medias/3ado2k4f6c.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;posição:relativa;"><div class="wistia_responsive_wrapper" style="altura:100%;esquerda:0;posição:absoluta;topo:0;largura:100%;"><div class="wistia_embed wistia_async_3ado2k4f6c seo=false videoFoam=true" style="altura:100%;posição:relativa;largura:100%"><div class="wistia_swatch" estilo="altura:100%;esquerda:0;opacidade:0;overflow:oculto;posição:absoluto;topo:0;transição:opacidade 200 ms;largura:100%;"><img src="https://fast.wistia.com/embed/medias/3ado2k4f6c/swatch" estilo="filtro:desfoque(5px);altura:100%;objeto-ajuste:contém;largura:100%;" alt="" aria-oculto="verdadeiro" onload="this.parentNode.style.opacity=1;" /></div></div></div></div></div>
      ```

## Implantar os Guardrails Restantes

Neste ponto, os usuários finais deveriam ter tido tempo suficiente para verificar se havia dados confidenciais desnecessários em seus boards e ajustar manualmente suas classificações de board .

[Como implantar Guardrails Inteligentes](../../canvas-25-admin-features/data-classification/05-define-guardrails.md)

> ⚠️ Tenha cuidado ao aplicar guardrails à classificação padrão do board . A aplicação de proteções à classificação padrão terá um impacto significativo nos usuários finais porque muitas boards terão a classificação padrão.

### Anúncio de Guardrails

Após publicar os Guardrails, envie um anúncio aos seus usuários finais.

Considere incluir as seguintes informações:

- Uma referência a anúncios anteriores sobre o Enterprise Guard
- O que são Guardrails
- Uma visão geral das classificações e seus guardrails associados
- Como ajustar classificações manualmente
- Onde ir com perguntas e feedback

## Afrouxe as restrições gerais de colaboração

O Enterprise Guard permite que você implante controles direcionados. Antes do Enterprise Guard, no entanto, não havia tantas opções para adaptar os controles a casos específicos. O resultado provavelmente foram “controles gerais” — configurações preventivamente rígidas que se aplicam à maioria dos boards , portanto, adicionam atrito à colaboração dos seus usuários do Miro .

Aplicar controles gerais, como bloquear a colaboração externa para todos os usuários e boards, carece de precisão. Os usuários podem enfrentar atritos quando o conteúdo em que estão colaborando não é sensível e isso pode bloquear casos de uso inteiros do Miro.

No geral, os controles gerais podem impactar o ROI que você obtém do Miro, mas agora com o Enterprise Guard, seus usuários finais podem obter mais valor do Miro , garantindo ao mesmo tempo que o conteúdo confidencial esteja protegido. Você precisará reavaliar algumas configurações em sua conta para aproveitar ao máximo o Enterprise Guard.

*<iframe allowfullscreen="" frameborder="0" height="315" src="//fast.wistia.com/embed/iframe/pukpdy1ji9" width="560"></iframe>*
Afrouxando as restrições da board

### Outras configurações vs Enterprise Guard

No Miro, há 3 áreas de configurações que trabalham juntas para determinar a experiência real do usuário.

- Configurações de nível de empresa
- Configurações em nível de equipe
- Enterprise Guard

Sempre que houver configurações concorrentes, a configuração mais rigorosa será implementada. Clique aqui para mais informações.

### Configurações relevantes e onde encontrá-las

Você precisará reavaliar algumas configurações para garantir que o Miro esteja configurado de forma holística. Aqui está uma lista de configurações relevantes e onde encontrá-las na sua conta da Miro. Algumas configurações podem ser controladas tanto no nível da empresa quanto no nível da time .

Lembre-se, se duas configurações se aplicam à mesma parte da experiência do Miro , a configuração mais rigorosa determinará a experiência.

|  |  |  |
| --- | --- | --- |
| **Como configurar** | **Descrição** | **Onde está disponível** |
| Links públicos | Um link público concede acesso a um board sem precisar fazer login. Ele pode ser configurado para visualizar, comentar ou editar acesso e exigir uma senha. | Nível da empresa  Nível do time  Enterprise Guard |
| Incorporação | Controla se e como os usuários podem incorporar boards da Miro em outros softwares ou sites. | Nível da empresa |
| Configurações do Convidado | Um Convidado é um usuário que é convidado apenas para um único board e não para uma time ou conta inteira. | Nível da empresa  Nível do time |
| Compartilhamento de board | Controla como os boards podem ser compartilhados com outros usuários na conta, dentro e entre times. | Nível do time  Enterprise Guard |
