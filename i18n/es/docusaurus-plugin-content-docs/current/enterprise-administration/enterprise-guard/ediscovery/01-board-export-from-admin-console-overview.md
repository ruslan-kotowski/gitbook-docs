---
title: "Resumen de exportaci\xF3n de tableros desde la consola de admin"
article_id: 26259747401362
translation_id: 26259747401362
locale: es
sidebar_position: 0
created_at: '2025-04-24T14:18:00Z'
updated_at: '2025-11-25T15:50:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

Los admins de eDiscovery ahora pueden exportar directamente tableros bajo retención legal desde la consola de admin.
Esta capacidad permite a los admins de eDiscovery:

- Iniciar exportaciones de tableros desde la consola de admin.
- Monitorea el progreso del trabajo de exportación en tiempo real a través de la pestaña **Exportaciones** dentro de cada caso.
- Filtra los trabajos de exportación por estado y creador y ve qué tableros están incluidos.
- Obtén un registro completo de contenido para cada tablero exportado.
- Ver una lista de tableros exportados y su metadata (clasificación, propietario, estado de exportación).
- Descargar tableros exportados individualmente, directamente desde la consola de admin.
- Completa el flujo de trabajo de exportación sin depender de APIs o integraciones.
- Cancelar trabajos de exportación en cola o en progreso.

:::note
Para exportar tableros y gestionar las operaciones de exportación, debes tener el [rol de admin de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.
:::

## **Capacidades de exportación de tableros**

- Cada **trabajo de exportación** puede contener hasta **1,000 tableros**.
- **Límites de exportación** por plan:

  - **Enterprise Guard:** Hasta **100** trabajos de exportación activos.
  - **Enterprise:** Hasta **10** trabajos de exportación activos.
- **Límites de procesamiento en paralelo**:

  - **Enterprise Guard**: Hasta **5** trabajos de exportación procesados en paralelo.
  - **Enterprise**: **1** trabajo de exportación procesado a la vez.
- **Registros de contenido con trabajos de exportación:** Las exportaciones pueden incluir opcionalmente un registro completo de contenido para cada tablero exportado.
- **Filtros para trabajos de exportación**: Filtra los trabajos de exportación y ve qué tableros están incluidos.
- **Cancelar trabajos de exportación en curso y en cola**: Gestiona el ancho de banda de exportación de manera eficiente.
  > ✏️ Cuando cancelas una exportación, todos los tableros en progreso se completarán y estarán disponibles para descargar. Cualquier tablero que no se haya iniciado no será exportado.

- **Acceso de descarga**: Los resultados están disponibles para descargar durante **14 días.**
- **Alcance de la consola de admin**: Solo las exportaciones iniciadas a través de la consola de admin aparecen en la pestaña **Exportaciones**. Los trabajos de exportación basados en API no están incluidos en la lista de la consola de admin.
