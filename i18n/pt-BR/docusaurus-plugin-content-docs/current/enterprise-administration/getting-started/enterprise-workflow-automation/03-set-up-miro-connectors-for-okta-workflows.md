---
title: Configurar conectores Miro para fluxos de trabalho Okta
article_id: 8166481458706
translation_id: 8166481458706
locale: pt-br
sidebar_position: 2
created_at: '2022-10-19T06:52:05Z'
updated_at: '2025-02-26T11:59:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Os conectores Miro para fluxos de trabalho Okta permitem que você automatize facilmente tarefas admin repetitivas e de várias etapas no Miro. Aprenda a configurar a automação do fluxo de trabalho e simplificar o gerenciamento de time e usuário .

> **Relevante para:** Plano Enterprise

## Conector de gerenciamento de usuários Miro

O Miro User Management Connector permite que clientes empresariais Miro com SCIM habilitado adicionem usuários à sua organização e gerenciem licenças e status de usuários.

**Autorize seu Miro User Management Connector:**

Ao adicionar um cartão de gerenciamento de usuários do Miro a um fluxo pela primeira vez, você será solicitado a configurar uma conexão para sua organização. Ver Autorização.

**Cartões de ação do Miro User Management Connector:**

|  |  |
| --- | --- |
| Ação | Descrição |
| Criar usuário | Cria um novo usuário. |
| Ler usuário | Pesquisar um usuário existente em uma organização por e-mail. |
| Atualizar tipo de licença de usuário para completo | Atualiza um recurso de usuário existente, alterando seu Tipo de Licença de Usuário para **Completo**. |
| Atualizar status do usuário | Atualiza um recurso de usuário existente, alterando seu status ativo para um valor verdadeiro ou falso.O conector de gerenciamento de usuários Miro funciona usando seu token SCIM. O Miro User Management está disponível apenas para empresas com SSO e SCIM habilitados. |

## Autorização

Você pode criar e gerenciar várias conexões na página**Conexões** .
Isso é útil se você plano operar com várias organizações. Cada conexão para o Miro User Management Connector pode apontar para apenas uma Miro Organization.

Para habilitar o SCIM e obter um novo token, ou copiar um token existente, siga as instruções em [Como habilitar o SCIM](https://developers.miro.com/docs/how-to-enable-scim).
Para criar uma nova conexão a partir de um cartão de ação:

1. Clique em **Nova conexão**.
2. Insira um **apelido de conexão**. Recomendamos um nome que represente a organização.
3. Habilite o provisionamento do SCIM na página de integração Enterprise do Miro, seguindo as [instruções](https://developers.miro.com/docs/how-to-enable-scim).
   1. Copie **a URL base** do Miro e cole-a no campo **URL base** na conexão
   2. Copie **o token da API** do Miro e cole-o no campo **Token de acesso**em Conexão
4. Clique em **Criar**. Isso salva sua conexão e o leva de volta ao seu fluxo.

### Criar usuário

Cria um usuário dentro da organização.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| **Detalhes do usuário** |  |  |  |
| E-mail | O endereço de e-mail do usuário. | Corda | VERDADEIRO |
| ativo | O status do usuário.   - **Verdadeiro**: o usuário está ativo. - **Falso**: o usuário está inativo.   Quando não especificado, o padrão é **false**. | Menu suspenso | FALSO |
| Tipo de licença de usuário | O tipo de licença do usuário.   - **Completa** - **Gratuito**    Quando não especificado, a licença de usuário é definida de acordo com a lógica interna do Miro , que depende do plano da organização. | Menu suspenso | FALSO |
| Cargo (Role): | O papel do usuário dentro da organização.   - **Membro da organização**: membro regular sem privilégios de admin . - **admin da organização**: usuário com privilégios de admin em toda a empresa.   Quando não especificado, o padrão é **Membro da Organização**. | Menu suspenso | FALSO |
| Nome |  |  |  |
| Nome de família | O sobrenome ou sobrenome do usuário. | Corda | FALSO |
| Nome dado | O nome fornecido pelo usuário. | Corda | FALSO |
| Nome de exibição | O nome a ser exibido no Miro. | Corda | FALSO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| **Usuário** |  |  |
| ID do usuário | O ID do novo usuário. | Corda |

### Ler usuário

Pesquisar um usuário existente em uma organização por e-mail

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| **Consulta** |  |  |  |
| E-mail | O endereço de e-mail do usuário a ser pesquisado | Corda | VERDADEIRO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| usuário |  |  |
| ID do usuário | O ID do usuário. | Número |
| Tipo de licença de usuário | O tipo de licença do usuário. | Número |
| ativo | O status do usuário.  - **Verdadeiro**: o usuário está ativo. - **Falso**: o usuário está inativo. | Número |
| Nome |  |  |
| Username (Nome de usuário). | O endereço de e-mail do usuário. | Número |
| Nome de família | O sobrenome ou sobrenome do usuário. | Número |
| Nome dado | O nome fornecido pelo usuário. | Número |
| Nome de exibição | O nome exibido no Miro. | Número |

### Atualizar tipo de licença de usuário para Completo

Atualiza um recurso de usuário existente, alterando seu tipo de usuário (licença) para **Completo**.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| usuário |  |  |  |
| ID do usuário | O ID do usuário. | Corda | VERDADEIRO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| resposta |  |  |
| Código de status | status HTTP da solicitação.  Códigos que indicam atualização de licença bem-sucedida:   - 200. OK    Códigos que indicam atualização de licença malsucedida:   - 400. Solicitação malformada - 401. Não autorizado - 403. Proibido - 404. não encontrado - 409. Conflito - 429. Muitas solicitações | Número |

### Atualizar status do usuário

Atualiza um recurso de usuário existente, alterando seu **status ativo** para um valor verdadeiro ou falso.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| usuário |  |  |  |
| ID do usuário | O ID do usuário. | Corda | VERDADEIRO |
| ativo | O novo status do usuário.  - **Verdadeiro**: o usuário está ativo. - **Falso**: o usuário está inativo. | Menu suspenso | VERDADEIRO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| resposta |  |  |
| Código de status | status HTTP da solicitação.  Códigos que indicam atualização de status ativo bem-sucedida:   - 200. OK    Códigos que indicam atualização de status ativo sem sucesso:   - 400. Solicitação malformada - 401. Não autorizado - 403. Proibido - 404. não encontrado - 409. Conflito - 429. Muitas solicitações | Número |

## Conector de Administração Miro

O Miro Administration Connector permite que clientes empresariais criem times e gerenciem suas configurações de time e membros das times.

**Autorize seu conector de administração Miro**:

Ao adicionar um cartão Miro a um fluxo pela primeira vez, você será solicitado a configurar uma conexão para sua organização. Ver Autorização.

Cartões de ação **do Conector de Administração Miro** **:**

|  |  |
| --- | --- |
| Ação | Descrição |
| Criar time | Cria uma nova time em uma organização existente. |
| Pesquisar times | Pesquisar times existentes em uma organização. Os primeiros 10 registros correspondentes são selecionados do Conjunto de Resultados. |
| Adicionar membro à Team | Adiciona um novo membro a uma time existente. |
| Atualizar função de membro da Team | Atualiza a função de um time em uma time existente. |
| Obter configurações da Team | Recupera as configurações de time de uma time existente. |
| Atualizar as configurações de políticas de compartilhamento de Team | Atualiza as configurações da política de compartilhamento de uma time existente. |
| Atualizar configurações de convite de Team | Atualiza as configurações da política de convites de uma time existente. |
| Atualizar configurações de colaboração da Team | Atualiza as configurações da política de colaboração de uma time existente. |
| Atualizar as configurações de descoberta da Team | Atualiza as configurações da política de descoberta de uma time existente. |
| Atualizar configurações de acesso de cópia de Team | Atualiza as configurações da política de acesso de cópia de uma time existente. |
| Eliminação da sessão do usuário (BETA) | Limpa todas as sessões de usuário para um determinado endereço de e-mail. |

## Autorização

O Miro Administration Connector funciona usando o OAuth API Token. O Miro Administration Connector está disponível apenas para clientes no plano Enterprises. Para criar uma nova conexão, os usuários devem ter as permissões necessárias para instalar aplicativos com os escopos suportados abaixo.

Você pode criar e gerenciar várias conexões na página**Conexões** .
Isso é útil se você plano operar com várias organizações. Cada conexão para o Miro Administration Connector pode apontar para apenas uma Miro Organization.

Para criar uma nova conexão a partir de um cartão de ação:

1. Clique em **Nova conexão**.
2. Insira um **apelido de conexão**. Recomendamos um nome que represente a organização.
3. Obtenha **o ID da organização** e **o token de acesso** na página de integração Enterprise do Miro, seguindo as [instruções](02-miro-connector-for-okta-workflows.md).
4. Clique em **Criar**. Isso salva sua conexão e o leva de volta ao seu fluxo.

Escopos suportados:

- organizações: times:escrever
- organizações: times:ler

### Criar time

Cria um time em uma organização existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | **Tipo de** | **(obrigatório)** |
| = membros do time |  |  |  |
| Nome do time | O nome do time. | Corda | VERDADEIRO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| resposta |  |  |
| ID da Team | O ID da nova time. | Corda |

### Pesquisar times

Pesquisar times existentes em uma organização. Os primeiros 10 registros correspondentes são selecionados do Conjunto de Resultados.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| **Consulta** |  |  |  |
| Nome do time | Palavras que devem ser combinadas com o nome da time . Qualquer time cujo nome contenha essas palavras exatas será retornada como um conjunto de resultados. As equipes com nomes que correspondem totalmente à consulta estarão no topo do resultado. | Corda | FALSO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| resposta |  |  |
| **Times** | Lista com os 10 primeiros times encontrados. Cada time tem os campos abaixo. | Lista |
| ID da Team | O ID da time | Corda |
| Nome | Nome da time | Corda |

### Adicionar membro à time

Adiciona um novo membro a uma time existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| = membros do time |  |  |  |
| ID da Team | O ID da time. | Corda | VERDADEIRO |
| Membro |  |  |  |
| E-mail do usuário | O e-mail do usuário que você deseja adicionar à time. | Corda | VERDADEIRO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| resposta |  |  |
| ID do membro | O ID do novo membro do time. | Corda |

### Atualizar função do membro do time

Atualiza a função de um time em uma time existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| = membros do time |  |  |  |
| ID da Team | O ID da time. | Corda | VERDADEIRO |
| Membro |  |  |  |
| ID do membro | O ID do membro do time. | Corda | VERDADEIRO |
| Cargo (Role): | O novo papel do membro dentro da time.  - **Membro**: membro regular. - **admin**: membro com privilégios de admin dentro da time. - **Convidado da Team**: convidado com privilégios limitados. | Menu suspenso | VERDADEIRO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| resposta |  |  |
| ID do membro | O ID do membro do time. | Corda |
| Cargo | A nova função atribuída ao membro do time.  - **membro**: membro regular. - **admin**: membro com privilégios de admin dentro da time. - **team_guest**: convidado com privilégios limitados. | Corda |

### Obter configurações da Team

Recupera as configurações de time de uma time existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | **Tipo de** | **(obrigatório)** |
| = membros do time |  |  |  |
| ID da Team | O ID da time. | Corda | VERDADEIRO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| Configurações de convite do time |  |  |
| Quem pode convidar | - **only_org_admins**: somente admins da empresa podem convidar colaboradores. - **admins**: admins da empresa e admins de time podem convidar colaboradores. - **all_members**: todos os membros do time podem convidar colaboradores. | Corda |
| Convidar usuários externos | - **permitido**: permitir colaboradores que não sejam membros da time. - **Not_allowed**: não permitir colaboradores que não sejam membros da time. | Corda |
| **Configurações de colaboração em Team** |  |  |
| Função de coproprietário | - **habilitado**: habilitar a função de cotitular em boards e projetos. - **desabilitado**: desabilita a função de cotitular em boards e projetos. | Corda |
| **Configurações de nível de acesso de cópia de Team** |  |  |
| Nível de acesso de cópia | - **qualquer pessoa**: qualquer pessoa com acesso ao board pode copiar o conteúdo existente do board para boards recém-criados. AVISO: esta opção só estará disponível se **a Limitação do Nível de Acesso à Cópia** estiver definida como **qualquer pessoa**. - **team_members**: os membros do time podem copiar o conteúdo do board existente para boards recém-criados. - **team_editors**: membros do time com direitos de edição podem copiar o conteúdo do board existente para boards recém-criados. - **board_owner**: somente os titulares dos board podem copiar o conteúdo existente dos board para boards recém-criados. | Corda |
| Limitação do nível de acesso à cópia | - **qualquer pessoa**: membros do time e usuários de fora da time podem receber permissão para copiar o conteúdo do board . - **team_members**: somente membros do time podem receber permissão para copiar o conteúdo do board . | Corda |
| Configurações de visibilidade do time |  |  |
| Descoberta | - **oculto**: somente usuários convidados podem ver e acessar a time. - **solicitação**: os membros da organização podem encontrar a time e solicitar a entrada na time com a aprovação do admin . - **participar**: os membros da organização podem encontrar e participar da time. | Corda |
| **Configurações da política de compartilhamento de Team** |  |  |
| Acesso padrão ao board | - **privado**: somente os titulares dos board podem acessar os boards. - **visualizar**: qualquer pessoa na time pode visualizar os boards. - **comentar**: qualquer pessoa na time pode adicionar comentários aos boards. - **editar**: qualquer pessoa na time pode editar os boards. | Corda |
| Acesso à organização padrão | - **privado**: somente os titulares dos board podem acessar os boards. - **visualizar**: qualquer pessoa na organização pode visualizar os boards. - **comentar**: qualquer pessoa na organização pode adicionar comentários aos boards. - **editar**: qualquer pessoa na organização pode editar boards. | Corda |
| Compartilhando na Organização | - - **permitido**: permitir compartilhamento no nível da organização. - **allowed_with_editing**: permitir compartilhamento com direitos de edição no nível da organização. - **not_allowed**: não permitir compartilhamento no nível da organização. | Corda |
| Compartilhando na Team | - - **permitido**: permitir compartilhamento no nível da time . - **allowed_with_editing**: permitir compartilhamento com direitos de edição no nível da time . - **not_allowed**: não permitir compartilhamento no nível da time . | Corda |
| Compartilhamento por link público | - **permitido****: permitir compartilhamento via link público.** - **allowed_with_editing**: permitir compartilhamento com direitos de edição via link público. - **not_allowed**: não permitir compartilhamento via link público. | Corda |
| Mover board para o time | - **permitido**: permitir mover boards para uma time diferente. - **not_allowed**: não permitir a movimentação de boards para uma time diferente. | Corda |

### Atualizar as configurações da Política de Compartilhamento de Team

Atualiza as configurações da política de compartilhamento de uma time existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| = membros do time |  |  |  |
| ID da Team | O ID da time. | Corda | VERDADEIRO |
| Acesso padrão ao board | - **Privado**: somente os titulares dos board podem acessar os boards. - **Visualizar**: qualquer pessoa na time pode visualizar os boards. - **Comentário**: qualquer pessoa na time pode adicionar comentários aos boards. - **Editar**: qualquer pessoa na time pode editar os boards. | Menu suspenso | FALSO |
| Acesso à organização padrão | - **Privado**: somente titulares de board podem acessar os boards. - **Visualizar**: qualquer pessoa na time pode visualizar os boards. - **Comentário**: qualquer pessoa na time pode adicionar comentários aos boards. - **Editar**: qualquer pessoa na time pode editar os boards. | Menu suspenso | FALSO |
| Compartilhamento por link público | - **Permitido**: permitir compartilhamento via link público. - **Permitido com edição**: permitir compartilhamento com direitos de edição via link público. - **Não permitido**: não permitir compartilhamento via link público. | Menu suspenso | FALSO |
| Compartilhando na Team | - **Permitido**: permitir compartilhamento em nível de time . - **Permitido com edição**: permite compartilhamento com direitos de edição no nível da time . - **Não permitido**: não permitir compartilhamento em nível de time . | Menu suspenso | FALSO |
| Compartilhando na Organização | - **Permitido**: permitir compartilhamento no nível da organização. - **Permitido com edição**: permitir compartilhamento com direitos de edição no nível da organização. - **Não permitido**: não permitir compartilhamento no nível da organização. | Menu suspenso | FALSO |
| Mover board para o time | - **Permitido** mover boards para uma time diferente. - **Não permitido:** não permitir mover boards para uma time diferente. | Menu suspenso | FALSO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| **Configurações da política de compartilhamento de Team** |  |  |
| Acesso padrão ao board | - **privado**: somente os titulares dos board podem acessar os boards. - **visualizar**: qualquer pessoa na time pode visualizar os boards. - **comentar**: qualquer pessoa na time pode adicionar comentários aos boards. - **editar**: qualquer pessoa na time pode editar os boards. | Corda |
| Acesso à organização padrão | - **privado**: somente os titulares dos board podem acessar os boards. - **visualizar**: qualquer pessoa na organização pode visualizar os boards. - **comentar**: qualquer pessoa na organização pode adicionar comentários aos boards. - **editar**: qualquer pessoa na organização pode editar boards. | Corda |
| Compartilhando na Organização | - - **permitido**: permitir compartilhamento no nível da organização. - **allowed_with_editing**: permitir compartilhamento com direitos de edição no nível da organização. - **not_allowed**: não permitir compartilhamento no nível da organização. | Corda |
| Compartilhando na Team | - - **permitido**: permitir compartilhamento no nível da time . - **allowed_with_editing**: permitir compartilhamento com direito de edição no nível da time . - **not_allowed**: não permitir compartilhamento no nível da time . | Corda |
| Compartilhamento por link público | - - **permitido**: permitir compartilhamento via link público. - **allowed_with_editing**: permitir compartilhamento com direitos de edição via link público. - **not_allowed**: não permitir compartilhamento via link público. | Corda |
| Mover board para o time | - **permitido**: permitir mover boards para uma time diferente. - **not_allowed**: não permitir a movimentação de boards para uma time diferente. | Corda |

### Atualizar configurações de convite de Team

Atualiza as configurações da política de convites de uma time existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| = membros do time |  |  |  |
| ID da Team | O ID da time. | Corda | VERDADEIRO |
| Convidar usuários externos | - **Permitido**: permitir colaboradores que não sejam membros da time. - **Não permitido:** não permitir colaboradores que não sejam membros da time. | Menu suspenso | FALSO |
| Quem pode convidar | - **Somente admins da organização**: somente admins da empresa podem convidar colaboradores. - **admins**: admins da empresa e admins de time podem convidar colaboradores. - **Todos os membros**: todos os membros do time podem convidar colaboradores. | Menu suspenso | FALSO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| Configurações de convite do time |  |  |
| Convidar usuários externos | - **permitido**: permitir colaboradores que não sejam membros da time. - **Not_allowed**: não permitir colaboradores que não sejam membros da time. | Corda |
| Quem pode convidar | - **only_org_admins**: somente admins da empresa podem convidar colaboradores. - **admins**: admins da empresa e admins de time podem convidar colaboradores. - **all_members**: todos os membros do time podem convidar colaboradores. | Corda |

### Atualizar configurações de acesso à cópia da Team

Atualiza as configurações da política de acesso de cópia de uma time existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| = membros do time |  |  |  |
| ID da Team | O ID da time. | Corda | VERDADEIRO |
| Nível de acesso de cópia | - **qualquer pessoa**: qualquer pessoa com acesso ao board pode copiar o conteúdo existente do board para boards recém-criados. - **Membros da Team**: os membros do time podem copiar o conteúdo do board existente para boards recém-criados. - **Editores de Team**: membros do time com direitos de edição podem copiar o conteúdo existente do board para boards recém-criados. - **board_owner**: somente os titulares dos board podem copiar o conteúdo existente dos board para boards recém-criados. | Menu suspenso | FALSO |
| Limitação do nível de acesso à cópia | - **Qualquer pessoa**: membros do time e usuários de fora da time podem receber permissão para copiar o conteúdo do board . - **Membros da Team**: somente membros do time podem receber permissão para copiar o conteúdo do board . | Menu suspenso | FALSO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| **Configurações de acesso à cópia da Team** |  |  |
| Nível de acesso de cópia | - **qualquer pessoa**: qualquer pessoa com acesso ao board pode copiar o conteúdo existente do board para boards recém-criados. - **team_members**: os membros do time podem copiar o conteúdo do board existente para boards recém-criados. - **team_editors**: membros do time com direitos de edição podem copiar o conteúdo do board existente para boards recém-criados. - **board_owner**: somente os titulares dos board podem copiar o conteúdo existente dos board para boards recém-criados. | Corda |
| Limitação do nível de acesso à cópia | - **qualquer pessoa**: membros do time e usuários de fora da time podem receber permissão para copiar o conteúdo do board . - **team_members**: somente membros do time podem receber permissão para copiar o conteúdo do board . | Corda |

### Atualizar as configurações de colaboração da Team

Atualiza as configurações da política de colaboração de uma time existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| = membros do time |  |  |  |
| ID da Team | O ID da time. | Corda | VERDADEIRO |
| Função de coproprietário | - **Habilitado**: habilita a função de cotitular em boards e projetos. - **Desativado**: desabilita a função de cotitular em boards e projetos. | Menu suspenso | FALSO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| **Configurações de colaboração em Team** |  |  |
| Função de coproprietário | - **habilitado**: habilitar a função de cotitular em boards e projetos. - **desabilitado**: desabilita a função de cotitular em boards e projetos. | Corda |

### Atualizar as configurações do Team Discovery

Atualiza as configurações da política de descoberta de uma time existente.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| = membros do time |  |  |  |
| ID da Team | O ID da time. | Corda | VERDADEIRO |
| Descoberta | - **Oculto**: somente usuários convidados podem ver e acessar a time. - **Solicitação**: os membros da organização podem encontrar e solicitar a entrada na time com aprovação do admin . - **Participar**: os membros da organização podem encontrar e participar da time. | Menu suspenso | FALSO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| Configurações de visibilidade do time |  |  |
| Descoberta | - **oculto**: somente usuários convidados podem ver e acessar a time. - **solicitação**: os membros da organização podem encontrar e solicitar a entrada na time com aprovação do admin . - **participar**: os membros da organização podem encontrar e participar da time. | Corda |

### Eliminação da sessão do usuário

Limpa todas as sessões de usuário para um determinado endereço de e-mail.

Entrada

|  |  |  |  |
| --- | --- | --- | --- |
| **Campo** | **Definição** | Tipo de | **(obrigatório)** |
| **Detalhes do usuário** |  |  |  |
| E-mail | O endereço de e-mail do usuário cujas sessões devem ser apagadas. | Corda | VERDADEIRO |

Saída

|  |  |  |
| --- | --- | --- |
| **Campo** | **Definição** | Tipo de |
| resposta |  |  |
| Código de status | status HTTP da solicitação.  Códigos que indicam atualização bem-sucedida da eliminação da sessão do usuário :   - 200. Sessão de usuário excluída    Códigos que indicam atualização malsucedida de eliminação de sessão do usuário :   - 400. Solicitação malformada - 401. Não autorizado - 403. Proibido - 404. não encontrado - 409. Conflito - 429. Muitas solicitações | Número |
