---
title: Adicione a Miro a aplicativos permitidos
article_id: 360017572694
translation_id: 360017572694
locale: pt-br
sidebar_position: 1
created_at: '2019-02-11T10:14:41Z'
updated_at: '2026-03-03T20:16:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Relevante para: todos os usuários da Miro'
---

Ocasionalmente, as funções da Miro podem ter problemas de desempenho quando a Miro não tem acesso permitido. Isso pode acontecer devido a problemas ou limitações aplicadas à sua conexão de rede, ou ao ambiente que você usa. O seguinte artigo lista as causas mais comuns de tais problemas.

## WebSockets

O aplicativo da Miro — especificamente as páginas do *board* — requer conexões WebSocket. Se você estiver tendo problemas para abrir seus boards, mas o painel e as páginas de configurações abrirem como esperado, isso pode significar que sua conexão não é compatível com WebSockets.

Para testar sua conexão, abra [este site](http://websocketstest.com).

Se os WebSockets forem identificados, você verá a seguinte mensagem:

![wensocket_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264610066_wensocket%20connection.jpg)

Se o resultado for diferente, é muito provável que haja algo na sua rede que bloqueia as conexões WebSocket. Se este for o caso, tente o seguinte:

- Use uma conexão de rede diferente
- Use ou desligue uma VPN
- Se você usa uma conexão corporativa, entre em contato com seu administrador de rede e peça para habilitar as conexões WebSocket nas portas 80 e 443 (SSL). Elas podem ser fechadas ou passar por filtros na sua rede corporativa por razões de segurança. Para estabelecer uma conexão, essas portas devem estar abertas para que os endereços da Miro possam acessá-las (veja endereços na seção "Se você usar um Firewall" abaixo)

Se os Websockets forem identificados corretamente, mas ainda houver problemas para estabelecer a conexão, por favor, [entre em contato com o Suporte da Miro](https://help.miro.com/hc/requests/new?referer=help-center-article).

## Se você usar um Firewall

Você deve adicionar nossos endereços IP estáticos à lista de permissões. Observe que os endereços IP são usados apenas para acessar os sistemas da Atlassian em relação às integrações relacionadas ao Jira que temos. Os endereços IP do aplicativo Miro são *dinâmicos*.
52.16.47.17,
54.216.81.236,
54.217.180.21,
54.73.153.141,
34.249.78.135,
46.51.161.49,
54.217.110.122,
54.220.142.217,
54.228.53.200,
54.73.173.202,
54.73.41.83,
54.74.0.207,
54.74.167.92,
54.75.137.71,
52.64.11.98,
13.55.76.39,
13.54.151.233
3.131.34.166,
13.59.239.75,
13.59.239.75

### Lista de permissões de domínios da Miro

Organizações que usam uma rede segura devem permitir todos os domínios da Miro. Para ver a lista completa de domínios que você deve permitir, consulte [Domínios da Miro](../technical-guidelines/07-miro-domains-reference.md).

## Se você usar um proxy

Certifique-se de fornecer à Miro uma alternativa. As seguintes especificações ajudarão.

- O servidor proxy deve oferecer suporte às conexões WebSocket (HTTP/2).
- A versão HTTP do proxy deve ser definida como 1.1.
- IP de origem/host: veja os IPs NAT acima (usados apenas para integrações da Atlassian).
- Porta de origem: **80.** 80 é usada para usuários que acessam a Miro por meio de HTTP para direcioná-los para HTTPS (bloquear a porta 80 não é recomendado).
- Porta de destino: **443 (SSL).**443 é usada para HTTPS.
- Protocolo: HTTPS
- TLS: 1.2. (Estamos hospedados na AWS e usamos as Políticas de segurança da AWS. Quando a AWS e todos os nossos parceiros de plugins começarem a oferecer suporte à 1.3. poderemos migrar também).
- O valor de tempo limite no servidor proxy deve ser prolongado. É muito provável que seu sistema aguarde cerca de 60 a 90 segundos para se conectar. Seria melhor prolongá-lo para 120 a 180 segundos.
- O servidor proxy não deve truncar os cabeçalhos de solicitação e resposta. Verifique se os cabeçalhos de *atualização*e *conexão*são proxiados pelo cliente.

[Aqui está um artigo](../../tools/troubleshooting/02-allowlist-miro-mailers.md) com mais informações sobre os mailers que você precisa permitir na lista.
