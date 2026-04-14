---
title: "Funci\xF3n de exportaci\xF3n de tableros de eDiscovery en la consola de administraci\xF3\
  n"
article_id: 26529264912146
translation_id: 26529264912146
locale: es
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

Los administradores de Enterprise Guard ahora pueden usar la consola de administración para apoyar los flujos de trabajo de eDiscovery de manera más efectiva. Pueden:

- Exportar todos los tableros bajo retención legal (no se admite la exportación selectiva).
- Ver una lista de trabajos de exportación (completados, en curso y planificados) dentro de cada caso de eDiscovery.
- Ver el estado de exportación de tableros individuales en un trabajo.
- Descarga los tableros exportados individualmente, disponibles durante 14 días después de la exportación.

**Límites y comportamiento de exportación:**

- Cada trabajo de exportación puede incluir hasta **1000 tableros**. Los trabajos no comenzarán si una retención legal incluye más de 1000 tableros.
- Un máximo de **100 trabajos de exportación** pueden estar activos en la organización.
- Hasta **5 trabajos** se procesan en paralelo (sin cambios).

**Límites de la API (API de exportación de tableros):**

- Hasta **100 trabajos de exportación** para organizaciones Guard y **10 trabajos** para organizaciones Enterprise.
- Límite de tamaño para trabajos de exportación: **1000 tableros**.

Estas actualizaciones ayudan a agilizar los procesos de retención legal mientras aseguran la transparencia y el control sobre las actividades de exportación de tableros.
