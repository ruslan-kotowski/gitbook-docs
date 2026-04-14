---
title: "Gu\xEDa de implantaci\xF3n de Enterprise Guard: Presentaci\xF3n"
article_id: 17120515162386
translation_id: 17120515162386
locale: es
sidebar_position: 0
created_at: '2024-02-19T09:17:20Z'
updated_at: '2025-11-25T15:40:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Este documento te guiará en el despliegue del producto de seguridad avanzada de Miro, Enterprise Guard, detallando las mejores prácticas tanto para la configuración como para la habilitación del usuario final. Si tienes alguna pregunta relacionada con el contenido de esta guía, ponte en contacto con tu equipo de cuentas Miro.

## Cómo utilizar esta guía

- Navega de una sección a otra utilizando el esquema de la parte izquierda de tu pantalla
- Utiliza la guía junto con la documentación de funciones enlazada a lo largo de
- Personaliza las plantillas proporcionadas para ahorrar tiempo habilitando a tus usuarios

## Esquema de la guía

- [Parte 1 | Configurar roles de admins](02-enterprise-guard-deployment-guide-part-1-configure-admin-roles.md)
- [Parte 2 | Despliega la Seguridad de los Datos](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md)
- [Parte 3 | Gestionar el ciclo de vida del contenido](04-enterprise-guard-deployment-guide-part-3-manage-content-lifecycle.md)

## Por qué necesitas Enterprise Guard

Miro es el espacio de trabajo en línea para la innovación, preparado para las empresas, que transforma la forma de trabajar de los equipos distribuidos de cualquier tamaño.

Hemos visto un aumento en la cantidad de trabajo estratégico que se realiza en Miro, y con este crecimiento hay aún más contenido que necesita protección y gobierno.

Los datos sensibles aparecen donde los clientes menos se lo esperan. Basándonos en un muestreo de 100 empresas clientes, descubrimos que el 62% de ellas tenían tableros que contenían datos sensibles, como información de identificación personal, información sanitaria personal e información de tarjetas de crédito. Esta superficie de riesgo no hace más que aumentar, ya que el número de tableros de nuestros clientes empresariales crece un 250% cada año.

Este crecimiento del contenido hace aún más difícil intentar gestionar los riesgos estrictamente mediante las herramientas tradicionales existentes o confiando en que los empleados se adhieran a las políticas de la empresa.

Enterprise Guard es el complemento avanzado de Miro para la seguridad y gobernanza de datos. Las organizaciones pueden encontrar y proteger contenido sensible, y gestionar ciclos de vida del contenido, automáticamente y a escala.

## Presentamos Enterprise Guard: una solución integral de seguridad y gobernanza para Miro

Consciente de estos retos, Miro presenta **Enterprise Guard**, un complemento avanzado de seguridad y gobernanza. Enterprise Guard ofrece un conjunto de funciones que permiten a las empresas identificar, clasificar, proteger y gestionar eficazmente el contenido confidencial en los tableros de Miro. Esta solución está adaptada para garantizar el cumplimiento normativo y una sólida protección de datos a escala.

Con la integración de Enterprise Guard en el ecosistema empresarial de Miro, las empresas pueden aprovechar ahora un marco de seguridad más sólido, automatizado y completo. Este complemento no trata solo de proteger los datos, sino de habilitar a las empresas para que sigan innovando y colaborando en Miro de forma segura, sin obstaculizar las operaciones de la empresa.

## Versión de disponibilidad general de Enterprise Guard: funciones principales

![Funciones principales de la versión de disponibilidad general de Enterprise Guard](images/26240574186898_Enterprise-Guard-Data-Security.png)

- **Descubrimiento de datos:** Enterprise Guard habilita un proceso proactivo y minucioso de descubrimiento de datos, crucial para identificar datos sensibles tales como números de tarjetas de crédito, números de seguridad social y otra información crítica dispersa por varios tableros de Miro. Esta estrategia proactiva es esencial para identificar y mitigar las vulnerabilidades potenciales, ayudando a prevenir las violaciones de datos y a garantizar el cumplimiento.
- eDiscovery Habilita la conservación, el seguimiento y la exportación seguros de los datos de los tableros para habilitar los requisitos legales, de cumplimiento y de seguridad. La función de eDiscovery de Enterprise Guard ayuda a las empresas a cumplir las obligaciones normativas mediante las funciones de [Retenciones legales](../../canvas-25-admin-features/ediscovery/02-legal-hold-overview.md), [Registros de contenido](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md) y [Exportación de tableros](../../canvas-25-admin-features/ediscovery/13-board-export-api-overview.md).

  Las Retenciones Legales evitan la eliminación permanente de contenido relevante para investigaciones o asuntos legales, conservando todos los tableros con los que interactúa un usuario retenido, incluidas todas sus versiones. Los Registros de contenido proporcionan registros detallados de la actividad de los usuarios, que pueden exportarse e integrarse en herramientas externas de auditoría o revisión legal. Con las API de eDiscovery, los clientes de empresas también pueden exportar datos de tableros a escala, garantizando que la información crítica sea accesible para los flujos de trabajo legales y de cumplimiento.
- **Clasificación automática:** establece criterios para que Miro clasifique automáticamente tus tableros en función de los datos sensibles que contengan.
- ****Barreras de protección inteligentes:**** aplica normas de seguridad en tiempo real y restringe lo que los usuarios pueden hacer con un tablero, como restringir las capacidades de replicación y uso compartido del contenido del tablero en varios niveles (público, equipo, organización), en función de la clasificación manual o automatizada del tablero. Esto garantiza la privacidad y el cumplimiento de las normas sin obstaculizar las operaciones de la empresa.
- **Política papelera:** la política de papelera de Enterprise Guard ofrece un mayor control sobre la eliminación y restauración de los tableros de Miro. Las empresas pueden establecer plazos de eliminación automática (30, 60, 90, 180 días) para el cumplimiento de los requisitos normativos, equilibrando la retención de datos con la minimización del riesgo empresarial.
- **Retención:** garantiza la protección de datos y su cumplimiento permitiendo a los administradores definir, editar y eliminar políticas adaptadas a las necesidades de su organización. Estas políticas desempeñan un rol crucial en la protección de los tableros de Miro dentro de la organización, permitiendo conservar determinados tableros durante un periodo de tiempo determinado. La retención garantiza que los tableros de Miro no se borren accidental o intencionadamente hasta que el tablero esté fuera del periodo de retención. Aprovechando las políticas de retención, las empresas pueden garantizar la protección de los datos, el cumplimiento y la conservación de la información crítica para la empresa.
- eliminación Habilita la limpieza automática de tableros archivándolos y eliminándolos según las políticas de retención. [La eliminación](../../canvas-25-admin-features/content-lifecycle-management/03-disposition-overview.md) garantiza que los tableros se conserven sólo el tiempo necesario y se muevan automáticamente a la Papelera tras un periodo de inactividad. A partir de ahí, la configuración estándar de la papelera determina quién puede restaurar los tableros y cuándo se eliminarán definitivamente, lo que favorece el cumplimiento, la eficacia operativa y la seguridad de los datos.
- ****Gestión de claves de cifrado** **(EKM):**** EKM otorga un control centralizado sobre las claves de cifrado, habilitando a las organizaciones para supervisar las actividades relacionadas con las claves y revocar el acceso siempre que sea necesario, garantizando así una capa adicional de seguridad de los datos.
