---
title: eDiscovery Board-Exportfunktion in der Admin-Konsole
article_id: 26529264912146
translation_id: 26529264912146
locale: de
sidebar_position: 16
created_at: '2025-05-06T17:01:06Z'
updated_at: '2025-05-26T08:55:18Z'
draft: false
outdated: false
user_segment_id: 16307853619090
user_segment: Enterprise Company Admins
backstage_link:
  entity_kind: capability
  entity_id: content-explorer
---

Enterprise Guard-Administratoren können nun die Adminkonsole nutzen, um eDiscovery-Workflows effektiver zu unterstützen. Sie können:

- Alle Boards unter einer Aufbewahrungsfrist exportieren (selektiver Export wird nicht unterstützt).
- Liste der Exportaufträge (abgeschlossen, laufend und geplant) in jedem eDiscovery-Fall ansehen.
- Exportstatus für einzelne Boards in einem Vorgang einsehen.
- Die exportierten Boards können einzeln heruntergeladen werden und sind 14 Tage nach dem Export verfügbar.

**Exportgrenzen und Verhalten:**

- Jeder Exportauftrag kann bis zu **1000 Boards** beinhalten. Jobs werden nicht gestartet, wenn eine Aufbewahrungsfrist mehr als 1.000 Boards umfasst.
- Maximal **100 Exportaufträge** können in der Organisation aktiv sein.
- Bis zu **5 Aufträge** werden parallel verarbeitet (unverändert).

**API-Limits (Board-Export-API):**

- Bis zu **100 Exportaufträge** für Guard-Organisationen und **10 Aufträge** für Enterprise-Organisationen.
- Exportjob-Größenlimit: **1.000 Boards**.

Diese Updates helfen, die Prozesse für rechtliche Aufbewahrungen zu straffen und gleichzeitig Transparenz und Kontrolle über Board-Exportaktivitäten sicherzustellen.
