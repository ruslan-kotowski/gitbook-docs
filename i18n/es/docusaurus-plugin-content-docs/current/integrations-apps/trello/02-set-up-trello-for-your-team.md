---
title: Configura Trello para tu equipo
article_id: 30634093325842
translation_id: 30634093325842
locale: es
sidebar_position: 2
created_at: '2025-10-29T15:59:48Z'
updated_at: '2026-02-23T11:40:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

La integración de Trello está implementada técnicamente a través de una API REST. Para fines de autenticación y autorización, la integración utiliza el protocolo estándar de la industria OAuth 2.0. Un componente clave de esta arquitectura es el uso de una plataforma API unificada como subprocesador para datos de terceros. Esta plataforma proporciona APIs unificadas que son responsables de autenticar, normalizar y sincronizar datos a través de diversos proveedores de API.

## Flujos de datos

Una comprensión completa del flujo de datos es fundamental para gestionar la seguridad y el cumplimiento dentro de tu organización.

### Diagrama de secuencia de alto nivel

Creando un widget de tarjeta de Trello

![Trello (BETA) 2.jpg](images/30635006985362_Trello%20(BETA) 2.jpg)

Actualización de un widget de tarjeta de Trello

![Trello (BETA) 2.jpg](images/30635006985362_Trello%20(BETA) 2.jpg)

### Datos de Trello en Miro

Cuando los usuarios importan tarjetas de Trello a un tablero de Miro, los datos relevantes de la tarjeta pasan a ser parte integral de los datos del lienzo de Miro. Miro almacena los siguientes puntos de datos específicos para las tarjetas importadas, siempre que estén disponibles en Trello:

- Título
- Descripción
- Miembros (incluidos nombres de usuario y correos electrónicos)
- Lista
- Etiquetas

La enumeración explícita de tipos de datos almacenados es crucial para la gobernanza de datos de la organización y el cumplimiento. Permite a los administradores evaluar con precisión qué información, particularmente cualquier dato potencialmente sensible, se está replicando en el entorno de Miro. Esta transparencia asegura la alineación con las políticas internas de manejo de datos de su organización. También es notable que, según la sección de "Limitaciones", los campos personalizados no son compatibles y por lo tanto no se almacenan, lo cual es un detalle clave para la creación de mapas de datos y evaluaciones de cumplimiento. Miro emplea un enfoque híbrido para el almacenamiento de datos, minimizando los datos almacenados directamente en el widget de tarjeta y obteniendo detalles adicionales cuando el usuario abre la vista de edición.

### Retención de datos de la información almacenada en Miro

Todos los datos importados desde Trello que se almacenan dentro de Miro se adhieren estrictamente a la política estándar de retención de datos de Miro. Esta política se aplica de manera consistente a todos los datos de los clientes, garantizando un enfoque uniforme para la gestión del ciclo de vida de los datos.

## Autenticación y autorización

La integración de Trello inicia un flujo de autenticación cuando un usuario interactúa por primera vez con la integración. La autorización dentro de Trello la maneja el servicio de integración. Para cada usuario individual, Miro establece una cuenta con el servicio de integración y estas credenciales son posteriormente utilizadas para todas las interacciones del usuario con la integración.

La integración generalmente requiere la aprobación de un administrador de Trello para autorizar la aplicación de integración dentro del ecosistema de su organización. Además, los usuarios individuales también deben autorizar la integración de Miro Trello a través de la página de autorización OAuth de Trello cuando intentan insertar un enlace de Trello por primera vez.

### Alcances necesarios de autorización

El alcance de la autorización puede variar dependiendo del sistema de terceros específico. Sin embargo, para integraciones de gestión de tarjetas como Trello, Miro generalmente requiere acceso a los siguientes datos:

| Alcance | Descripción |
| --- | --- |
| Tarjetas (lectura y escritura) | Otorga a la integración permiso para leer tarjetas existentes y crear o modificar tarjetas dentro de Trello. |
| Usuarios (lectura) | Otorga a la integración permiso para leer información de usuarios dentro de Trello, principalmente para asignar tarjetas o mostrar nombres de miembros. |
| Colecciones (lectura) | Otorga a la integración permiso para leer colecciones, tableros y listas dentro de Trello. |

### Qué se almacena en Miro y cómo

Miro almacena de manera segura tanto los datos relacionados con la autorización como los relacionados con el desglose para la integración de Trello:

- **Datos relacionados con la autorización:** Esto abarca los valores de los tokens de acceso y de renovación, que se almacenan en la base de datos de Miro por un periodo limitado de varios días. Estos tokens se renuevan automáticamente al expirar usando el token de renovación para asegurar un acceso continuo. Todos estos datos almacenados en la base de datos para esta integración están cifrados utilizando el Estándar de Cifrado Avanzado de 256 bits, proporcionando una capa robusta de seguridad de datos.
- **Datos relacionados con la revelación:** Esto incluye los títulos de las tarjetas, que se almacenan como parte de los tableros de Miro. Además, los títulos y las referencias cifradas de estos elementos se almacenan en un servicio interno, aún más asegurados a través del cifrado (EKM).

### Revocación de un token

Si se hace necesario, los administradores o usuarios individuales pueden revocar los tokens otorgados a la integración de Trello. Los usuarios pueden navegar a la configuración de la integración abriendo un "picker" de tarjetas de integraciones, haciendo clic en el menú de tres puntos en la esquina superior derecha y seleccionando **configuración de la integración**, o accediendo a la pestaña **Aplicaciones** en la configuración del equipo de Miro, encontrando la integración específica y haciendo clic en ella. En la página de configuración, se puede revocar la autorización haciendo clic en el botón **Desconectar**. Al realizar esta acción, Miro revocará el acceso a Trello y eliminará la cuenta asociada del usuario. Para desinstalación a nivel de equipo, los administradores pueden seguir los pasos específicos que se detallan en la sección "Soluciones de problemas y preguntas frecuentes (Admin)".

## Cómo configurar la integración de Trello

El proceso de configuración para la integración de Miro + Trello implica pasos distintos tanto para administradores como para usuarios finales, asegurando un despliegue controlado dentro de una organización.

1. **Asegurar cuentas activas:** Antes de iniciar la instalación, asegúrate de que tanto las cuentas activas de Miro como de Trello estén disponibles.
2. **Instalación a nivel de equipo (Acción del admin):**
   - Los administradores pueden necesitar autorizar explícitamente la integración de Trello para su equipo en Miro. Los miembros del equipo solo podrán utilizar la integración si ha sido instalada a nivel de equipo.
   - Un administrador de equipo de Miro puede instalar directamente la aplicación abriendo un tablero de Miro, seleccionando **Herramientas, Medios e Integraciones (+)**, buscando "Trello" y haciendo clic en **Conectar** para autorizar la integración. Si un administrador de equipo de Miro realiza esta acción, la aplicación será automáticamente autorizada e instalada sin requerir más aprobación administrativa.
3. **Flujo de solicitud de usuario y aprobación de admin (si corresponde):**
   - En organizaciones donde se requiere un consentimiento administrativo estricto, un usuario que no sea admin en un equipo de Miro configurado para la integración con Trello puede pegar un enlace de Trello en un tablero de Miro. Esta acción podría desencadenar un diálogo de "solicitud de instalación de aplicación" para el usuario, solicitándole que busque la aprobación administrativa.
   - Los administradores designados pueden entonces revisar y aprobar esta solicitud pendiente a través de sus consolas administrativas de Miro o Trello, dependiendo del flujo de consentimiento específico configurado.
4. **Conexión individual de usuario:**
   - Después de que la integración haya sido instalada y autorizada exitosamente a nivel de equipo por un administrador, los usuarios individuales procederán a hacer clic en **Conectar** en el widget de Trello que aparece en el tablero de Miro.
   - Luego, los usuarios serán redirigidos a una página de autorización de Trello donde otorgarán acceso a Miro a su cuenta de Trello individual, confirmando así su autorización personal para insertar e interactuar con el contenido.

## Consideraciones de seguridad y cumplimiento

### Restricción de acceso al archivo fuente

Para asegurar que el acceso a los datos insertados desde Trello siga restringido a las mismas personas que en el tablero fuente de Trello, los administradores de la organización de Miro deben mantener controles estrictos sobre el uso compartido de tableros y la exportación de contenido. Si bien la integración principal de Trello respeta los permisos individuales para la interacción en vivo, cualquier exportación o captura estática del contenido del tablero podría potencialmente exponer datos a individuos no autorizados si el tablero de Miro no se gestiona de forma segura.

### Manejo de errores

La integración está diseñada con una interfaz de usuario de respaldo y manejo de errores en casos donde la actualización de datos de tarjetas falle debido al rechazo por parte de terceros.

### Anexo de procesamiento de datos de Miro (DPA)

Para obtener detalles legales y de cumplimiento sobre las prácticas de procesamiento de datos de Miro, los administradores deben consultar el [Anexo de Procesamiento de Datos de Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Resolución de problemas y preguntas frecuentes

### ¿Cómo puedes desactivar la integración (desinstalación a nivel de equipo)?

Un administrador de equipo de Miro puede desinstalar la integración de Trello a nivel de equipo. Esta acción deshabilita la integración para todos los miembros del equipo. Para hacerlo, ve a **Configuración del equipo Apps & Integraciones**. Encuentra "Trello" o "Gestión de Tarjetas de Trello" en la lista de aplicaciones instaladas, desplázate hacia abajo y haz clic en **Desinstalar para el equipo**.

### ¿Cómo puedes desactivar la integración (desinstalación individual)?

Los usuarios individuales pueden desinstalar la integración por sí mismos. Navega a **Aplicaciones e integraciones** en tu configuración de Miro. Ubica "Trello" o "Gestión de tarjetas de Trello" y haz clic en **Desinstalar para mí**.

### ¿Qué administradores pueden instalar la integración de Trello para su equipo?

Solo los administradores de equipo de Miro pueden instalar la aplicación directamente. Si un administrador de equipo de Miro pega una URL de Trello en un tablero de Miro, la aplicación se autorizará e instalará automáticamente sin necesidad de más acciones.

### ¿Cuáles son los requisitos de disponibilidad para la integración de Trello?

La integración de Trello está disponible para los planes Business y Enterprise de Miro.

### ¿Necesitan los administradores autorizar la integración de Trello para su equipo?

Sí, los administradores pueden necesitar autorizar la integración de Trello para su equipo en Miro. Los miembros del equipo solo pueden usar la integración de Trello si se ha instalado a nivel de equipo.
