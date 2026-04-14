---
title: Seguridad de admin para Talktrack
article_id: 11148211487378
translation_id: 11148211487378
locale: es
sidebar_position: 8
created_at: '2023-04-24T08:12:36Z'
updated_at: '2025-11-25T16:22:19Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Talktrack permite a los usuarios individuales grabar videos interactivos o recorridos de audio en su tablero de Miro para que puedan compartir sus ideas sin perder tiempo extra en reuniones. Aprende de qué manera Miro garantiza la seguridad y el cumplimiento de nivel empresarial con Talktrack.

> ***Actualizaciones de la IU de Miro en implementación progresiva***
> Miro está mejorando la interfaz de usuario del tablero para que sea más inclusiva e intuitiva e introduciendo una evolución de los proyectos llamada Espacios. El despliegue se producirá gradualmente para todas las cuentas de Miro a lo largo de varias semanas.
>
> En caso de que ya tengas la interfaz de usuario y el diseño de Espacios mejorados, este artículo puede describir los puntos de entrada que han cambiado.
>
> Para ver la documentación más actual, consulta [la nueva interfaz de usuario simplificada de Miro](../../../using-miro/working-on-the-board/02-miro's-new-simplified-user-interface.md).
>
> Este artículo se actualizará cuando se haya completado el lanzamiento.

:::note
Concede acceso a [Talktrack](../../../using-miro/facilitation-tools/asynchronous-tools/02-talktrack-board-recordings.md) para tu organización en la [configuración de Función](../../managing-enterprise-teams-and-content/06-feature-activation.md).
:::

:::note
Puedes conocer los detalles sobre privacidad y seguridad de Talktrack en el [libro blanco de Talktrack para Enterprises de Miro](https://go2.miro.com/rs/228-GPV-835/images/Talktrack_WhitePaper.pdf).
:::

## Seguridad de nivel Enterprise

Miro es el espacio de trabajo online para la innovación empresarial que permite a equipos distribuidos de cualquier tamaño soñar, diseñar y construir el futuro juntos. En la oficina, de forma remota o combinando las dos formas de trabajar, tus equipos pueden usar Miro para cualquier caso de uso en la empresa.

Pero eso conlleva una gran responsabilidad, por eso nos tomamos la seguridad tan en serio como la colaboración, para ayudarte a mantener tus ideas protegidas.

|  |  |  |
| --- | --- | --- |
| **Checkmark.png**  **Aprobado y certificado** | **Security_lock.png**  **Protección de confianza** | **Fingerprint.png**  **Gestión de acceso segura** |
| Las mejores prácticas y requisitos reglamentarios de la industria | Protege y gestiona tu propiedad intelectual | Controla quién puede acceder y administrar tu contenido de Miro |

## Aprobado y certificado

Miro sigue las mejores prácticas y los requisitos normativos de la industria, incluidos [ISO 27001, SOC2 Tipo II y SOC3](https://miro.com/trust/compliance/). También nos aseguramos de que tu infraestructura y servicios cumplan con los estándares del RGPD, lo que incluye las grabaciones de Talktrack.

**Gestión del ciclo de vida del contenido**

**Eliminación de Talktrack**
**Eliminar un Talktrack:** Cuando se elimina un Talktrack, no se puede restaurar.

**Eliminar un tablero:** Los Talktracks son grabaciones en capas que brindan contexto a un tablero. Si se elimina un tablero, sus Talktracks también se eliminarán. Sin embargo, si un admin recupera un tablero eliminado en un plazo de 90 días, los Talktracks del tablero también se restaurarán. Lee más sobre [eliminación de tableros](../../../using-miro/managing-boards/07-how-to-delete-a-board.md).

**Privacidad**

**Datos capturados cuando se graba un Talktrack:** los movimientos del cursor de quien está grabando y el visualizador del tablero de Miro, el contenido del tablero en el momento en que se creó el Talktrack, el video de quien está grabando, ya sea la vista de su cámara o su avatar, en función de si la cámara está activada o desactivada, el audio de quien está grabando desde la fuente de audio seleccionada y cualquier otro audio que esté presente en el mismo espacio físico que el presentador.

**Datos no capturados cuando se graba un Talktrack:** el cursor o la información de cualquier otro usuario que haya accedido al tablero en el momento de la grabación, la pantalla de quien está grabando o los sonidos de la computadora.

**Aviso de privacidad**

La base legal para procesar datos personales relacionados con Talktrack, en la que Miro es el controlador (básicamente de metadatos) son la ejecución de un contrato (en el caso de los usuarios de autoservicio) y/o los intereses legítimos (de todos los usuarios). El cliente es el controlador de los datos registrados con Talktrack. La base legal del cliente es para que este la evalúe y probablemente sean intereses legítimos.

**Accesibilidad**

Talktrack te permite navegar con el teclado y ofrece soporte para transcripciones automáticas y subtítulos.

**Observabilidad**

[Los registros de auditoría](../../security-integrations/security-management/01-audit-logs.md) están disponibles para Talktrack en la configuración del admin. Tenemos integraciones con los siguientes sistemas SIEM (administración de información y eventos de seguridad):
[Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md)
[IBM QRadar](../../security-integrations/security-information-and-event-management-siem/02-miro-connector-for-ibm-qradar.md)

**Auditoría externa**

Miro emplea las mejores firmas de consultoría externa para realizar auditorías anuales. Nuestra certificación ISO 27001 actual está firmada por BSI (British Standard Institution), del Reino Unido, y los informes SOC2 y SOC3 por KirkpatrickPrice, de Estados Unidos. Lee más sobre el [cumplimiento en Miro](https://miro.com/trust/compliance/).

## Protección de confianza

Protege y gestiona la propiedad intelectual creada o agregada a nuestra plataforma. Tus datos están cifrados con el protocolo TLS 1.3 cuando están en tránsito y con el algoritmo AES 256 cuando están inactivos.

**Cifrado**

Los datos en Miro, incluidos los datos de Talktrack, están cifrados de forma predeterminada cuando están inactivos con el algoritmo AES256 y en tránsito con el protocolo TLS1.3. Lee más en nuestro [Documento técnico sobre cifrado de Miro](https://go2.miro.com/rs/228-GPV-835/images/Encryption%20Whitepaper.pdf).

**Clasificación de datos**

La [etiqueta de clasificación del tablero](../../canvas-25-admin-features/data-security/02-data-classification.md) no está visible mientras ves o grabas un Talktrack.

**Gestión de claves de cifrado**

Si tu organización tiene configurada y desplegada la [gestión de claves de cifrado](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md) (EKM), los admins pueden solicitar que Miro use la clave de cifrado de tu organización para el contenido de Talktrack.

**Residencia de datos**

Por defecto, los datos de Talktrack se almacenan en la misma ubicación que el resto de los datos de contenido del cliente en Miro: en servidores de AWS ubicados en la UE. Miro ofrece un mayor nivel de control y cumplimiento sobre los datos de tu empresa al garantizar que todo tu contenido de cliente esté alojado en Europa. Para los clientes que han solicitado la [residencia de datos en EE. UU.](../../canvas-25-admin-features/data-security/09-us-data-center-residency.md), los datos de Talktrack se almacenan en nuestro centro de datos principal en Ohio y en el centro de datos de respaldo en Virginia.

## Administración de acceso seguro

Controla quién puede acceder a Miro con funciones de nivel Enterprise, aprovechando funcionalidades avanzadas de identidad y capacidades administrativas. Lee más sobre las características de seguridad y cumplimiento del plan Enterprise [aquí](../../../administration/security-compliance).

**Controlar el acceso de tu organización a Talktrack**

Los admins de empresa pueden otorgar o revocar el acceso a Talktrack para toda la empresa o para equipos específicos desde sus [preferencias de acceso a funciones](../../managing-enterprise-teams-and-content/06-feature-activation.md).

**Acceso para grabar un Talktrack**

La opción para [grabar un Talktrack](../../../using-miro/facilitation-tools/asynchronous-tools/02-talktrack-board-recordings.md) está disponible para usuarios que tienen acceso de comentario o edición en un tablero, o que son propietarios o copropietarios del tablero.

**Acceso para ver un Talktrack**

La reproducción del Talktrack está disponible para todos los usuarios que tienen [acceso al tablero](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Preguntas frecuentes

¿El admin de empresa puede ver qué tableros tienen Talktracks?

Solo puedes ver si un tablero tiene un Talktrack cuando lo abres. Si el tablero no está compartido contigo, puedes usar [permisos de admin de contenido](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) para obtener acceso y ver el Talktrack.

¿Cómo desactivo Talktrack para mi empresa o equipo?

Para desactivar Talktrack, ve a tus [preferencias de acceso a funciones](../../managing-enterprise-teams-and-content/06-feature-activation.md) y selecciona **Nadie puede usar**, o elimina el acceso de equipos específicos haciendo clic en **X** junto al nombre del equipo.

¿Qué sucede con los Talktracks existentes cuando un admin revoca el acceso a la función de Talktrack?

Los Talktracks existentes permanecerán disponibles, pero no se podrán grabar nuevos Talktracks.

¿Los admins pueden eliminar Talktracks?

Los admins pueden compartir un tablero consigo mismos en los [permisos de admin de contenido](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), y luego eliminar el Talktrack del tablero.

¿Los nombres de los usuarios se muestran en la aplicación o se guardan con los datos del Talktrack?

Talktrack muestra el nombre (nombre y apellido o nombre para mostrar, según la disponibilidad) durante la reproducción y como el "nombre del grabador". Sin embargo, Talktrack solo guarda los IDs de usuario, por lo que no se guarda información personal con la grabación. Si el usuario no forma parte de la organización durante la reproducción, el nombre mostrado aparecerá como "Usuario desconocido".
