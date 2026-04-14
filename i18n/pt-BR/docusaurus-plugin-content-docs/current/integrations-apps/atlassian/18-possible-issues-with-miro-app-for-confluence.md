---
title: "Poss\xEDveis problemas com o aplicativo da Miro para Confluence"
article_id: 360021388500
translation_id: 14537686631058
locale: pt-br
sidebar_position: 21
created_at: '2023-10-19T15:38:50Z'
updated_at: '2025-02-26T11:23:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
---

Use as dicas de solução de problemas abaixo se você tiver algum problema ao usar [o plugin Confluence](https://help.miro.com/hc/articles/360020712594).

|  |  |  |
| --- | --- | --- |
| **Mensagem / problema** | **Possíveis causas** | **Etapas para resolver o problema** |
| Você tem um seletor Miro preto/em branco ao tentar fazer login no Miro/incorporar boards da Miro nas páginas do Confluence | Configurações incorretas do navegador | Acesse as configurações do seu navegador e verifique se:   - A caixa de seleção **Impedir rastreamento entre sites** está desabilitada - A caixa de seleção **Bloquear todos os cookies** está desabilitada:   mceclip0.png   - **Janelas pop-up** nos sites Miro e Atlassian são permitidas:   mceclip1.png |
| Você tem permissão somente para visualizar este board e não pode compartilhá-lo ou incorporá-lo  **mceclip0.png** | Você não é um editor/ titular do board | - Verifique se:   - Você é um editor ou o titular do board - Você está autorizado em seu navegador no Miro com as credenciais corretas - Você incorpora um board no Confluence no mesmo navegador |
| Após incorporar uma board da Miro, você verá a mensagem: "O Miro requer acesso aos seus arquivos de cookie" | Seu navegador não permite salvar cookies de terceiros | Para habilitar a incorporação, você precisa habilitar os cookies no seu navegador. Isso acontece principalmente no Mozilla e Safári |
| A board incorporada mostra a mensagem de erro "Sua sessão expirou" |
| Ao tentar incorporar uma board, você recebe a seguinte mensagem: "Você não é membro de nenhuma time. Faça login na versão completa do produto e crie sua time ou deixe que alguém o convide para a equipe existente."  mceclip0.png | Você não é membro de nenhuma time sob o perfil da Miro autorizado no navegador | Vá até o [Miro](https://miro.com/app/dashboard/) e crie um time. Se você sabe que deve ser membro de alguma time(s) no Miro, abra o Miro em outra aba do navegador e certifique-se de que está autorizado com o **e-mail correto** |
