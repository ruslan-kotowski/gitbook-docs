---
title: Dodaj Miro do dozwolonych aplikacji
article_id: 360017572694
translation_id: 360017572694
locale: pl-pl
sidebar_position: 1
created_at: '2019-02-11T10:14:41Z'
updated_at: '2026-03-03T20:16:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Odpowiednie dla: wszystkich użytkowników Miro'
---

Czasami funkcje Miro mogą napotykać problemy, gdy Miro nie ma dostępu. Może się to zdarzyć z powodu problemów lub ograniczeń nałożonych na Twoje połączenie sieciowe lub środowisko, z którego korzystasz. Poniższy artykuł wymienia najczęstsze przyczyny takich problemów.

## WebSockets

Aplikacja Miro - szczególnie strony *tablic* - wymagają połączeń WebSocket. Jeśli masz problemy z otwieraniem swoich tablic, ale pulpit i strony ustawień otwierają się prawidłowo, może to oznaczać, że Twoje połączenie nie obsługuje WebSockets.

Aby przetestować swoje połączenie, otwórz [tę stronę](http://websocketstest.com).

Jeśli WebSockety zostały zidentyfikowane, zobaczysz następującą wiadomość:

![wensocket_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264610066_wensocket%20connection.jpg)

Jeśli wynik jest inny, najprawdopodobniej w Twojej sieci jest coś, co blokuje połączenia WebSocket. W takiej sytuacji spróbuj wykonać następujące działania:

- Użyj innego połączenia sieciowego
- Użyj VPN lub wyłącz go
- Jeśli korzystasz z połączenia korporacyjnego, skontaktuj się z administratorem sieci i poproś go o włączenie połączeń WebSocket na porcie 80 i 443 (SSL). Mogą być one zamknięte lub filtrują w twojej sieci korporacyjnej ze względów bezpieczeństwa. Aby nawiązać połączenie, te porty muszą być otwarte dla adresów Miro (zobacz adresy w sekcji "Jeśli używasz zapory sieciowej" poniżej)

Jeśli połączenia WebSocket są zidentyfikowane poprawnie, ale nadal występują problemy z nawiązaniem połączenia, skontaktuj się z [pomocą Miro](https://help.miro.com/hc/requests/new?referer=help-center-article).

## Jeśli używasz zapory sieciowej

Musisz dodać nasze statyczne adresy IP do listy dozwolonych. Zwróć uwagę, że te adresy IP są używane wyłącznie do kontaktu z systemami Atlassian w kontekście integracji z Jira, które posiadamy. Adresy IP aplikacji Miro są *dynamiczne*.
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

### Lista dozwolonych domen Miro

Organizacje korzystające z zabezpieczonej sieci muszą zezwolić na wszystkie domeny Miro. Aby zobaczyć pełną listę domen, które musisz dodać do listy dozwolonych, zobacz [domeny Miro](../technical-guidelines/07-miro-domains-reference.md).

## Jeśli używasz serwera proxy

Upewnij się, że zapewnisz Miro obejście. Poniższe specyfikacje będą pomocne.

- Serwer proxy musi obsługiwać połączenia WebSocket (HTTP/2).
- Wersja HTTP proxy powinna być ustawiona na 1.1.
- Źródłowy IP/host: zobacz powyższe adresy IP NAT (używane wyłącznie do integracji z Atlassian).
- Źródłowy port: **80.** 80 jest używany dla użytkowników, którzy uzyskują dostęp do Miro przez HTTP w celu przekierowania na HTTPS (blokowanie portu 80 nie jest zalecane).
- Port docelowy: **443 (SSL).** 443 jest używany dla HTTPS.
- Protokoł: HTTPS
- TLS: 1.2 (Jesteśmy hostowani w AWS i korzystamy z AWS Security Policies. Gdy AWS i wszyscy nasi partnerzy wtyczek zaczną obsługiwać 1.3, również będziemy mogli się migrować).
- Wartość limitu czasu na serwerze proxy powinna zostać przedłużona. Najprawdopodobniej system czeka około 60-90 sekund na połączenie. Najlepiej byłoby przedłużyć go do 120-180 sekund.
- Serwer proxy nie powinien skracać nagłówków żądań i odpowiedzi. Proszę sprawdzić, czy nagłówki *Upgrade* i *Connection* są przekazywane przez klienta.

[Oto artykuł](../../tools/troubleshooting/02-allowlist-miro-mailers.md) z dalszymi informacjami na temat mailerów, które należy dodać do listy dozwolonych.
