---
title: "Descripci\xF3n general de los registros de auditor\xEDa de Enterprise Guard"
article_id: 17331872857746
translation_id: 17331872857746
locale: es
sidebar_position: 0
created_at: '2024-02-27T21:08:55Z'
updated_at: '2025-11-25T15:41:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Los registros de auditoría proporcionan a los admins un registro completo de todos los eventos asociados con Enterprise Guard. Estos registros son un recurso valioso para la solución eficiente de problemas y ofrecen información detallada sobre eventos críticos, como actualizaciones de la política de tiempo de vida de la papelera y la política de permisos de tableros en la papelera, la creación, actualización o eliminación de políticas de retención para la organización, o la eliminación permanente de un tablero de la papelera. El seguimiento sistemático de estas actividades fortalece la supervisión, análisis y mantenimiento, asegurando un sistema seguro y bien gestionado.

## Eventos de Enterprise Guard en los registros de auditoría

Además de [los eventos existentes registrados](../../security-integrations/security-management/01-audit-logs.md), los registros de auditoría incluyen registros sobre las siguientes categorías de eventos y eventos asociados con Enterprise Guard.

### Política de papelera

La siguiente tabla enumera las categorías de eventos y las acciones de eventos registradas para el componente de la Política de papelera de la organización.

|  |  |
| --- | --- |
| **Categoría de evento** | **Acción del evento** |
| Administración | Se cambió la política de tiempo de vida de la papelera para la organización. |
| Administración | Se cambió la política de permisos de tableros en la papelera para la organización. |

*Tabla 1: Categorías de eventos y acciones de eventos registradas para el componente de la política de papelera de la organización*Para obtener más información sobre políticas de papelera, consulta [nuestra documentación](https://help.miro.com/hc/articles/13860817985426-Trash-Policy).

### Política de retención

La siguiente tabla enumera las categorías de eventos y las acciones de eventos registradas para el componente de las Políticas de Retención de Contenido.

|  |  |
| --- | --- |
| **Categoría de evento** | **Acción de evento** |
| Administración | Política de retención creada para la organización |
| Administración | Política de retención actualizada para la organización |
| Administración | Política de retención eliminada para la organización |

*Tabla 2: Categorías de eventos y acciones de eventos registradas para el componente de las Políticas de Retención de Contenido.*Para más información sobre las políticas de retención, consulta [nuestra documentación](https://help.miro.com/hc/articles/16855776325778-Retention-Beta).

### Descubrimiento de datos

La siguiente tabla enumera las categorías de eventos y las acciones de eventos registradas para el componente de Descubrimiento de Contenido.

|  |  |
| --- | --- |
| **Categoría de evento** | **Acción de evento** |
| Administración | Se cambió la detección de información privada para la organización  (habilitado/deshabilitado) |
| Administración | Suprimió un hallazgo de descubrimiento de datos en la organización |

*Tabla 3: Categorías de eventos y acciones de eventos registradas para el componente de Descubrimiento de Contenido*

Para obtener más información sobre el descubrimiento de datos, consulta [nuestra documentación](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md).

### Barreras de protección inteligentes

La siguiente tabla enumera las categorías de eventos y las acciones de eventos registradas para el componente de barreras de protección inteligentes.

|  |  |
| --- | --- |
| **Categoría de evento** | **Acción de evento** |
| Barreras de protección inteligentes | Barreras de protección inteligentes cambiadas para un tablero |

*Tabla 4: Categorías de eventos y acciones de eventos registradas para el componente de barreras de protección inteligentes*

Para más información sobre las Barreras de protección inteligentes, consulta [nuestra documentación](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md).

### eDiscovery

La siguiente tabla enumera las categorías de eventos y las acciones de eventos registradas para el componente de eDiscovery.

|  |  |
| --- | --- |
| **Categoría de evento** | **Acción de evento** |
| Administración | Caso creado para la organización |
| Administración | Caso cerrado para la organización |
| Administración | Se creó la retención legal para la organización |
| Administración | Retención legal cerrada para la organización |
| Administración | Retención legal aplicada al tablero Tablero liberado de la retención legal |

*Tabla 3: Categorías de eventos y acciones de eventos registradas para el componente eDiscovery*

Para más información sobre eDiscovery, consulta [nuestra documentación](https://help.miro.com/hc/sections/22049853357842-eDiscovery-Legal-Hold-Beta).
