---
title: "[GitHub] Hola, documentos-como-c\xF3digo!"
article_id: 29239655610258
translation_id: 29239655610258
locale: es
sidebar_position: 2
created_at: '2025-09-04T17:11:12Z'
updated_at: '2026-01-23T15:01:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Esta sección proporciona detalles técnicos y administrativos completos, esenciales para los profesionales de TI y seguridad responsables de la implementación, seguridad y gestión continua de la integración de Trello dentro de su organización.

## Visión técnica general

La integración de Trello se implementa técnicamente a través de una API REST. Para propósitos de autenticación y autorización, la integración utiliza el protocolo estándar de la industria OAuth 2.0. Un componente clave de esta arquitectura es el uso de una plataforma API unificada como subprocesador para datos de terceros. Esta plataforma proporciona APIs unificadas que son responsables de autenticar, normalizar y sincronizar datos a través de varios proveedores de API.

## Flujos de datos

Una comprensión exhaustiva de los flujos de datos es fundamental para gestionar la seguridad y el cumplimiento dentro de tu organización.

### Diagrama de secuencia de alto nivel

Creación de un widget de tarjeta de Trello

![image (7).png](images/32777120091026_image%20(7).png)

Actualización de un widget de tarjeta de Trello

![image (8).png](images/32777120094482_image%20(8).png)

### Datos de Trello en Miro

Cuando los usuarios importan tarjetas de Trello a un tablero de Miro, los datos relevantes de la tarjeta se convierten en parte integral de los datos del lienzo de Miro. Miro almacena los siguientes puntos de datos específicos de las tarjetas importadas, siempre que estén disponibles en Trello:

- Título
- Descripción
- Miembros (incluidos nombres de usuario y correos electrónicos)
- Lista
- Etiquetas

La enumeración explícita de los tipos de datos almacenados es crucial para la gobernanza de datos y el cumplimiento de una organización. Permite a los administradores evaluar con precisión qué información, especialmente cualquier dato potencialmente sensible, está siendo replicada en el entorno de Miro. Esta transparencia garantiza la alineación con las políticas internas de manejo de datos de la organización. También es digno de mención que, según la sección de "Limitaciones", los campos personalizados no son compatibles y por lo tanto no se almacenan, lo cual es un detalle clave para el mapeo de datos y las evaluaciones de cumplimiento. Miro emplea un enfoque híbrido de almacenamiento de datos, minimizando los datos almacenados directamente en el widget de tarjeta y obteniendo detalles adicionales cuando el usuario abre la vista de edición.

### Retención de datos de la información almacenada en Miro

Todos los datos importados de Trello que se almacenen en Miro adhieren estrictamente a la política estándar de retención de datos de Miro. Esta política se aplica de manera consistente a todos los datos de los clientes, asegurando un enfoque uniforme en la gestión del ciclo de vida de los datos.

## Autenticación y autorización

La integración de Trello inicia un flujo de autenticación cuando un usuario interactúa por primera vez con la integración. La autorización dentro de Trello es gestionada por el servicio de integración. Para cada usuario individual, Miro establece una cuenta con el servicio de integración, y estas credenciales se usan posteriormente para todas las interacciones del usuario con la integración.

La integración generalmente requiere la aprobación de un administrador de Trello para autorizar la aplicación de integración dentro del ecosistema de su organización. Además, los usuarios individuales también deben autorizar la integración de Miro con Trello a través de la página de autorización OAuth de Trello cuando intentan insertar un enlace de Trello por primera vez.

### Alcances de autorización requeridos

El alcance de la autorización puede variar dependiendo del sistema de terceros específico. Sin embargo, para integraciones de gestión de tarjetas como Trello, Miro generalmente requiere acceso a los siguientes datos:

| Alcance | Descripción |
| --- | --- |
| Tarjetas (lectura y escritura) | Concede a la integración permiso para leer tarjetas existentes y crear o modificar tarjetas dentro de Trello. |
| Miembros (lectura) | Concede a la integración permiso para leer información de los miembros en Trello, generalmente para asignar tarjetas o mostrar nombres de miembros. |
| Etiquetas (lectura) | Concede a la integración permiso para leer etiquetas asociadas con las tarjetas en Trello. |
| Tableros (lectura) | Concede a la integración permiso para leer información de tableros y listas dentro de Trello. |

### ¿Qué se almacena en Miro y cómo?

Miro almacena de forma segura tanto los datos relacionados con la autorización como aquellos relacionados con el despliegue para la integración Trello:

- **Datos relacionados con la autorización:** Esto abarca los valores de los tokens de acceso y de renovación, los cuales se almacenan en la base de datos de Miro por un tiempo limitado de varios días. Estos tokens se actualizan automáticamente al expirar utilizando el token de renovación para asegurar un acceso continuo. Todos estos datos almacenados en la base de datos para esta integración están cifrados utilizando el Estándar de Cifrado Avanzado de 256 bits, proporcionando una capa robusta de seguridad de datos.
- **Datos relacionados con el despliegue:** Esto incluye los títulos de las tarjetas, que se almacenan como parte de los propios tableros de Miro. Además, los títulos y las referencias cifradas a estos elementos se almacenan en un servicio interno, asegurados adicionalmente a través del cifrado (EKM).

### Revocar un token

Si es necesario, los administradores o usuarios individuales pueden revocar los tokens otorgados a la integración de Trello. Los usuarios pueden navegar a la configuración de la integración ya sea abriendo un selector de tarjetas de integraciones, haciendo clic en el menú de tres puntos en la esquina superior derecha y seleccionando **Configuración de integración**, o accediendo a la pestaña de **Aplicaciones** del equipo en la configuración del equipo de Miro, buscando la integración específica y haciendo clic en ella. En la página de configuración, se puede revocar la autorización al hacer clic en el botón **Desconectar**. Al realizar esta acción, Miro revocará el acceso a Trello y eliminará la cuenta asociada del usuario. Para la desinstalación a nivel de equipo, los administradores pueden seguir los pasos específicos que se detallan en la sección "Solución de problemas y Preguntas frecuentes (Admin)".

## Cómo configurar la integración de Trello

El proceso de configuración de la integración de Miro + Trello involucra pasos distintos para tanto administradores como usuarios, asegurando un despliegue controlado dentro de una organización.

1. **Asegurar cuentas activas:** Antes de iniciar la instalación, asegúrate de que estén disponibles tanto las cuentas activas de Miro como de Trello.
2. **Instalación a nivel de equipo (Acción del admin):**
   - Los administradores pueden necesitar autorizar explícitamente la integración de Trello para su equipo de Miro. Los miembros del equipo solo pueden utilizar la integración si ha sido instalada a nivel de equipo.
   - Un administrador del equipo de Miro puede instalar la aplicación directamente abriendo un tablero de Miro, seleccionando **herramientas Medios e Integraciones (+)**, buscando "Trello" y haciendo clic en **Conectar** para autorizar la integración. Si un administrador de equipo de Miro realiza esta acción, la aplicación se autorizará e instalará automáticamente sin requerir más aprobación administrativa.
3. **Flujo de solicitudes de usuario y aprobación de admin (si corresponde):**
   - En organizaciones donde se requiere un consentimiento administrativo estricto, un usuario no-administrador en un equipo de Miro configurado para la integración con Trello puede pegar un enlace de Trello en un tablero de Miro. Esta acción podría activar un diálogo de "solicitud de instalación de la aplicación" para el usuario, instándolos a buscar la aprobación administrativa.
   - Los administradores designados pueden revisar y aprobar esta solicitud pendiente a través de sus consolas administrativas de Miro o Trello, dependiendo del flujo de consentimiento específico configurado.
4. **Conexión de usuario individual:**
   - Después de que la integración haya sido instalada y autorizada exitosamente a nivel de equipo por un administrador, los usuarios individuales procederán a hacer clic en **Conectar** en el widget de Trello que aparece en el tablero de Miro.
   - Luego, los usuarios serán redirigidos a una página de autorización de Trello donde otorgan a Miro acceso a su cuenta individual de Trello, confirmando así su autorización personal para insertar e interactuar con el contenido.

## Consideraciones de seguridad y cumplimiento

### Restricción de acceso al archivo fuente

Para asegurarse de que el acceso a los datos de Trello insertados permanezca restringido a las mismas personas que en el tablero de origen de Trello, los administradores de la organización de Miro deben mantener controles estrictos sobre el uso compartido del tablero y la exportación de contenido. Si bien la integración principal de Trello respeta los permisos individuales para la interacción en vivo, cualquier exportación o captura de pantalla estática del contenido del tablero podría potencialmente exponer datos a personas no autorizadas si el propio tablero de Miro no está gestionado de manera segura.

### Manejo de errores

La integración está diseñada con un sistema de respuesta amigable en la interfaz y manejo de errores en casos donde las actualizaciones de datos de tarjetas fallan debido a un rechazo por parte de terceros.

### Anexo de procesamiento de datos de Miro (DPA)

Para obtener detalles legales y de cumplimiento completos sobre las prácticas de procesamiento de datos de Miro, los administradores deben consultar el [Anexo de Procesamiento de Datos de Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Resolución de problemas y preguntas frecuentes

### ¿Cómo puedes desactivar la integración (desinstalación a nivel de equipo)?

Un administrador del equipo de Miro puede desinstalar la integración de Trello a nivel de equipo. Esta acción deshabilita la integración para todos los miembros del equipo. Para hacerlo, navega a **Configuración del equipo Aplicaciones e Integraciones**. Encuentra "Trello" o "Gestión de Tarjetas de Trello" en la lista de aplicaciones instaladas, desplázate hacia abajo y haz clic en **Desinstalar para el equipo**.

### ¿Cómo puedes desactivar la integración (desinstalación individual)?

Los usuarios individuales pueden desinstalar la integración por sí mismos. Ve a **Apps & Integraciones** en tu configuración de Miro. Ubica "Trello" o "Gestión de Tarjetas de Trello" y haz clic en **Desinstalar para mí**.

### ¿Qué administradores pueden instalar la integración de Trello para su equipo?

Solo los administradores de equipo de Miro pueden instalar la aplicación directamente. Si un administrador de equipo de Miro pega una URL de Trello en un tablero de Miro, la aplicación se autorizará e instalará automáticamente sin requerir más acciones.

### ¿Cuáles son los requisitos de disponibilidad para la integración de Trello?

La integración de Trello está disponible para los planes Business y Enterprise de Miro. API REST

### ¿Necesitan los administradores autorizar la integración de Trello para su equipo?

Sí, es posible que los administradores deban autorizar la integración de Trello para su equipo de Miro. Los miembros del equipo solo pueden utilizar la integración de Trello si ha sido instalada a nivel de equipo.
