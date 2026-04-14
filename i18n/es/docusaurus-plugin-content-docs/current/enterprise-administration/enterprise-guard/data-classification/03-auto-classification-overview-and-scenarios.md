---
title: "Descripci\xF3n general y casos de clasificaci\xF3n autom\xE1tica"
article_id: 15431302000914
translation_id: 15431302000914
locale: es
sidebar_position: 2
created_at: '2023-11-29T16:42:42Z'
updated_at: '2025-11-25T15:39:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Para respaldarte con la protección del contenido sensible, Enterprise Guard incluye la función de clasificación automática, un proceso de clasificación de datos automatizado que ordena los tableros de Miro en función del nivel de su contenido sensible. La clasificación automática representa un avance significativo en la forma en que administras y proteges tus datos sensibles. Automatizar el proceso de clasificación le permite a tu organización mantener un nivel de seguridad de datos más alto, cumplir con los requisitos normativos y brindar una mejor experiencia de admin de seguridad. La transición de la clasificación manual a la automática es un movimiento estratégico hacia un marco de seguridad de datos más preciso, seguro y eficaz.

## Descripción de casos de clasificación automática

### Requisitos previos

Para usar la función de clasificación automática, debes:

- [Habilitar el descubrimiento de datos](../data-discovery/13-activate-privacy-related-data-discovery.md).
- [Definir los niveles de clasificación](07-define-classification-levels.md).

### Ejemplo de configuración de clasificación automática y barreras de protección

Debes [configurar la clasificación automática y las barreras de protección](https://help.miro.com/hc/articles/15853672236946) según tus requisitos de seguridad y gobernanza. La siguiente tabla enumera la configuración utilizada para todos los casos de ejemplo de esta página y tiene solo fines explicativos.

|  |  |  |  |
| --- | --- | --- | --- |
| **Clasificación del tablero** | **Orden de sensibilidad** | **Criterios de clasificación automática** | **Barreras de protección** |
| PÚBLICO | 1  (menos sensible) | Ninguno | Ninguna |
| INTERNO (predeterminado) | 2 | TELECOM | - Bloquear el uso compartido público |
| CONFIDENCIAL | 3 | RGPD  PCI DSS | - Bloquear el uso compartido público  - Bloquear el uso compartido con equipos |
| RESTRINGIDO | 4 (más sensible) | HIPAA  CREDENCIALES | - Bloquear el uso compartido público  - Bloquear el uso compartido con equipos  - Bloquear el uso compartido con la organización |

*Tabla 1: Configuración de ejemplo solo con fines explicativos.*

## Actualización manual de la clasificación de tableros para anular la clasificación automática

Solo los propietarios, copropietarios o editores del tablero pueden actualizar la clasificación del tablero para anular el nivel de Clasificación automática. Si el propietario, los copropietarios o los editores de un tablero actualizan su clasificación a un nivel menos sensible, deben seleccionar o proporcionar un motivo para el cambio y esta información se agrega a los registros de auditoría.

### Actualizar manualmente a un nivel de clasificación sensible inferior

**Caso**
Piensa en una situación en la que Juan Pérez es el propietario de un tablero que se clasificó automáticamente como **Confidencial**, que tiene el orden de sensibilidad **3** según nuestra configuración.

Juan analiza la información y decide actualizar el nivel de clasificación a **Interno**, que tiene el nivel de sensibilidad **2**, un nivel inferior comparado con la clasificación automática del tablero (**Confidencial**, nivel **3**).

:::note
Solo los propietarios, copropietarios o editores del tablero pueden actualizar manualmente el nivel de clasificación.
:::

**Resultado**

Como Juan es el propietario del tablero, puede actualizarlo a un nivel de clasificación sensible inferior: **Interno**, nivel **2**. En este caso, se le solicita a Juan el motivo por el que quiere cambiar el nivel de clasificación del tablero a uno menos sensible (figura 1). Juan puede seleccionar el motivo y hacer clic en **Actualizar**.

El nivel de clasificación del tablero se actualiza y la información sobre esta actualización se agrega a los registros de auditoría.

### Actualizar manualmente a un nivel de clasificación sensible superior

**Caso**

Piensa en una situación en la que Juan Pérez es el propietario de un tablero que se clasificó automáticamente como **Confidencial**, que tiene el orden de sensibilidad **3** según nuestra configuración.

Juan analiza la información y decide actualizar el nivel de clasificación a **Restringido**, que tiene el nivel de sensibilidad más alto (**4**), un nivel superior comparado con la clasificación automática del tablero (**Confidencial**, nivel **3**).

:::note
Solo los propietarios, copropietarios o editores del tablero pueden actualizar manualmente el nivel de clasificación.
:::

**Resultado**

Como Juan es el propietario del tablero, puede actualizarlo a un nivel de clasificación sensible superior.

La siguiente tabla resume diversos casos y sus resultados, considerando que el tablero se autoclasificó en algún momento anterior y que luego el propietario, copropietario o editor actualizó manualmente la clasificación.

|  |  |  |
| --- | --- | --- |
| **Nivel de clasificación automática** | **Acción del propietario del tablero** | **Nuevo nivel de clasificación** |
| CONFIDENCIAL | **Actualización a un nivel de clasificación inferior**  Juan, el propietario del tablero, actualiza manualmente la clasificación a  **INTERNO**, que tiene un nivel de sensibilidad 2, un nivel inferior comparado con el que le otorgó la clasificación automática (CONFIDENCIAL, nivel 3). | Como Juan es el propietario del tablero, puede actualizarlo a un nivel de clasificación sensible inferior, **INTERNO**.  En este caso, se le solicita al propietario el motivo por el que quiere cambiar el nivel de clasificación del tablero a uno menos sensible. Juan puede seleccionar el motivo y hacer clic en **Actualizar**.  El nivel de clasificación del tablero se actualiza a **INTERNO** y la información sobre esta actualización se agrega a los registros de auditoría. |
| CONFIDENCIAL | **Actualización a un nivel de clasificación superior**  Juan, el propietario del tablero, decide actualizar su clasificación a **RESTRINGIDO**, que tiene el nivel de sensibilidad más alto (4), un nivel superior comparado con la clasificación automática del tablero (CONFIDENCIAL, nivel 3). | Como Juan es el propietario del tablero, puede actualizarlo a un nivel de clasificación sensible superior. |

*Tabla 2: Casos y niveles de clasificación automática resultantes*

## Actualización automática de la clasificación del tablero

El ciclo de descubrimiento de datos se ejecuta cada hora. Si el contenido de un tablero cambia, ya sea que se agreguen o eliminen datos altamente sensibles, los tableros con estas actualizaciones se volverán a clasificar automáticamente, en función del contenido actualizado del tablero y del último nivel de clasificación no automática. Las siguientes secciones proporcionan escenarios de ejemplo para las actualizaciones automáticas del nivel de clasificación.

### Datos de alta sensibilidad eliminados del tablero

Una vez que se completa el siguiente ciclo de descubrimiento de datos, la clasificación del tablero se actualiza automáticamente al nivel de sensibilidad correspondiente.

**Ejemplo de escenario del contenido del tablero**

El tablero contiene datos altamente sensibles que incluían información que pertenecía a las siguientes etiquetas de sensibilidad: CREDENCIALES, HIPAA, RGPD o PCI DSS. Por lo tanto, una vez que se completa el ciclo de descubrimiento de datos, la clasificación automática otorga la et**iqueta REST**RINGIDO, nivel 4, que es el orden de sensibilidad más alto según nuestra configuración de clasificación automática de ejemplo. La tabla a continuación describe lo siguiente:

- **Última clasificación no automática:** la última clasificación no automática del tablero que podría haberse realizado [manualmente](03-auto-classification-overview-and-scenarios.md), a través de una [clasificación predeterminada de tableros](../data-security/02-data-classification.md) o mediante las API de [actualización de clasificación de tableros](https://developers.miro.com/reference/enterprise-dataclassification-board-set)/[actualización masiva de clasificación de tableros](https://developers.miro.com/reference/enterprise-dataclassification-team-boards-bulk).

- **Clasificación automática:** el nivel que la clasificación automática aplicó al tablero una vez completado el ciclo de descubrimiento de datos.

- **Acción realizada:** las actualizaciones realizadas al contenido del tablero después de la clasificación automática.

- **Nueva clasificación:** la nueva clasificación teniendo en cuenta la acción realizada y todos los demás aspectos, como el contenido del tablero y la última clasificación no automática.

|  |  |  |  |
| --- | --- | --- | --- |
| **Última clasificación no automática** | **Clasificación automática** | **Acción del usuario** | **Nuevo nivel de clasificación aut**omática |
| Interno (mediante la clasificación predeterminada de tableros) | RESTRINGIDO | Todos los datos sensibles eliminados del tablero | Una vez que se completa el ciclo de descubrimiento de datos, la clasificación del tablero se actualiza automáticamente al nivel **INTERNO**, porque el tablero ya no contiene información sensible, pero la clasificación no automática anterior era INTERNO, asignada mediante la clasificación predeterminada. |
| CONFIDENCIAL | RESTRINGIDO | Todos los datos sensibles eliminados del tablero | Una vez que se completa el ciclo de descubrimiento de datos, la clasificación del tablero se actualiza automáticamente al nivel **CONFIDENCIAL**, orden de sensibilidad 3, incluso si el tablero ya no contiene información sensible porque el nivel de clasificación no automática anterior era CONFIDENCIAL, nivel 3. |
| NO CLASIFICADO | RESTRINGIDO | CREDENCIALES e HIPAA, que son de nivel RESTRINGIDO, orden de sensibilidad 4, el contenido se elimina del tablero. | Una vez que se completa el ciclo de descubrimiento de datos, la clasificación del tablero se actualiza automáticamente al nivel **CONFIDENCIAL**, orden de sensibilidad 3, ya que:  - el tablero ya no contiene información de CREDENCIALES ni de HIPAA, pero aún contiene datos sensibles de PCI DSS, que se asignan al nivel **CONFIDENCIAL**. - el tablero no se había clasificado antes de la clasificación automática. |
| RESTRINGIDO | RESTRINGIDO | CREDENCIALES e HIPAA, que son de nivel RESTRINGIDO, orden de sensibilidad 4, el contenido se elimina del tablero. | Una vez que se completa el ciclo de descubrimiento de datos, el tablero permanece en el nivel **RESTRINGIDO**, orden de sensibilidad 4, incluso si ya no contiene ninguna información de CREDENCIALES ni de HIPAA, porque el nivel de clasificación no automática anterior era RESTRINGIDO, nivel 4. |
| NO CLASIFICADO | RESTRINGIDO | Todos los datos sensibles eliminados del tablero | Una vez que se completa el ciclo de descubrimiento de datos, la clasificación del tablero se actualiza automáticamente al nivel **NO CLASIFICADO**, porque ya no contiene información sensible y no se había clasificado antes de la clasificación automática. |

*Tabla 3: Casos y niveles de clasificación automática resultantes*

### Datos de alta sensibilidad agregados al tablero

Una vez que se completa el ciclo de descubrimiento de datos, la clasificación del tablero se actualiza automáticamente al nivel de sensibilidad correspondiente según el nivel más alto de datos sensibles encontrados.

|  |  |  |
| --- | --- | --- |
| **Último nivel de clasificación automática** | **Acción del usuario** | **Nuevo nivel de clasificación aut**omática |
| PÚBLICO | El colaborador agregó un número de tarjeta de crédito. | **CONFIDENCIAL** PCI DSS |
| Interno | El colaborador agregó un token de autenticación. | **RESTRINGIDO** CREDENCIALES |
| RESTRINGIDO | El colaborador agregó un token de autenticación. | **RESTRINGIDO** Permanece igual. |
| Interno | El colaborador agregó un número de licencia de conducir de Alemania. | **CONFIDENCIAL**  RGPD |
| CONFIDENCIAL | El colaborador agregó una dirección MAC. | **RESTRINGIDO**  CREDENCIALES |

*Tabla 4: Casos y niveles de clasificación automática resultantes*
