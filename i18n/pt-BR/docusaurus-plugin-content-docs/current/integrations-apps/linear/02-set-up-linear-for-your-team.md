---
title: Configurar o Linear (Beta) para o seu time
article_id: 30630697364626
translation_id: 30630697364626
locale: pt-br
sidebar_position: 2
created_at: '2025-10-29T14:09:41Z'
updated_at: '2026-02-23T11:23:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

A integração do Linear é tecnicamente implementada por meio de uma REST API. Para fins de autenticação e autorização, utiliza-se o protocolo padrão da indústria OAuth 2.0. Um componente central dessa arquitetura é uma plataforma API unificada usada como sub-processador para dados de terceiros — gerenciando autenticação, normalização e sincronização entre diferentes provedores de API.

## Fluxos de dados

Compreender o fluxo de dados é crucial para gerenciar a segurança e a conformidade.

### Diagrama de sequência em alto nível

Criando um widget de cartão do Linear

![Asana Cards (BETA) (1).jpg](images/30631672640658_Asana%20Cards%20(BETA) (1).jpg)

Atualizando um widget de cartão do Linear

![Asana Cards (BETA) (1).jpg](images/30631672640658_Asana%20Cards%20(BETA) (1).jpg)

### Dados do Linear no Miro

Quando os usuários importam itens do Linear para um board da Miro, os seguintes dados são integrados ao canvas da Miro:

- Título
- Descrição
- Responsável (nome/e-mail)
- Status
- Prioridade

Esta enumeração é vital para a governança de dados, confirmando quais dados confidenciais são inseridos no ambiente da Miro. Observe que não há suporte a campos personalizados.

### Retenção de dados

Todos os dados importados do Linear aderem estritamente à política de retenção de dados padrão da Miro, aplicada consistentemente a todos os dados dos clientes.

## Autenticação e autorização

No primeiro contato, a integração com Linear inicia um fluxo de autenticação. Para cada usuário, a Miro cria credenciais com o serviço de integração para interações subsequentes.

A integração normalmente requer aprovação de um admin do Linear.

### Escopos de autorização necessários

| Escopo | Descrição |
| --- | --- |
| Coleções | Acesso a coleções de itens. |
| Usuários | Ler informações de usuários para atribuição/exibição. |
| Itens | Ler, criar, modificar itens no Linear. |

## O que é armazenado na Miro e como

- **Dados relacionados à autorização:** Os tokens são armazenados no banco de dados da Miro por vários dias, criptografados com AES-256.
- **Dados relacionados ao desfazimento:** Os títulos dos itens são armazenados com referências criptografadas.

### Revogação de um token

A revogação dos tokens pode ocorrer via **configurações de integração** ou **Aplicativos** ao selecionar **Desconectar**. Esta ação remove o acesso ao Linear e apaga as credenciais dos usuários.

## Como configurar a integração Linear

Passos para garantir a implantação controlada tanto para admins quanto para usuários finais.

1. **Garantir Contas Ativas:** As contas da Miro e da Linear devem estar ativas.
2. **Instalação a Nível de Time (Ação do Admin):**
   - Os admins devem autorizar a integração da Linear no nível do time.
   - Instalação via **Mídia de Ferramentas e Integrações**, buscando "Linear" e conectando.
3. **Solicitação do Usuário e Aprovação do Admin:**
   - Em organizações com consentimento rigoroso, colar um link do Linear pode acionar uma solicitação de aprovação pelo admin.
   - Os admins podem aprovar via consoles da Miro ou Linear.
4. **Conexão Individual do Usuário:**
   - Usuários se conectam pelo widget Linear e autorização OAuth.

## Segurança e conformidade

### Restrição de Acesso ao Arquivo-Fonte

Manter controles rigorosos de compartilhamento de board alinha as permissões do Linear com a Miro.

### Tratamento de erros

A integração apresenta uma funcionalidade de fallback de interface de usuário para rejeições de terceiros.

### Adendo de Processamento de Dados da Miro (DPA)

Consulte [o Adendo de Processamento de Dados da Miro](https://miro.com/legal/customer-data-processing-addendum/) para obter informações detalhadas sobre aspectos legais e de conformidade.

## Solução de problemas e perguntas frequentes

### Como desabilitar a integração (Nível de time)

Os admins podem desinstalar nas **Configurações de aplicativos e integrações do time** selecionando "Linear" e clicando em **Desinstalar para o time**.

### Como desabilitar a integração (Individual)

Os usuários podem navegar até **Apps e Integrações** e selecionar "Desinstalar para mim" para o Linear.

### Permissões de administrador

Somente admins de time da Miro podem instalar o aplicativo diretamente. Configurações automáticas ocorrem ao colar uma URL do Linear em um board.

### Requisitos de disponibilidade

A integração com o Linear está disponível para os planos Business e Enterprise.

### Autorização necessária do admin

Sim, a autorização no nível do time pelos admins é necessária para o acesso do time.
