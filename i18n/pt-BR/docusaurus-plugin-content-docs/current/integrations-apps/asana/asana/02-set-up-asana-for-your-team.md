---
title: Configurar o Asana para seu time
article_id: 28252196453778
translation_id: 28252196453778
locale: pt-br
sidebar_position: 2
created_at: '2025-07-22T13:30:20Z'
updated_at: '2026-02-20T09:00:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Esta seção fornece detalhes técnicos e administrativos abrangentes, essenciais para profissionais de TI e segurança responsáveis pela implantação, segurança e gestão contínua da integração do Asana dentro da sua organização.

## Visão geral técnica

A integração do Asana é tecnicamente implementada através de uma API REST. Para fins de autenticação e autorização, a integração utiliza o protocolo padrão da indústria OAuth 2.0. Um componente chave desta arquitetura é a utilização de uma plataforma de API unificada como sub-processador para dados de terceiros. Esta plataforma fornece APIs unificadas que são responsáveis por autenticar, normalizar e sincronizar dados através de vários provedores de API.

## Fluxos de dados

Uma compreensão completa do fluxo de dados é fundamental para gerenciar a segurança e a conformidade dentro da sua organização.

### Diagrama de sequência em alto nível

Criando um widget de cartão Asana

![image (7).png](images/30597084526482_image%20(7).png)

Atualizando um widget de cartão Asana

![image (8).png](images/30597105661202_image%20(8).png)

### Dados do Asana na Miro

Quando os usuários importam tarefas do Asana para um board da Miro, os dados relevantes da tarefa tornam-se parte integrante dos dados do canvas da Miro. A Miro armazena os seguintes pontos de dados específicos para as tarefas importadas, desde que estejam disponíveis no Asana:

- Título
- Descrição
- Atribuído a (incluindo o nome e/ou endereço de e-mail do usuário)
- Status
- Prioridade

A enumeração explícita dos tipos de dados armazenados é crucial para a governança de dados organizacional e conformidade. Isso permite que os admins avaliem com precisão quais informações, especialmente quaisquer dados potencialmente confidenciais, estão sendo replicadas no ambiente Miro. Essa transparência garante o alinhamento com as políticas internas de manuseio de dados da organização. Também é importante notar que, conforme a seção "Limitações", campos personalizados não são suportados e, portanto, não são armazenados, o que é um detalhe fundamental para o mapeamento de dados e avaliações de conformidade. A Miro adota uma abordagem híbrida para armazenamento de dados, minimizando os dados armazenados diretamente no widget de cartão e buscando detalhes adicionais quando o usuário abre a visualização de edição.

### Retenção de dados das informações armazenadas na Miro

Todos os dados importados do Asana que são armazenados na Miro seguem estritamente a política de retenção de dados padrão da Miro. Esta política é aplicada de forma consistente em todos os dados dos clientes, garantindo uma abordagem uniforme para o gerenciamento do ciclo de vida dos dados.

## Autenticação e autorização

A integração com o Asana inicia um fluxo de autenticação quando um usuário interage pela primeira vez com a integração. A autorização dentro do Asana é gerenciada pelo serviço de integração. Para cada usuário individual, a Miro estabelece uma conta com o serviço de integração, e essas credenciais são subsequentemente usadas para todas as interações do usuário com a integração.

A integração normalmente requer a aprovação de um admin de Asana (ou de um admin do Microsoft Entra, se o Asana for gerenciado via Azure AD) para autorizar o aplicativo de integração dentro do ecossistema da organização. Além disso, os usuários individuais também devem autorizar a integração Miro Asana através da página de autorização OAuth do Asana na primeira tentativa de incorporar um link do Asana.

### Escopos de autorização necessários

O escopo de autorização pode variar dependendo do sistema de terceiros específico. No entanto, para integrações de ticket como o Asana, a Miro geralmente requer acesso aos seguintes dados:

| Escopo | Descrição |
| --- | --- |
| Tickets (leitura e edição) | Concede à integração permissão para ler tarefas existentes e criar ou modificar tarefas dentro do Asana. |
| Usuários (leitura) | Concede à integração permissão para ler informações de usuários no Asana, tipicamente para atribuir tarefas ou mostrar nomes de responsáveis. |
| Tags (leitura) | Concede à integração permissão para ler tags associadas às tarefas no Asana. |
| Coleções (leitura) | Concede à integração permissão para ler coleções de tarefas ou projetos no Asana. |

### O que é armazenado na Miro e como

A Miro armazena de forma segura dados relacionados à autorização e ao "unfurling" para a integração Asana:

- **Dados relacionados à autorização:** Isso abrange valores de tokens de acesso e de refresh, que são armazenados no banco de dados da Miro por um período limitado de vários dias. Esses tokens são automaticamente renovados ao expirar usando o refresh token para garantir acesso contínuo. Todos esses dados armazenados no banco de dados para essa integração são criptografados usando o Padrão de Criptografia Avançada de 256 bits, fornecendo uma robusta camada de segurança de dados.
- **Dados relacionados ao unfurling:** Isso inclui títulos de tarefas, que são armazenados como parte dos próprios boards da Miro. Além disso, títulos e referências criptografadas desses elementos são armazenados em um serviço interno, ainda mais seguro por meio de criptografia (EKM).

### Revogação de um token

Se necessário, admins ou usuários individuais podem revogar os tokens concedidos à integração com a Asana. Os usuários podem navegar até as configurações de integração abrindo um seletor de tarefas de integrações, clicando no menu de três pontos no canto superior direito e selecionando **Configurações de integração**, ou acessando a guia **Aplicativos** no menu de configurações do time do Miro, encontrando a integração específica e clicando nela. Na página de configurações, a autorização pode ser revogada clicando no botão **Desconectar**. Com essa ação, o Miro revogará o acesso à Asana e deletará a conta associada do usuário. Para desinstalar ao nível do time, os admins podem seguir etapas específicas descritas na seção "Resolução de Problemas & FAQs (Admin)".

## Como configurar a integração com a Asana

O processo de configuração da integração Miro + Asana envolve etapas distintas tanto para admins quanto para usuários, garantindo uma implantação controlada dentro da organização.

1. **Garantir contas ativas:** Antes de iniciar a instalação, certifique-se de que contas ativas de Miro e Asana estão disponíveis.
2. **Instalação ao nível do time (Ação do Admin):**
   - Os admins podem precisar autorizar explicitamente a integração Asana para o time Miro deles. Os membros do time só poderão utilizar a integração se ela tiver sido instalada ao nível do time.
   - Um admin do time Miro pode instalar o aplicativo diretamente ao abrir um board Miro, selecionar **Ferramentas Mídia & Integrações (+)**, procurar "Asana" e clicar em **Conectar** para autorizar a integração. Se um admin do time Miro realizar esta ação, o aplicativo será automaticamente autorizado e instalado sem necessidade de aprovação administrativa adicional.
3. **Fluxo de solicitação de usuário e aprovação do admin (se aplicável):**
   - Em organizações onde é exigida aprovação administrativa rigorosa, um usuário não-admin de um time Miro configurado para integração com Asana pode colar um link do Asana em um board da Miro. Essa ação pode disparar um diálogo de "solicitação de instalação do aplicativo" para o usuário, solicitando que ele busque a aprovação administrativa.
   - Os admins designados podem então revisar e aprovar essa solicitação pendente através de seus consoles administrativos do Miro ou do Asana, dependendo do fluxo de consentimento específico configurado.
4. **Conexão de usuário individual:**
   - Após a integração ter sido instalada e autorizada com sucesso no nível do time por um admin, usuários individuais deverão clicar em **Conectar** no widget do Asana que aparece no board da Miro.
   - Os usuários serão então redirecionados para uma página de autorização do Asana, onde concedem à Miro acesso à sua conta individual do Asana, confirmando assim sua autorização pessoal para incorporar e interagir com o conteúdo.

## Considerações de segurança e conformidade

### Restrição de acesso ao arquivo-fonte

Para garantir que o acesso aos dados incorporados do Asana permaneça restrito aos mesmos indivíduos do arquivo fonte do Asana, os administradores da organização Miro devem manter controles rigorosos sobre o compartilhamento de boards e a exportação de conteúdo. Embora a integração central do Asana respeite permissões individuais para interação ao vivo, qualquer exportação ou captura estática do conteúdo do board pode potencialmente expor dados a indivíduos não autorizados se o próprio board do Miro não for gerenciado com segurança.

### Tratamento de erros

A integração foi projetada com uma interface de usuário e tratamento de erros que permitem uma resposta eficaz em casos em que atualizações de dados de cartão falhem devido à rejeição de terceiros.

### Adendo de Processamento de Dados da Miro (DPA)

Para obter detalhes abrangentes sobre os aspectos jurídicos e de conformidade referentes às práticas de processamento de dados da Miro, os administradores devem consultar o [Anexo de Processamento de Dados da Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Solução de problemas e FAQs

### Como desativar a integração (desinstalação em nível de time)?

Um admin de time da Miro pode desinstalar a integração com o Asana no nível de time. Esta ação desabilita a integração para todos os membros do time. Para fazê-lo, vá para **Configurações do time Apps e Integrações**. Encontre "Asana Ticketing" na lista de apps instalados, desça a tela e clique em **Desinstalar para o time**.

### Como desativar a integração (desinstalação individual)?

Usuários individuais podem desinstalar a integração para si mesmos. Navegue até **Apps e Integrações** nas suas configurações da Miro. Localize "Asana Ticketing" e clique em **Desinstalar para mim**.

### Quais administradores podem instalar a integração Asana para o seu time?

Somente os admins de time da Miro podem instalar o aplicativo diretamente. Se um admin do time da Miro colar um URL do Asana em um board da Miro, o aplicativo será automaticamente autorizado e instalado sem necessidade de ação adicional.

### Quais são os requisitos de disponibilidade para a integração Asana?

A integração Asana está disponível para os planos Business e Enterprise da Miro.

### Os administradores precisam autorizar a integração Asana para o seu time?

Sim, os admins podem precisar autorizar a integração com o Asana para o time no Miro. Os membros do time só podem usar a integração com o Asana se ela tiver sido instalada no nível do time.
