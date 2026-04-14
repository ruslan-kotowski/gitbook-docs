---
title: Ajouter Miro aux applications autorisées
article_id: 360017572694
translation_id: 360017572694
locale: fr
sidebar_position: 1
created_at: '2019-02-11T10:14:41Z'
updated_at: '2026-03-03T20:16:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Relevé pour: tous les utilisateurs de Miro'
---

Des fonctionnalités de Miro peuvent parfois rencontrer des difficultés en termes de performance lorsque Miro ne dispose pas des accès nécessaires. Cela peut se produire en raison de problèmes ou de limitations appliquées à votre connexion réseau ou à l’environnement que vous utilisez. L’article suivant liste les causes les plus courantes de ces difficultés.

## WebSockets

L’application Miro, notamment les pages de *tableau*, nécessitent des connexions de type WebSocket. Si vous rencontrez des difficultés en ouvrant vos tableaux, mais que le tableau de bord et les pages des paramètres s’ouvrent comme prévu, il est possible que votre connexion ne prenne pas en charge les WebSockets.

Pour tester votre connexion, veuillez ouvrir [ce site Web](http://websocketstest.com).

Si les Websockets sont identifiés, vous verrez le message qui suit :

![wensocket_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264610066_wensocket%20connection.jpg)

Si le résultat est différent, il est très probable que quelque chose dans votre réseau bloque les connexions de type WebSocket. Si tel est le cas, essayez les opérations suivantes :

- Utilisez une connexion réseau différente.
- Utilisez ou désactivez un VPN.
- Si vous utilisez une connexion d’entreprise, contactez l’admin du réseau et demandez à ce que les connexions WebSocket sur les ports 80 et 443 (SSL) soient activées. Il est possible qu’elles soient fermées ou filtrées à l’intérieur de votre réseau d’entreprise pour des raisons de sécurité. Afin d’établir une connexion, ces ports devraient être ouverts et accessibles pour les adresses Miro (voir les adresses dans la section « Si vous utilisez un pare-feu » ci-dessous).

Si les Websockets sont correctement identifiés mais que vous rencontrez toujours des problèmes pour établir la connexion, veuillez [contacter le service d’assistance de Miro](https://help.miro.com/hc/requests/new?referer=help-center-article).

## Si vous utilisez un pare-feu

Vous devez ajouter nos adresses IP statiques à la liste d’autorisations. Notez que les adresses IP sont utilisées uniquement pour communiquer avec les systèmes d’Atlassian dans le cadre des intégrations Jira que nous proposons. Les adresses IP de l’application Miro sont *dynamiques*.
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

### Liste d’autorisations des domaines Miro

Les organisations qui utilisent un réseau sécurisé doivent autoriser tous les domaines de Miro. Pour voir la liste complète des domaines à autoriser, consultez [Domaines de Miro](../technical-guidelines/07-miro-domains-reference.md).

## Si vous utilisez un proxy

Assurez-vous de fournir à Miro un by-pass. Les spécifications suivantes vous aideront.

- Le serveur proxy doit prendre en charge les connexions WebSocket (HTTP/2).
- La version HTTP du proxy doit être définie sur 1.1.
- Source IP/hôte : voir les IP NAT ci-dessus (utilisées uniquement pour les intégrations Atlassian).
- Port source : **80.** Le port 80 est utilisé pour les utilisateurs qui accèdent à Miro via HTTP, afin de les rediriger sur HTTPS (il n’est pas recommandé de bloquer le port 80).
- Port de destination : **443 (SSL).**Le port 443 est utilisé pour HTTPS.
- Protocole : HTTPS
- TLS : 1.2. (Nous sommes hébergés sur AWS et utilisons les politiques de sécurité d’AWS. Lorsque AWS et tous nos plugins partenaires commenceront à prendre en charge la version 1.3., nous pourrons également migrer à notre tour).
- La valeur du délai d’expiration sur le serveur proxy devrait être prolongée. Il est fort probable que votre système attende environ 60-90 secondes pour se connecter. Il serait préférable de prolonger ce délai à 120-180 secondes.
- Le serveur proxy ne doit pas tronquer les en-têtes de demande et de réponse. Vérifiez si les en-têtes *Upgrade* et *Connection* se font bien en proxy par le client.

[Voici un article](../../tools/troubleshooting/02-allowlist-miro-mailers.md) avec plus d’informations sur les expéditeurs que vous devez ajouter à la liste blanche.
