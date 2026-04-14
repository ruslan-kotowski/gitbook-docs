---
title: "[GitHub] Ol\xE1, documentos-como-c\xF3digo!"
article_id: 29239655610258
translation_id: 29239655610258
locale: pt-br
sidebar_position: 2
created_at: '2025-09-04T17:11:12Z'
updated_at: '2026-01-23T15:01:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Esta seção fornece detalhes técnicos e administrativos abrangentes, essenciais para profissionais de TI e segurança responsáveis pela implantação, segurança e gestão contínua da integração com o Trello em suas organizações.

## Visão geral técnica

A integração com o Trello é implementada tecnicamente por meio de uma API REST. Para fins de autenticação e autorização, a integração utiliza o protocolo OAuth 2.0, padrão do setor. Um componente chave dessa arquitetura é a utilização de uma plataforma unificada de API como sub-processador de dados de terceiros. Esta plataforma fornece APIs unificadas responsáveis por autenticar, normalizar e sincronizar dados entre vários provedores de API.

## Fluxos de dados

Uma compreensão completa do fluxo de dados é essencial para gerenciar a segurança e conformidade dentro da sua organização.

### Diagrama de sequência de alto nível

Criando um widget de cartão do Trello

![image (7).png](images/32777076216338_image%20(7).png)

Atualizando um widget de cartão do Trello

![image (8).png](images/32777076218642_image%20(8).png)

### Dados do Trello na Miro

Quando os usuários importam cartões do Trello para um board da Miro, os dados relevantes do cartão tornam-se parte integrante dos dados do canvas da Miro. A Miro armazena os seguintes pontos de dados específicos para cartões importados, desde que estejam disponíveis no Trello:

- Título
- Descrição
- Membros (incluindo nomes de usuário e e-mails)
- Lista
- Etiquetas

A enumeração explícita dos tipos de dados armazenados é crucial para a governança de dados organizacional e conformidade. Isso permite que os administradores avaliem com precisão quais informações, em particular quaisquer dados possivelmente confidenciais, estão sendo replicadas no ambiente da Miro. Essa transparência garante alinhamento com as políticas internas de gerenciamento de dados da organização. Vale também ressaltar que, conforme a seção "Limitações", campos personalizados não são suportados e, portanto, não são armazenados, o que é um detalhe importante para o mapeamento de dados e avaliações de conformidade. A Miro emprega uma abordagem híbrida para armazenamento de dados, minimizando os dados armazenados diretamente no widget de cartão e buscando detalhes adicionais quando o usuário abre a visualização de edição.

### Retenção de dados das informações armazenadas na Miro

Todos os dados importados do Trello que são armazenados dentro da Miro aderem estritamente à política padrão de retenção de dados da Miro. Esta política é aplicada consistentemente a todos os dados de clientes, garantindo uma abordagem uniforme para o gerenciamento do ciclo de vida dos dados.

## Autenticação e autorização

A integração com o Trello inicia um fluxo de autenticação quando um usuário interage com a integração pela primeira vez. A autorização dentro do Trello é gerida pelo serviço de integração. Para cada usuário individual, a Miro estabelece uma conta com o serviço de integração, e essas credenciais são usadas subsequentemente para todas as interações do usuário com a integração.

Tipicamente, a integração requer aprovação de um admin do Trello para autorizar a aplicação de integração dentro do ecossistema da organização. Além disso, usuários individuais também devem autorizar a integração Miro Trello por meio da página de autorização OAuth do Trello ao tentarem incorporar um link do Trello pela primeira vez.

### Escopos de autorização necessários

O escopo de autorização pode variar dependendo do sistema de terceiros específico. No entanto, para integrações de gerenciamento de cartões como o Trello, a Miro geralmente requer acesso aos seguintes dados:

| Escopo | Descrição |
| --- | --- |
| Cartões (leitura e escrita) | Concede à integração permissão para ler cartões existentes e criar ou modificar cartões dentro do Trello. |
| Membros (leitura) | Concede à integração permissão para ler informações de membros no Trello, normalmente para atribuir cartões ou exibir nomes de membros. |
| Etiquetas (leitura) | Concede à integração permissão para ler etiquetas associadas a cartões no Trello. |
| Boards (leitura) | Concede à integração permissão para ler informações de boards e listas dentro do Trello. |

### O que é armazenado na Miro e como

A Miro armazena com segurança dados relacionados à autorização e ao unfurling para a integração com o Trello:

- **Dados relacionados à autorização:** Isso inclui tokens de acesso e valores de tokens de atualização, que são armazenados no banco de dados da Miro por um período limitado de vários dias. Esses tokens são automaticamente atualizados ao expirarem, utilizando o token de atualização para garantir acesso contínuo. Todos esses dados armazenados no banco de dados para essa integração são criptografados usando o Padrão de Criptografia Avançada de 256 bits, proporcionando uma camada robusta de segurança de dados.
- **Dados relacionados ao desvelamento:** Isso inclui títulos de cartões, que são armazenados como parte dos próprios boards da Miro. Além disso, títulos e referências criptografadas a esses elementos são armazenados em um serviço interno, ainda mais protegido por meio de criptografia (EKM).

### Revogação de um token

Se necessário, administradores ou usuários individuais podem revogar os tokens concedidos à integração do Trello. Os usuários podem navegar para as configurações da integração abrindo um seletor de cartões de integrações, clicando no menu de três pontos no canto superior direito e selecionando **Configurações de Integração**, ou acessando a guia **Apps** nas configurações de time da Miro, encontrando a integração específica e clicando nela. Na página de configurações, a autorização pode ser revogada clicando no botão **Desconectar**. Após essa ação, a Miro revogará o acesso ao Trello e excluirá a conta associada do usuário. Para desinstalação no nível do time, os administradores podem seguir passos específicos detalhados na seção "Soluções de Problemas & FAQs (Admin)".

## Como configurar a integração com o Trello

O processo de configuração da integração Miro + Trello envolve etapas distintas tanto para admins quanto para usuários finais, garantindo uma implantação controlada dentro de uma organização.

1. **Garanta contas ativas:** Antes de iniciar a instalação, certifique-se de que ambas as contas ativas do Miro e do Trello estejam disponíveis.
2. **Instalação no nível do time (Ação do Admin):**
   - Os admins podem precisar autorizar explicitamente a integração do Trello para seu time no Miro. Os membros do time só poderão utilizar a integração se ela for instalada no nível do time.
   - Um admin do time no Miro pode instalar diretamente o aplicativo abrindo um board do Miro, selecionando **Mídia & Integrações (+)**, procurando por "Trello" e clicando em **Conectar** para autorizar a integração. Se um admin do time do Miro realizar essa ação, o aplicativo será automaticamente autorizado e instalado, sem necessidade de aprovação administrativa adicional.
3. **Fluxo de solicitação de usuário e aprovação do admin (se aplicável):**
   - Em organizações onde é necessário consentimento administrativo rigoroso, um usuário não-admin em um time da Miro configurado para integração com o Trello pode colar um link do Trello em um board da Miro. Esta ação pode acionar um diálogo de "solicitação de instalação do aplicativo" para o usuário, solicitando que ele busque aprovação administrativa.
   - Os admins designados podem então analisar e aprovar esta solicitação pendente através de seus consoles administrativos da Miro ou do Trello, dependendo do fluxo de consentimento específico configurado.
4. **Conexão de usuário individual:**
   - Após a integração ter sido instalada e autorizada com sucesso no nível do time por um admin, os usuários individuais deverão clicar em **Conectar** no widget do Trello que aparece no board da Miro.
   - Em seguida, os usuários serão redirecionados para uma página de autorização do Trello, onde concederão à Miro acesso à sua conta individual do Trello, confirmando assim sua autorização pessoal para inserir e interagir com o conteúdo.

## Considerações de segurança e conformidade

### Restrição de acesso ao arquivo fonte

Para garantir que o acesso aos dados do Trello incorporados permaneça restrito aos mesmos indivíduos do board fonte do Trello, os admins de organização do Miro devem manter controles rigorosos sobre o compartilhamento do board e a exportação de conteúdo. Embora a integração principal do Trello respeite permissões individuais para interação ao vivo, qualquer exportação ou captura estática de conteúdo do board pode potencialmente expor dados a indivíduos não autorizados se o board do Miro não for gerenciado adequadamente.

### Tratamento de erros

A integração é projetada com uma interface amigável para quedas e tratamento de erros nos casos em que as atualizações de dados do cartão falham devido à rejeição de terceiros.

### Adendo de Processamento de Dados da Miro (DPA)

Para obter detalhes legais e de conformidade abrangentes sobre as práticas de processamento de dados da Miro, os admins devem consultar o [Anexo de Processamento de Dados da Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Solução de problemas e FAQs

### Como desabilitar a integração (desinstalação a nível de time)?

Um admin do time Miro pode desinstalar a integração com o Trello a nível de time. Esta ação desabilita a integração para todos os membros do time. Para isso, vá para **Configurações do time Apps e integrações**. Encontre "Trello" ou "Gerenciamento de Cartões Trello" na lista de aplicativos instalados, role para baixo e clique em **Desinstalar para o time**.

### Como desabilitar a integração (desinstalação individual)?

Usuários individuais podem desinstalar a integração por conta própria. Navegue até **Apps e Integrações** nas suas configurações da Miro. Localize "Trello" ou "Gerenciamento de Cartões Trello" e clique em **Desinstalar para mim**.

### Quais administradores podem instalar a integração Trello para o seu time?

Apenas admin da Miro pode instalar diretamente o aplicativo. Se um admin do time da Miro colar uma URL do Trello em um board da Miro, o aplicativo será automaticamente autorizado e instalado sem necessidade de mais ações.

### Quais são os requisitos de disponibilidade para a integração Trello?

A integração Trello está disponível para os planos Business e Enterprise da Miro. REST API

### Os administradores precisam autorizar a integração Trello para seu time?

Sim, os administradores podem precisar autorizar a integração do Trello para o time na Miro. Os membros do time só podem usar a integração do Trello se ela tiver sido instalada no nível do time.
