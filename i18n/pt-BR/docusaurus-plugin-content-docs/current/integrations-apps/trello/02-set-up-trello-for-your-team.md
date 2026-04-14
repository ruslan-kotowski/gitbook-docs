---
title: Configure o Trello para o seu time
article_id: 30634093325842
translation_id: 30634093325842
locale: pt-br
sidebar_position: 2
created_at: '2025-10-29T15:59:48Z'
updated_at: '2026-02-23T11:40:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

A integração com o Trello é implementada tecnicamente através de uma API REST. Para fins de autenticação e autorização, a integração utiliza o protocolo OAuth 2.0, que é o padrão da indústria. Um componente chave dessa arquitetura é a utilização de uma plataforma API unificada como subprocessador de dados de terceiros. Esta plataforma fornece APIs unificadas responsáveis por autenticar, normalizar e sincronizar dados entre vários provedores de API.

## Fluxos de dados

Uma compreensão completa do fluxo de dados é essencial para gerenciar a segurança e conformidade dentro da sua organização.

### Diagrama de sequência em alto nível

Criando um widget de cartão do Trello

![Trello (BETA) 2.jpg](images/30634984622738_Trello%20(BETA) 2.jpg)

Atualizando um widget de cartão do Trello

![Trello (BETA) 2.jpg](images/30634984622738_Trello%20(BETA) 2.jpg)

### Dados do Trello na Miro

Quando os usuários importam cartões do Trello para um board da Miro, os dados relevantes do cartão tornam-se parte integrante dos dados do canvas da Miro. A Miro armazena os seguintes pontos de dados específicos para cartões importados, desde que estejam disponíveis no Trello:

- Título
- Descrição
- Membros (incluindo nomes de usuários e e-mails)
- Lista
- Etiquetas

A enumeração explícita dos tipos de dados armazenados é crucial para a governança de dados organizacional e conformidade. Ela permite que os administradores avaliem com precisão quais informações, particularmente quaisquer dados confidenciais, estão sendo replicadas no ambiente da Miro. Essa transparência garante alinhamento com as políticas internas de manuseio de dados da organização. Também é importante notar que, conforme a seção "Limitações", campos personalizados não são suportados e, portanto, não são armazenados, o que é um detalhe chave para avaliações de mapeamento de dados e conformidade. A Miro adota uma abordagem híbrida para armazenamento de dados, minimizando os dados armazenados diretamente no widget de cartão e buscando detalhes adicionais quando o usuário abre a visualização de edição.

### Retenção de dados das informações armazenadas na Miro

Todos os dados importados do Trello que são armazenados na Miro aderem estritamente à política padrão de retenção de dados da Miro. Esta política é aplicada de forma consistente a todos os dados de clientes, garantindo uma abordagem uniforme para o gerenciamento do ciclo de vida dos dados.

## Autenticação e autorização

A integração do Trello inicia um fluxo de autenticação quando um usuário interage pela primeira vez com a integração. A autorização dentro do Trello é gerida pelo serviço de integração. Para cada usuário individual, a Miro estabelece uma conta com o serviço de integração, e essas credenciais são posteriormente usadas para todas as interações do usuário com a integração.

A integração normalmente requer a aprovação de um admin do Trello para autorizar o aplicativo de integração dentro do ecossistema da organização. Além disso, os usuários individuais também devem autorizar a integração Miro Trello por meio da página de autorização do OAuth do Trello quando tentam, pela primeira vez, inserir um link do Trello.

### Escopos de autorização necessários

O escopo de autorização pode variar dependendo do sistema de terceiros específico. No entanto, para integrações de gestão de cartões como o Trello, a Miro geralmente requer acesso aos seguintes dados:

| Escopo | Descrição |
| --- | --- |
| Cartões (leitura e escrita) | Concede à integração permissão para ler cartões (tickets) existentes e criar ou modificar cartões dentro do Trello. |
| Usuários (leitura) | Concede à integração permissão para ler informações de usuários dentro do Trello, geralmente para atribuir cartões ou exibir nomes de membros. |
| Coleções (leitura) | Concede à integração permissão para ler coleções, boards e listas dentro do Trello. |

### O que é armazenado na Miro e como

A Miro armazena com segurança tanto dados relacionados à autorização quanto dados relacionados ao unfurling para a integração com o Trello:

- **Dados relacionados à autorização:** Isso inclui tokens de acesso e valores de tokens de atualização, que são armazenados no banco de dados da Miro por um período limitado de alguns dias. Esses tokens são automaticamente atualizados após a expiração utilizando o token de atualização para garantir acesso contínuo. Todos esses dados armazenados no banco de dados para essa integração são criptografados com o padrão de criptografia avançada de 256 bits, fornecendo uma camada robusta de segurança de dados.
- **Dados relacionados à expansão:** Isso inclui títulos de cartões, que são armazenados como parte dos boards da Miro. Além disso, títulos e referências criptografadas a esses elementos são armazenados em um serviço interno, seguros por meio de criptografia (EKM).

### Revogação de um token

Se necessário, admins ou usuários individuais podem revogar os tokens concedidos à integração com o Trello. Os usuários podem acessar as configurações de integração abrindo um seletor de cartões de integrações, clicando no menu de três pontos no canto superior direito e selecionando **Configurações de Integração**, ou acessando a guia **Aplicativos** nas configurações do time na Miro, localizando a integração específica e clicando nela. Na página de configurações, a autorização pode ser revogada clicando no botão **Desconectar**. Com esta ação, a Miro revogará o acesso ao Trello e excluirá a conta do usuário associado. Para desinstalação no nível do time, os admins podem seguir as etapas específicas descritas na seção "Solução de Problemas e FAQ (Admin)".

## Como configurar a integração com o Trello

O processo de configuração para a integração Miro + Trello envolve etapas distintas tanto para admins quanto para usuários finais, garantindo uma implantação controlada dentro de uma organização.

1. **Assegurar contas ativas:** Antes de iniciar a instalação, certifique-se de que ambas as contas ativas da Miro e do Trello estão disponíveis.
2. **Instalação no nível do time (Ação do Admin):**
   - Os admins podem precisar autorizar explicitamente a integração com o Trello para seu time no Miro. Os membros do time só poderão utilizar a integração se ela tiver sido instalada no nível do time.
   - Um admin do time no Miro pode instalar diretamente o aplicativo abrindo um board do Miro, selecionando **Ferramentas, Mídias e Integrações (+)**, pesquisando por "Trello" e clicando em **Conectar** para autorizar a integração. Se um admin do time no Miro realizar essa ação, o aplicativo será automaticamente autorizado e instalado sem necessitar de aprovação administrativa adicional.
3. **Fluxo de solicitação de usuário e aprovação de admin (se aplicável):**
   - Em organizações onde é necessário um consentimento administrativo rigoroso, um usuário não admin em um time da Miro configurado para a integração com o Trello pode colar um link do Trello em um board da Miro. Esta ação pode acionar um diálogo de "solicitação de instalação do aplicativo" para o usuário, solicitando que ele busque a aprovação administrativa.
   - Os admins designados podem então revisar e aprovar esta solicitação pendente através de seus consoles administrativos da Miro ou Trello, dependendo do fluxo de consentimento específico configurado.
4. **Conexão do usuário individual:**
   - Após a integração ter sido instalada e autorizada com sucesso no nível do time por um admin, os usuários individuais deverão clicar em **Conectar** no widget do Trello que aparece no board da Miro.
   - Os usuários serão então redirecionados para uma página de autorização do Trello onde eles concedem à Miro acesso à sua conta individual do Trello, confirmando assim sua autorização pessoal para incorporar e interagir com o conteúdo.

## Considerações de segurança e conformidade

### Restrição de acesso ao arquivo fonte

Para garantir que o acesso aos dados incorporados do Trello permaneça restrito aos mesmos indivíduos do board de origem do Trello, os admins da organização Miro devem manter controles rigorosos sobre o compartilhamento do board e a exportação de conteúdo. Embora a integração principal do Trello respeite permissões individuais para interação em tempo real, qualquer exportação ou captura estática do conteúdo do board pode potencialmente expor dados a pessoas não autorizadas se o board da Miro propriamente dito não for gerido com segurança.

### Tratamento de erros

A integração é projetada com uma interface de usuário flexível e tratamento de erros para casos em que atualizações de dados do cartão falham devido à rejeição por terceiros.

### Adendo de Processamento de Dados da Miro (DPA)

Para obter detalhes legais e de conformidade abrangentes sobre as práticas de processamento de dados da Miro, os admins são orientados a consultar o [Addendum de Processamento de Dados da Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Solução de problemas e FAQs

### Como você pode desativar a integração (desinstalação a nível de time)?

Um admin do time na Miro pode desinstalar a integração com o Trello a nível de time. Esta ação desabilita a integração para todos os membros do time. Para isso, acesse **Configurações do time Apps e Integrações**. Encontre "Trello" ou "Gerenciamento de Cartão do Trello" na lista de aplicativos instalados, role para baixo e clique em **Desinstalar para time**.

### Como você pode desativar a integração (desinstalação individual)?

Usuários individuais podem desinstalar a integração para si mesmos. Vá até **Apps e Integrações** nas suas configurações da Miro. Localize "Trello" ou "Gerenciamento de Cartões Trello" e clique em **Desinstalar para mim**.

### Quais administradores podem instalar a integração Trello para seu time?

Somente admins de time da Miro podem instalar o aplicativo diretamente. Se um admin de time da Miro colar uma URL do Trello em um board da Miro, o aplicativo será automaticamente autorizado e instalado sem necessidade de mais ações.

### Quais são os requisitos de disponibilidade para a integração Trello?

A integração Trello está disponível para os planos Business e Enterprise da Miro.

### Os administradores precisam autorizar a integração Trello para seu time?

Sim, os admins podem precisar autorizar a integração com o Trello para o time na Miro. Os membros do time só podem usar a integração com o Trello se ela tiver sido instalada em nível de time.
