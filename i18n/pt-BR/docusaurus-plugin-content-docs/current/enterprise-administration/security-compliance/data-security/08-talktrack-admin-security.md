---
title: "Seguran\xE7a do Admin do Talktrack"
article_id: 11148211487378
translation_id: 11148211487378
locale: pt-br
sidebar_position: 8
created_at: '2023-04-24T08:12:36Z'
updated_at: '2025-11-25T16:22:19Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

O Talktrack permite que usuários individuais gravem vídeos ou áudios interativos de seus boards no Miro para que possam compartilhar suas ideias sem gastar tempo extra em reuniões. Aprenda como a Miro garante segurança e conformidade de nível Enterprise para o Talktrack.

> ***Atualizações da interface da Miro em implantação gradual***
> A Miro está aprimorando a interface de usuário do board para ser mais inclusiva e intuitiva, e introduzindo uma evolução dos Projetos chamada Espaços. A implementação ocorrerá gradualmente para todas as contas da Miro ao longo de várias semanas.
>
> Caso já tenha o layout aprimorado de IU e Espaços, este artigo pode descrever pontos de entrada que foram alterados.
>
> Para ver a documentação mais atual, veja a [nova interface de usuário simplificada da Miro](../../../using-miro/working-on-the-board/02-miro's-new-simplified-user-interface.md).
>
> Este artigo será atualizado quando a implementação for concluída.

:::note
Conceda acesso ao [Talktrack](../../../using-miro/facilitation-tools/asynchronous-tools/02-talktrack-board-recordings.md) para sua organização nas configurações de [Acesso às funcionalidades](../../managing-enterprise-teams-and-content/06-feature-activation.md).
:::

:::note
Você pode aprender sobre os detalhes de privacidade e segurança do Talktrack no [whitepaper sobre o Talktrack para Enterprises](https://go2.miro.com/rs/228-GPV-835/images/Talktrack_WhitePaper.pdf) da Miro.
:::

## Segurança de nível empresarial

A Miro é o espaço de trabalho online para as empresas inovarem, que capacita times em qualquer localidade e tamanho a sonhar, projetar e construir o futuro juntos. Seus times podem usar a Miro para todos os casos de uso da empresa, seja no trabalho presencial, remoto ou híbrido.

Mas com isso vem uma grande responsabilidade, por isso levamos a segurança tão a sério quanto a colaboração — para ajudar a manter suas ideias seguras.

|  |  |  |
| --- | --- | --- |
| **Checkmark.png**  **Aprovada e certificada** | **Security_lock.png**  **Proteção confiável** | **Fingerprint.png**  **Gerenciamento de acesso seguro** |
| Melhores práticas do setor e requisitos regulatórios | Proteja e gerencie sua propriedade intelectual | Controle quem pode acessar e gerenciar seu conteúdo na Miro |

## Aprovado e certificado

A Miro segue as melhores práticas do setor e requisitos regulatórios, incluindo [ISO 27001, SOC2 Tipo II e SOC3](https://miro.com/trust/compliance/). Além disso, garantimos que sua infraestrutura e serviços estejam em conformidade com os padrões do GDPR — isso inclui as gravações do Talktrack.

**Gerenciamento do ciclo de vida do conteúdo**

**Exclusão de Talktrack**
**Excluindo um Talktrack:** Quando um Talktrack é excluído, ele não pode ser restaurado.

**Excluindo um board:** Os Talktracks são gravações sobrepostas que fornecem contexto a um board. Se um board for excluído, seus Talktracks também serão excluídos. No entanto, se um admin restaurar um board excluído dentro de 90 dias, os Talktracks do board também serão restaurados. Leia mais sobre [exclusão de boards](../../../using-miro/managing-boards/07-how-to-delete-a-board.md).

**Privacidade**

**Dados capturados ao gravar um Talktrack:** Movimentos do cursor do gravador e o campo de visão do board da Miro, o conteúdo do board no momento em que o Talktrack é criado, o vídeo do gravador, seja a vista da câmera ou avatar, dependendo se a câmera está ligada ou desligada, o áudio do gravador da fonte de áudio selecionada, e qualquer outro áudio presente no mesmo espaço físico que o apresentador.

**Dados não capturados ao gravar um Talktrack:** O cursor ou informações de quaisquer outros usuários que estejam acessando o board no momento da gravação, a tela do gravador ou sons do computador.

**Aviso de privacidade**

A base legal para o processamento de dados pessoais relacionados ao Talktrack, onde a Miro é controladora (essencialmente metadados), é a execução de um contrato (usuários de autoatendimento) e/ou interesses legítimos (todos os usuários). O cliente é o controlador dos dados gravados com Talktrack. A base legal do cliente é para o cliente avaliar e provavelmente ser interesses legítimos.

**Acessibilidade**

O Talktrack fornece navegação por teclado e suporte para transcrição automática/legenda oculta.

**Observabilidade**

[Logs de auditoria](../../security-integrations/security-management/01-audit-logs.md) estão disponíveis para Talktrack nas configurações do admin. Temos integrações com os seguintes sistemas SIEM (Gerenciamento de Informações e Eventos de Segurança):
[Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md)
[IBM QRadar](../../security-integrations/security-information-and-event-management-siem/02-miro-connector-for-ibm-qradar.md)

**Auditoria externa**

A Miro utiliza as melhores empresas de consultoria externas para realizar auditorias anuais. Nossa atual certificação ISO 27001 é assinada pelo BSI (British Standard Institution) do Reino Unido e os relatórios SOC2 & SOC3 são da KirkpatrickPrice dos EUA. Leia mais sobre [conformidade na Miro](https://miro.com/trust/compliance/).

## Proteção confiável

Proteja e gerencie a propriedade intelectual criada ou adicionada à nossa plataforma. Seus dados são criptografados em trânsito com o protocolo TLS 1.3 e em repouso com AES 256.

**Criptografia**

Dados no Miro — incluindo dados do Talktrack — são, por padrão, criptografados em repouso com o algoritmo AES256 e em trânsito com o protocolo TLS1.3. Leia mais em nosso [Whitepaper de Criptografia Miro](https://go2.miro.com/rs/228-GPV-835/images/Encryption%20Whitepaper.pdf).

**Classificação de dados**

A [etiqueta de classificação de boards](../../canvas-25-admin-features/data-security/02-data-classification.md) não é visível ao assistir ou gravar um Talktrack.

**Gerenciamento de Chaves de Criptografia**

Se sua organização tiver o [gerenciamento de chaves de criptografia](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md) (EKM) configurado e implementado, os Admins podem solicitar que a Miro utilize a chave de criptografia de sua organização para o conteúdo do Talktrack.

**Residência de dados**

Por padrão, os dados do Talktrack são armazenados no mesmo local que os outros dados de conteúdo do cliente na Miro: nos servidores da AWS localizados na UE. A Miro oferece um nível mais elevado de controle e conformidade sobre os dados da sua empresa, garantindo que todo o conteúdo do cliente seja hospedado na Europa. Para clientes que solicitaram [Residência de Dados nos EUA](../../canvas-25-admin-features/data-security/09-us-data-center-residency.md), os dados do Talktrack são armazenados em nosso data center principal em Ohio e no data center de backup na Virgínia.

## Gerenciamento seguro de acesso

Controle quem pode acessar a Miro com funcionalidades de nível empresarial, contando com recursos de identidade e administração avançados. Leia mais sobre os recursos de segurança e conformidade do plano Enterprise [aqui](../../../administration/security-compliance).

**Controlando o acesso da sua organização ao Talktrack**

Os Admins da empresa podem conceder ou revogar o acesso ao Talktrack para toda a empresa ou para times específicos nas configurações de [Acesso a Funcionalidades](../../managing-enterprise-teams-and-content/06-feature-activation.md).

**Acesso para gravar um Talktrack**

A opção de [gravar um Talktrack](../../../using-miro/facilitation-tools/asynchronous-tools/02-talktrack-board-recordings.md) está disponível para usuários que têm acesso para comentar ou editar em um board, ou são titulares ou co-titulares de um board.

**Acesso para visualizar um Talktrack**

A reprodução do Talktrack está disponível para todos os usuários que têm [acesso ao board](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Perguntas frequentes

Um Admin da empresa pode ver quais boards têm um Talktrack?

Você só consegue ver se um board tem um Talktrack abrindo-o. Se o board não for compartilhado com você, pode usar as [permissões de admin de conteúdo](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) para obter acesso e ver o Talktrack.

Como posso desativar o Talktrack para minha empresa ou time?

Para desativar o Talktrack, vá às suas configurações de [acesso a funcionalidades](../../managing-enterprise-teams-and-content/06-feature-activation.md) e selecione **Ninguém pode usar**, ou remova o acesso para times específicos clicando em **X** ao lado do nome do time.

O que acontece com os Talktracks existentes quando um admin revoga o acesso à funcionalidade de Talktrack?

Os Talktracks existentes continuarão disponíveis, mas não será possível gravar novos Talktracks.

Os admins podem excluir Talktracks?

Os admins podem compartilhar um board consigo mesmos nas [permissões de admin de conteúdo](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) e, em seguida, excluir o Talktrack do board.

Os nomes dos usuários são exibidos no aplicativo e/ou salvos com os dados do Talktrack?

O Talktrack exibe o nome (primeiro e último nome ou nome de exibição, dependendo da disponibilidade) durante a reprodução e como "nome do gravador". No entanto, o Talktrack salva apenas IDs de usuários, portanto, nenhuma informação pessoal é salva com a gravação. Se o usuário não fizer parte da organização durante a reprodução, o nome de exibição aparecerá como "Usuário Desconhecido".
