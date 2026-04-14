---
title: "Introducci\xF3n a Enterprise Guard"
article_id: 15699815402514
translation_id: 15699815402514
locale: es
sidebar_position: 0
created_at: '2023-12-11T23:40:22Z'
updated_at: '2025-11-25T15:40:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

En la era digital actual, el crecimiento exponencial de los datos, especialmente de la información sensible, se ha convertido en una preocupación importante para las empresas. Miro, conocido por ser un espacio de trabajo de colaboración en línea preparado para empresas que fomenta la innovación y el trabajo en equipo, ha observado un aumento sustancial de la complejidad y volumen de contenido en sus tableros. Una cantidad notable de tableros de Miro contienen datos altamente sensibles, como Información de Identificación Personal (PII), Información de Salud Protegida (PHI), Información de Tarjetas de Pago (PCI) y más, lo que presenta desafíos para gestionar el riesgo y asegurar el cumplimiento. Esta tendencia resalta la importancia de aplicar medidas avanzadas de seguridad y cumplimiento para ayudar a prevenir posibles violaciones de datos y fugas de propiedad intelectual.

## Presentamos Enterprise Guard: una solución integral de seguridad y gobernanza para Miro

Consciente de estos retos, Miro presenta **Enterprise Guard**, un complemento avanzado de seguridad y gobernanza. Enterprise Guard ofrece un conjunto de funciones que permiten a las organizaciones identificar, clasificar, proteger y gestionar eficazmente el contenido confidencial en los tableros de Miro. Esta solución está adaptada para garantizar el cumplimiento normativo y una sólida protección de datos a escala.

Con la integración de Enterprise Guard en el ecosistema empresarial de Miro, las organizaciones pueden ahora aprovechar un marco de seguridad más robusto, automatizado y completo. Este complemento no trata solo de proteger datos—sino de permitir a las empresas seguir innovando y colaborando en Miro de forma segura, sin obstaculizar las operaciones del negocio.

## Versión de disponibilidad general de Enterprise Guard: funciones principales

![Enterprise Guard General Availability release key features](images/21019694868242_Enterprise-Guard-Data-Security.png)

- **Descubrimiento de datos:** Enterprise Guard habilita un [proceso de descubrimiento de datos](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md) proactivo y minucioso, crucial para identificar datos sensibles como números de tarjetas de crédito, números de seguridad social y otra información crítica dispersa por varios tableros de Miro. Esta estrategia proactiva es crucial para identificar y mitigar las vulnerabilidades potenciales, ayudándote a prevenir las violaciones de datos y garantizar el cumplimiento.
- **eDiscovery:** Habilitar la conservación, seguimiento y exportación segura de los datos del tablero para cumplir con los requisitos legales, de cumplimiento y de seguridad. La función eDiscovery en Enterprise Guard ayuda a las organizaciones a cumplir con las obligaciones regulatorias a través de [Retenciones Legales](../../canvas-25-admin-features/ediscovery/02-legal-hold-overview.md), [Registros de Contenido](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md) y capacidades de [Exportación de Tableros](../../canvas-25-admin-features/ediscovery/13-board-export-api-overview.md).

  Las retenciones legales evitan la eliminación permanente de contenido relevante para investigaciones o asuntos legales al preservar todos los tableros con los que interactúa un usuario bajo retención, incluidas todas sus versiones. Los registros de contenido proporcionan registros detallados de la actividad de los usuarios, que pueden ser exportados e integrados en herramientas externas para auditorías o revisiones legales. Con las API de eDiscovery, los clientes de Enterprise también pueden exportar datos de tableros a gran escala, asegurando que la información crítica sea accesible para los flujos de trabajo legales y de cumplimiento.
- **Clasificación automática**: Establece criterios para que Miro [clasifique automáticamente tus tableros](../../canvas-25-admin-features/data-classification/03-auto-classification-overview-and-scenarios.md) en función del contenido sensible encontrado en los tableros.
- **Barreras de protección inteligentes****:** [Aplica normas de seguridad en tiempo real](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md) y restringe lo que los usuarios pueden hacer con un tablero, como restringir la replicación del contenido del tablero y las capacidades de compartir en varios niveles (público, equipo, organización), en función de la clasificación manual o automatizada del tablero. Esto garantiza la privacidad y el cumplimiento de las normas sin obstaculizar las operaciones de la empresa.
- **Política de Papelera**: La [política de papelera](https://help.miro.com/hc/articles/13860817985426) de Enterprise Guard ofrece un mayor control sobre la eliminación y restauración de los tableros de Miro. Las empresas pueden establecer plazos de eliminación automática (30, 60, 90, 180 días) para el cumplimiento de los requisitos normativos, equilibrando la retención de datos con la minimización del riesgo empresarial.
- **Retención:** garantiza la protección de datos y su cumplimiento permitiendo a los administradores definir, editar y eliminar políticas adaptadas a las necesidades de su organización. Estas políticas desempeñan un rol crucial en la protección de los tableros de Miro dentro de la organización, permitiéndote conservar ciertos tableros durante un tiempo determinado. [Retention](https://help.miro.com/hc/articles/16855776325778) garantiza que los tableros de Miro no se borren accidental o intencionadamente hasta que el tablero esté fuera del periodo de retención. Aprovechando las políticas de retención, las organizaciones pueden garantizar la protección de los datos, el cumplimiento normativo y la conservación de la información crítica para el negocio.
- ****Eliminación:**** Habilitar limpieza automática de tableros archivándolos y eliminándolos según políticas de retención. [Disposición](../../canvas-25-admin-features/content-lifecycle-management/03-disposition-overview.md) garantiza que los tableros se conserven solo el tiempo necesario y se muevan automáticamente a la Papelera después de un período de inactividad. A partir de ahí, las configuraciones estándar de la papelera determinan quién puede restaurar los tableros y cuándo se eliminarán de forma permanente, fomentando el cumplimiento, la eficiencia operativa y la seguridad de los datos.
- **Gestión de claves de cifrado****(EKM)****:** [EKM](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md) otorga un control centralizado sobre las claves de cifrado, habilitando a las organizaciones para supervisar las actividades relacionadas con las claves y revocar el acceso siempre que sea necesario, garantizando así una capa adicional de seguridad de los datos.
