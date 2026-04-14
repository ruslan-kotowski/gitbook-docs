---
title: "Perguntas frequentes sobre os cart\xF5es do Jira"
article_id: 360013463739
translation_id: 14537387838226
locale: pt-br
sidebar_position: 17
created_at: '2023-10-19T15:27:38Z'
updated_at: '2025-10-14T19:23:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Este artigo responde às perguntas mais populares sobre como nossa integração com os cartões do Jira foi construída.

**Segurança**

**Como funciona a autenticação entre Jira e Miro?**

Consulte os artigos da Central de ajuda para

- **Jira Server on-premise**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Terceiros) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Data Center no local**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Terceiros) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Cloud**
  Selecione da página de configurações dos cartões do Jira.
  - [OAuth 2.0](https://help.miro.com/hc/articles/8588617184402) (3LO)

**Os dados são protegidos durante a transmissão entre o Jira e a Miro?**

Utilizamos o protocolo de segurança TLS. Ele criptografa mensagens HTTP antes da transmissão e as descriptografa na chegada. Também oferecemos suporte a mutual TLS para o [Enterprise plan](https://help.miro.com/hc/articles/360017730433).

**Vocês oferecem suporte a mutual TLS?**

Sim, [saiba mais](https://help.miro.com/hc/articles/4410562720658).

**A Miro retém algum dado do Jira do cliente?**

Sim, a Miro retém os dados dos cartões que são adicionados ao board.

**Qual é o período de retenção e como os dados são protegidos?**

Para OAuth 1.0 (Jira Server ou Data Center), os dados também são atualizados se os webhooks estiverem configurados durante o processo de configuração do plugin dos cartões do Jira. O período de retenção é ilimitado. Somente os protocolos de segurança gerais da Miro são aplicados.

**É possível restringir as informações que são obtidas da Miro?**

Não encontramos nenhuma menção na [documentação da Atlassian](https://developer.atlassian.com/server/jira/platform/webhooks/) sobre como limitar as informações apenas a alguns campos.

**Podemos ter um diagrama mostrando o fluxo de dados entre o Jira e a Miro?**

Informações detalhadas podem ser encontradas neste [artigo para desenvolvedores do Jira](https://developer.atlassian.com/server/jira/platform/oauth/). Nossa integração é implementada de acordo com a documentação da Atlassian.

**Como o token é gerenciado?**

OAuth 1.0: Apenas o token de acesso é usado. O token de acesso persiste [por 5 anos, a menos que](https://developer.atlassian.com/server/jira/platform/oauth) seja revogado (não há opção para personalizar, pois essa política é definida do lado da Atlassian. Você pode revogar o token do lado do Jira usando a interface web). Lembre-se de que cada novo token interrompe a integração e requer [reconexão](https://help.miro.com/hc/articles/360019501754#Step_2_-_Connection).

OAuth 2.0: O token de acesso dura 1 hora. O token de atualização dura 90 dias (se você passar 90 dias sem usar a integração, será necessário reautenticar).

**É usado um único token de acesso para todo o acesso do cliente ao Jira?**

Cada usuário da Miro que pretenda importar, criar ou editar cartões do Jira deve conectar suas credenciais do Jira individualmente. Todas as ações acima só podem ser realizadas em nome de credenciais individuais do Jira.

**Como os tokens de solicitação, tokens de acesso, chaves privadas e outros segredos e credenciais OAuth são protegidos?**

Durante a integração, apenas tokens de acesso são usados. Eles são armazenados de maneira segura dentro do banco de dados e são utilizados apenas no lado do servidor.

No OAuth 1.0. (Jira Server e Data Center) o authToken é usado apenas para o webhook. Ele não é o token de autenticação utilizado pelo OAuth. As requisições são enviadas através de uma conexão criptografada. A chave secreta é gerada automaticamente e é associada por time.

**Quais endpoints sua integração utiliza?**

```
POST /rest/api/2/issue - criar novo item
```

```
PUT /rest/api/2/issue/id - atualizar item
```

```
GET /rest/api/2/user/picker?query=xx
```

```
GET /rest/api/2/myself
```

```
GET /rest/api/2/filter/favourite
```

```
GET /rest/api/2/issue/picker
```

```
GET /rest/api/2/serverInfo
```

```
GET /rest/api/2/issue/$key
```

```
GET /rest/api/2/issue/createmeta
```

```
GET /rest/api/2/issue/$key/editmeta
```

```
GET /rest/api/2/priority
```

```
GET /rest/api/2/issuetype
```

```
GET /rest/api/2/mypermissions
```

Para OAuth 1.0. (Jira Server e Data Center) adicionalmente, usamos:

```
POST /rest/webhooks/1.0/webhook
```

**Os cartões funcionarão com o Jira Datacenter?**

Sim. Somos aprovados pela Atlassian e já temos muitos clientes usando com sucesso os cartões do Jira com o Datacenter. O procedimento de instalação é o mesmo.

**Quais IPs vocês estão usando para se comunicar com o sistema Jira?**

A lista dos nossos endereços IP estáticos pode ser encontrada [aqui](https://help.miro.com/hc/articles/360017572694).

Observe que esses são os endereços usados apenas para se comunicar com o sistema Jira. Os IPs do aplicativo Miro são dinâmicos e, para garantir que todas as funcionalidades nos boards da Miro (incluindo algumas relacionadas aos cartões do Jira) funcionem corretamente, pedimos que [adicione nossos domínios à sua lista de permissões](https://help.miro.com/hc/articles/360017572694).

**Podemos integrar o Jira com a Miro, mas bloquear itens do Jira com Nível de Segurança definido como "Privado"?**

Não, essa não é uma opção. Os Níveis de Segurança no Jira não têm correlação com a Miro.

**Geral**

**Podemos conectar o Miro ao Jira se usarmos um servidor Jira?**

Como o Miro é uma ferramenta online, você só pode se conectar ao Jira quando sua instância estiver aberta para a internet pública.

**Podemos conectar várias instâncias do Jira ao mesmo tempo?**

Sim. No entanto, lembre-se de que conectar uma instância do Jira é sobre estabelecer o link inicial, enquanto uma conexão ativa se refere à instância vinculada atualmente em uso. Uma conexão ativa define de onde os cartões do Jira são importados quando você abre o aplicativo de cartões do Jira, e para qual instância os usuários estão autorizados. Para um determinado usuário, só pode haver uma (1) conexão ativa por vez. Com OAuth 2.0, um usuário pode editar qualquer cartão do Jira associado a qualquer instância vinculada para a qual já está autenticado. Para qualquer outro protocolo de autenticação, uma equipe inteira compartilha uma instância ativa e pode apenas importar e interagir com cartões dessa instância. Você pode definir várias configurações em nível organizacional e alternar entre conexões ativas no nível do time.

**Qual é o processo de migração de Servidor para Cloud?**

Como sua URL base do Jira inevitavelmente mudará durante a migração para a nuvem, a integração será interrompida sem mudanças de nossa parte. Por favor, [entre em contato com o suporte da Miro](https://help.miro.com/hc/articles/360020185799) para assistência.

**A Miro criará um webhook por time, por projeto ou por instância da Miro?**

Se você ativar o Webhook Automático nas suas configurações da Miro, a criação do webhook ocorrerá automaticamente. Se você usar autorização ao nível de time com o Jira, então a Miro cria webhooks por time. Se você usar autorização ao nível de organização, então a Miro cria webhooks por organização.

**O plugin de cartões do Jira suporta projetos da próxima geração?**

Sim, suporta.

Observe que, atualmente, não há link/campo de Epic ao criar um cartão do Jira para um projeto da próxima geração no lado da Miro.

**Campos personalizados do Jira são suportados?**

Sim, damos suporte a quase todos os campos personalizados de tipos *básicos*. Se você tiver um campo de tipo de dado *complexo*, ele pode não ser suportado e causar um comportamento inesperado ao atualizar ou criar cartões do Jira no board.

**O que vai acontecer com os cartões do Jira existentes caso mudemos para outra instância do Jira?**

Atualmente, quando você move itens do Jira de um Projeto para outro no Jira, eles não são mais atualizados do lado da Miro.

Como solução alternativa, sugerimos que você copie a URL de um item do Jira (Ctrl/Cmd+C) e cole em um board da Miro (Ctrl/Cmd+V). Assim, um cartão do Jira exibirá novos valores e será atualizado automaticamente.

**Se um board for movido para outro time da Miro, o que acontecerá com os cartões do Jira no board?**

Os cartões do Jira permanecerão no board, mas ninguém poderá modificá-los (mesmo que a mesma instância do Jira esteja configurada para o time de destino).

Ao clicar em um cartão, você verá uma mensagem: *"O cartão do JIRA foi importado de outra conta"*. Se você deseja tornar os cartões editáveis, por favor, importe-os novamente para o board.

**Há custo adicional para a integração com os cartões do Jira?**

Os cartões do Jira estão disponíveis em todos os planos pagos e no Education sem custo adicional (planos Starter, Business, Education e Enterprise).

**Um usuário pode acessar todos os cartões do Jira no board?**

As permissões para a integração com os cartões do Jira garantem que os usuários possam apenas criar e editar cartões em projetos do Jira aos quais eles têm acesso.

Como todos os widgets em um board da Miro são visíveis para qualquer pessoa que tenha acesso ao board, se alguém não tiver credenciais do Jira ou não tiver as credenciais corretas, essa pessoa poderá visualizar o cartão do Jira colapsado em um board da Miro (com título e alguns outros campos), mas não poderá expandir o cartão para revisá-lo completamente ou modificá-lo.

**A Atlassian descontinuou o suporte para o Jira Server?**

Sim, a Atlassian descontinuou o suporte para o Jira Server a partir de fevereiro de 2024.

**O Miro Planner/cartões do Jira suporta os campos personalizados do Jira: tipos de itens personalizados e dependências personalizadas?**

Sim, ambos são suportados. Se os campos **tipos de itens personalizados** e **dependências personalizadas** estiverem configurados no Jira, *e* o Miro Planner estiver autenticado para essa instância do Jira, então esses campos personalizados estarão disponíveis no planner.

**A Miro suporta OAuth 2.0 para o Jira Data Center?**

Sim. Veja [Conectar ao Jira Data Center usando OAuth 2.0.](https://help.miro.com/hc/articles/25753304280466)

**Cartões do Jira em Tabelas e Linhas do Tempo**

**Como posso importar itens do Jira para Tabelas e Linhas do Tempo?**

Você pode arrastar e soltar um ou mais cartões do Jira diretamente em uma Tabela ou Linha do Tempo. Esta é atualmente a única maneira de fazê-lo.

**Todos os campos na Tabela se conectam ao Jira?**

Não, apenas cinco campos na Tabela sincronizam com o Jira na versão inicial:

Três campos do sistema Jira:

- Título
- Descrição
- Data de término (aparece como Data de Vencimento no Jira)

Dois campos personalizados do Jira:

- Data de início
- Estimativa

**Quais campos na Tabela não sincronizam com o Jira?**

Os campos Responsável e Status não sincronizam com o Jira e estão desabilitados nas Tabelas e Timeline. Esses campos e seus conteúdos existem, mas não são visíveis ou editáveis nas Tabelas e Timeline.

Você ainda pode editar esses campos diretamente nos cartões do Jira usando o painel lateral. Basta arrastar a linha da Tabela ou Timeline para o canvas para que o cartão do Jira reapareça.

Todos os demais campos, além dos cinco listados acima (Título, Descrição, Data de término, Data de início e Estimativa), são armazenados apenas no Miro e não sincronizam com o Jira.

**Por que não consigo editar um campo na Tabela ou Timeline a partir dos cinco campos do Jira acima suportados?**

O campo pode não estar presente na tela de edição no Jira.

Uma maneira fácil de verificar se o campo está presente na tela de edição ou não:

No Miro, abra o painel lateral do cartão do Jira. Verifique se o campo está presente no painel lateral. Se não estiver presente, você deve adicioná-lo à tela de edição no Jira.

Existem alguns casos raros em que os campos são editáveis no Jira, mas não estão presentes na tela de edição do Jira. Nesses casos, esses campos não podem ser editados no Miro.

O campo que você não pode editar é **Data de início** ou **Estimativa**? Se sim:

O campo pode não estar presente no Jira ou estar ausente da tela de edição (consulte o ponto anterior)

Pode haver um problema de mapeamento para Data de início ou Estimativa, pois são campos personalizados do Jira.

Mapeamos esses campos de acordo com esta lógica:

- **Data de início**: Verificamos campos nomeados: Start Date , StartDate, Target Start
- **Estimativa**: Verificamos campos nomeados: Story Points, Story point estimate, Story Point, StoryPoints, StoryPoint
- Se o campo Data de início ou Estimativa não tiver um dos nomes listados acima, isso pode explicar por que a edição não está funcionando.

**Por que editar a Data de Início ou a Estimativa na Tabela ou Timeline da Miro não funciona ou atualiza o campo errado no Jira?**

Atualmente, contamos com mapeamento automatizado para os campos Data de Início e Estimativa no Jira. Como esses são campos personalizados no Jira, pode haver um caso em que vários campos na sua configuração do Jira correspondam aos critérios mencionados acima.

Selecionamos a primeira correspondência de acordo com a ordem dos nomes de campo mencionados acima:

Por exemplo, se um ticket do Jira tiver campos tanto de Story Points quanto de Estimativa de Story Points, nós correspondemos ao primeiro conforme a lista acima, que é Story Points. Portanto, quaisquer alterações no campo Estimativa na tabela atualizarão o campo Story Points no Jira, não a Estimativa de Story Points.

No momento, não há uma forma de contornar isso. Se você enfrentar esse problema, por favor, envie um feedback para a sua equipe de suporte, para que possamos entender melhor suas necessidades enquanto desenvolvemos capacidades de mapeamento de campo mais avançadas.

**Por que não posso importar cartões do Jira de 2 instâncias diferentes para uma Tabela ou Linha do Tempo?**

Atualmente, suportamos apenas uma instância do Jira por Tabela/Linha do Tempo. Uma vez que um cartão do Jira é importado para uma Tabela/Linha do Tempo, ela fica vinculada a essa instância específica do Jira.

Mesmo que todos os registros do Jira sejam apagados, o vínculo com a instância original do Jira permanece. Para importar cartões de uma instância diferente do Jira, é necessário criar uma nova Tabela/Linha do Tempo.

**Por que não posso ver ou editar os campos de Status e Responsável dos meus registros do Jira em uma Tabela ou Linha do Tempo?**

Atualmente, os campos de Status e Responsável do Jira não são suportados em Tabelas e Linha do Tempo. Decidimos desabilitar esses campos em Tabelas e Linha do Tempo para gerenciar expectativas, evitar confusões e possível perda de dados. Os campos de Status e Responsável do Jira e seus conteúdos existem, mas não aparecem em Tabelas ou Linha do Tempo.

Você ainda pode editar esses campos diretamente nos cartões do Jira usando o painel lateral. Basta arrastar a linha da Tabela ou Timeline para o canvas para fazer o cartão do Jira reaparecer.

**Mais informações:**

- [Cartões do Jira](https://help.miro.com/hc/articles/360017572434)
- [Como configurar e desinstalar Cartões do Jira](https://help.miro.com/hc/articles/360019501754)
- [Como configurar Webhook para Cartões do Jira](https://help.miro.com/hc/articles/360017731113)
- [Possíveis problemas com Cartões do Jira e complemento do Jira](https://help.miro.com/hc/articles/360017572654)
