---
title: Agrega Miro a las aplicaciones permitidas
article_id: 360017572694
translation_id: 360017572694
locale: es
sidebar_position: 1
created_at: '2019-02-11T10:14:41Z'
updated_at: '2026-03-03T20:16:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Relevante para: todos los usuarios de Miro'
---

En algunas ocasiones, es posible que las funciones de Miro no funcionen bien cuando no se concede acceso a Miro. Lo anterior puede ocurrir por dificultades o limitaciones aplicadas a tu conexión de red o el entorno que uses. El artículo siguiente aborda las causas más comunes de dichas dificultades.

## WebSockets

La aplicación de Miro, especialmente las páginas del *tablero*, requiere conexiones de WebSocket. Si tienes dificultades para abrir tus tableros, pero el panel y las páginas de ajustes se abren como deberían, esto puede ser señal de que tu conexión no es compatible con WebSockets.

Para probar tu conexión, por favor abre [este sitio web](http://websocketstest.com).

Si se identifican los Websockets, verás el mensaje siguiente:

![wensocket_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264610066_wensocket%20connection.jpg)

Si el resultado es diferente, lo más probable es que haya algo en tu red que obstruya las conexiones de WebSocket. Si este es el caso, intenta lo siguiente:

- Usa una conexión de red diferente
- Usa o desactiva una VPN
- Si usas una conexión empresarial, comunícate con el administrador de tu red y pídele que habilite las conexiones de WebSocket en el puerto 80 y 443 (SSL). Pueden estar cerradas o filtradas dentro de la red de tu empresa por motivos de seguridad. Para establecer una conexión, estos puertos deben estar abiertos para las direcciones de Miro a fin de acceder (ver direcciones en la sección "Si usas un Firewall" a continuación)

Si los Websockets se identifican correctamente, pero aún hay dificultades para establecer la conexión, por favor [comunícate con el servicio de soporte de Miro](https://help.miro.com/hc/requests/new?referer=help-center-article).

## Si usas un Firewall

Debes agregar nuestras direcciones IP estáticas a la lista de admitidos. Ten en cuenta que las direcciones de IP se utilizan solo para conectarse a los sistemas de Atlassian en relación con las integraciones de Jira que tenemos. Las direcciones IP de la aplicación Miro son *dinámicas*.
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

### Lista de admitidos de dominios de Miro

Las organizaciones que utilizan una red segura deben permitir todos los dominios de Miro. Para ver la lista completa de dominios que debes permitir, consulta [Dominios de Miro](../technical-guidelines/07-miro-domains-reference.md).

## Si usas un proxy

Asegúrate de dar acceso a Miro. Las siguientes especificaciones serán útiles.

- El servidor proxy debe ser compatible con conexiones de WebSocket (HTTP/2).
- La versión de HTTP de proxy debe ser 1.1.
- IP/host fuente: ver las IP de NAT anteriores (solo se usan para integraciones de Atlassian).
- Puerto fuente: **80.** Se usa 80 para los usuarios que acceden a Miro a través de HTTP para dirigirlos a HTTPS (no se recomienda bloquear 80).
- Puerto de destino: **443 (SSL).**443 se usa para HTTPS.
- Protocolo: HTTPS
- TLS: 1.2. (Estamos alojados en AWS y usamos políticas de seguridad de AWS. Cuando AWS y todos nuestros socios de plugin empiecen a ser compatibles con 1.3., también podemos migrar).
- Debe prolongarse el valor de tiempo de espera en el servidor proxy. Lo más probable es que tu sistema espere de 60 a 90 segundos para conectarse. Lo mejor es prolongarlo a 120-180 segundos.
- El servidor proxy no debe truncar la solicitud ni los encabezados de respuesta. Verifica si el cliente usa un proxy para los encabezados *de Actualizar* y *Conexión*.

[Aquí hay un artículo](../../tools/troubleshooting/02-allowlist-miro-mailers.md) con más información sobre los correos que necesitas en la lista de admitidos.
