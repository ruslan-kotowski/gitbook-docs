---
title: Add Miro to allowed apps
article_id: 360017572694
sidebar_position: 2
created_at: '2019-02-11T10:14:41Z'
updated_at: '2026-04-07T07:50:48Z'
draft: false
availability:
  notes: 'Relevant for: all Miro users'
---

Occasionally Miro functions may have trouble performing when Miro is not allowed access. This can happen due to issues or limitations applied to your network connection or the environment that you use. The following article lists the most common causes of such issues.

## WebSockets

The Miro application - specifically the *board* pages - requires WebSocket connections. If you're having issues opening your boards but the dashboard and the settings pages open as expected this might mean that your connection does not support WebSockets.

To test your connection, please open [this website](http://websocketstest.com).

If the Websockets are identified, you'll see the following message:

![wensocket_connection.jpg](images/21020264610066_wensocket%20connection.jpg)

If the result is different, it's most likely that there's something in your network that blocks WebSocket connections. If this is the case try the following:

- Use a different network connection
- Use or turn off a VPN
- If you use a corporate connection contact your network administrator and ask them to enable the WebSocket connections on port 80 and 443 (SSL). They might be closed or filtered within your corporate network for security reasons. In order to establish a connection, these ports should be open for Miro addresses to access (see addresses in the "If you use a Firewall" section below)

If the Websockets are identified correctly but there are still issues establishing the connection, please [contact Miro Support](https://help.miro.com/hc/requests/new?referer=help-center-article).

## If you use a Firewall

You must add our static IP addresses to the allowlist. Note that the IP addresses are used only to reach out to the Atlassian systems in regard to the Jira-related integrations we have.

Miro application IP addresses are dynamic.

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
3.21.8.88

### Miro domains allowlist

Organizations that use a secured network must allow all Miro domains. To see the complete list of domains that you must allow, see [Miro domains](../technical-guidelines/07-miro-domains-reference.md).

## If you use a proxy

Please ensure that you provide Miro with a by-pass. The following specifications will help.

- The proxy server must support WebSocket connections (HTTP/2).
- The proxy HTTP version should be set as 1.1.
- Source IP/host: see the NAT IPs above (used for Atlassian integrations only).
- Source port: **80.** 80 is used for users that access Miro through HTTP to direct them to HTTPS (blocking 80 is not recommended).
- Destination port: **443 (SSL).**443 is used for HTTPS.
- Protocol: HTTPS
- TLS: 1.2. (We’re hosted in AWS and use AWS Security Policies. When AWS and all our plugin partners start supporting 1.3. we will be able to migrate as well).
- The timeout value on the proxy server should be prolonged. It is most likely that your system waits around 60-90 seconds to connect. It would be best to prolong it to 120-180 seconds.
- The proxy server should not truncate the request and response headers. Please check if the *Upgrade*and *Connection*headers are proxied by the client.

[Here is an article](../../tools/troubleshooting/02-allowlist-miro-mailers.md) with more information on the mailers you need to allowlist.
