---
title: Configura Asana para tu equipo
article_id: 28252196453778
translation_id: 28252196453778
locale: es
sidebar_position: 2
created_at: '2025-07-22T13:30:20Z'
updated_at: '2026-02-20T09:00:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Esta sección proporciona detalles técnicos y administrativos completos, esenciales para los profesionales de IT y seguridad responsables del despliegue, la seguridad y la gestión continua de la integración de Asana dentro de su organización.

## Visión general técnica

La integración de Asana se implementa técnicamente a través de una REST API. Para fines de autenticación y autorización, la integración utiliza el protocolo estándar de la industria OAuth 2.0. Un componente clave de esta arquitectura es la utilización de una plataforma API unificada como subprocesador para datos de terceros. Esta plataforma proporciona APIs unificadas responsables de autenticar, normalizar y sincronizar datos a través de varios proveedores de API.

## Flujo de datos

Comprender a fondo el flujo de datos es fundamental para gestionar la seguridad y el cumplimiento dentro de tu organización.

### Diagrama de secuencia de alto nivel

Crear una tarjeta de Asana

![image (7).png](images/30597091618834_image%20(7).png)

Actualizar una tarjeta de Asana

![image (8).png](images/30597112699922_image%20(8).png)

### Datos de Asana en Miro

Cuando los usuarios importan tareas de Asana en un tablero de Miro, los datos relevantes de las tareas se convierten en parte integral de los datos del lienzo de Miro. Miro almacena los siguientes puntos de datos específicos para las tareas importadas, siempre que estén disponibles en Asana:

- Título
- Descripción
- Asignado a (incluyendo el nombre y/o correo electrónico del usuario)
- Estado
- Prioridad

La enumeración explícita de los tipos de datos almacenados es crucial para la gobernanza de datos y el cumplimiento organizacional. Permite a los administradores evaluar con precisión qué información, particularmente cualquier dato confidencial, se está replicando en el entorno de Miro. Esta transparencia asegura la alineación con las políticas internas de manejo de datos de la organización. También es importante señalar que, según la sección "Limitaciones", los campos personalizados no son compatibles y, por lo tanto, no se almacenan, lo cual es un detalle clave para la creación de mapas y las evaluaciones de cumplimiento. Miro emplea un enfoque híbrido para el almacenamiento de datos, minimizando los datos almacenados directamente en el widget de la tarjeta y obteniendo detalles adicionales cuando el usuario abre la vista de edición.

### Retención de datos de la información almacenada en Miro

Todos los datos importados de Asana que se almacenan en Miro adhieren estrictamente a la política estándar de retención de datos de Miro. Esta política se aplica de manera consistente en todos los datos de los clientes, asegurando un enfoque uniforme para la gestión del ciclo de vida de los datos.

## Autenticación y autorización

La integración de Asana inicia un flujo de autenticación cuando un usuario interactúa por primera vez con la integración. La autorización dentro de Asana es gestionada por el servicio de integración. Para cada usuario individual, Miro establece una cuenta con el servicio de integración, y estas credenciales se utilizan posteriormente para todas las interacciones del usuario con la integración.

La integración generalmente requiere la aprobación de un administrador de Asana (o de un administrador de Microsoft Entra, si Asana se gestiona a través de Azure AD) para autorizar la aplicación de integración dentro del ecosistema de su organización. Además, los usuarios individuales también deben autorizar la integración de Miro Asana a través de la página de autorización OAuth de Asana cuando intenten insertar un enlace de Asana por primera vez.

### Alcances de autorización requeridos

El alcance de la autorización puede variar según el sistema de terceros específico. Sin embargo, para integraciones de gestión de tickets como Asana, Miro generalmente requiere acceso a los siguientes datos:

| Alcance | Descripción |
| --- | --- |
| Tareas (lectura y escritura) | Otorga a la integración permiso para leer tareas existentes y crear o modificar tareas dentro de Asana. |
| Usuarios (lectura) | Otorga a la integración permiso para leer información de usuarios dentro de Asana, típicamente para asignar tareas o mostrar nombres de los asignados. |
| Etiquetas (lectura) | Otorga a la integración permiso para leer etiquetas asociadas con tareas en Asana. |
| Colecciones (lectura) | Otorga a la integración permiso para leer colecciones de tareas o proyectos dentro de Asana. |

### ¿Qué se almacena en Miro y cómo?

Miro almacena de manera segura tanto datos relacionados con autorización como datos relacionados con la presentación de la integración de Asana:

- **Datos relacionados con la autorización:** Esto abarca tokens de acceso y valores de token de actualización, que se almacenan en la base de datos de Miro durante un tiempo limitado de varios días. Estos tokens se actualizan automáticamente al expirar utilizando el token de actualización para asegurar un acceso continuo. Todos estos datos almacenados dentro de la base de datos para esta integración están cifrados usando el Estándar de Cifrado Avanzado de 256 bits, proporcionando una capa robusta de seguridad de datos.
- **Datos relacionados con el despliegue de contenido:** Esto incluye los títulos de las tareas, que se almacenan como parte de los tableros de Miro. Además, los títulos y las referencias cifradas a estos elementos se almacenan en un servicio interno, asegurados adicionalmente a través del cifrado (EKM).

### Revocación de un token

Si es necesario, los administradores o los usuarios individuales pueden revocar los tokens otorgados a la integración de Asana. Los usuarios pueden navegar a la configuración de la integración ya sea abriendo un selector de tareas de integraciones, haciendo clic en el menú de tres puntos en la esquina superior derecha y seleccionando **Parámetros de Configuración de la Integración**, o accediendo a la pestaña **Aplicaciones** del equipo en la configuración del equipo de Miro, encontrando la integración específica y haciendo clic en ella. En la página de configuración, se puede revocar la autorización haciendo clic en el botón **Desconectar**. Tras esta acción, Miro revocará el acceso a Asana y eliminará la cuenta asociada del usuario. Para la desinstalación a nivel de equipo, los administradores pueden seguir los pasos específicos descritos en la sección "Solución de problemas y preguntas frecuentes (Admin)".

## Cómo configurar la integración de Asana

El proceso de configuración de la integración Miro + Asana involucra pasos distintos tanto para administradores como para usuarios, asegurando un despliegue controlado dentro de una organización.

1. **Asegurar cuentas activas:** Antes de iniciar la instalación, asegúrate de que estén disponibles cuentas activas tanto de Miro como de Asana.
2. **Instalación a nivel de equipo (Acción del Admin):**
   - Es posible que los administradores deban autorizar explícitamente la integración de Asana para su equipo de Miro. Los miembros del equipo solo podrán utilizar la integración si se ha instalado a nivel de equipo.
   - Un administrador de equipo de Miro puede instalar directamente la aplicación abriendo un tablero de Miro, seleccionando **Herramientas Medios & Integraciones (+)**, buscando "Asana" y haciendo clic en **Conectar** para autorizar la integración. Si un administrador de equipo de Miro realiza esta acción, la aplicación se autorizará e instalará automáticamente sin requerir más aprobación administrativa.
3. **Solicitud del usuario y flujo de aprobación de admin (si corresponde):**
   - En organizaciones donde se requiere un consentimiento administrativo estricto, un usuario no administrador en un equipo de Miro configurado para la integración con Asana puede pegar un enlace de Asana en un tablero de Miro. Esta acción podría desencadenar un diálogo de "solicitud de instalación de la aplicación" para el usuario, instándolos a buscar la aprobación administrativa.
   - Los administradores designados pueden entonces revisar y aprobar esta solicitud pendiente a través de sus consolas administrativas de Miro o Asana, dependiendo del flujo de consentimiento específico configurado.
4. **Conexión de usuario individual:**
   - Después de que la integración ha sido instalada y autorizada a nivel de equipo por un administrador, los usuarios individuales procederán a hacer clic en **Conectar** en el widget de Asana que aparece en el tablero de Miro.
   - Luego, los usuarios serán redirigidos a una página de autorización de Asana donde otorgan a Miro acceso a su cuenta individual de Asana, confirmando así su autorización personal para insertar e interactuar con contenido.

## Consideraciones de seguridad y cumplimiento

### Restricción de acceso al archivo fuente

Para garantizar que el acceso a los datos de Asana insertados permanezca restringido a las mismas personas que en el archivo fuente de Asana, los administradores de la organización de Miro deben mantener un control estricto sobre el uso compartido de tableros y la exportación de contenido. Aunque la integración principal de Asana respeta los permisos individuales para la interacción en vivo, cualquier exportación o captura estática del contenido del tablero podría potencialmente exponer los datos a personas no autorizadas si el tablero de Miro no se gestiona de manera segura.

### Manejo de errores

La integración está diseñada con un fallback de interfaz de usuario elegante y manejo de errores en casos donde las actualizaciones de datos de tarjetas fallan debido a rechazo por terceros.

### Anexo de procesamiento de datos de Miro (DPA)

Para obtener detalles legales y de cumplimiento sobre las prácticas de procesamiento de datos de Miro, los administradores deben consultar el [Anexo de Procesamiento de Datos de Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Resolución de problemas y preguntas frecuentes

### ¿Cómo se puede desactivar la integración (desinstalación a nivel equipo)?

Un administrador del equipo de Miro puede desinstalar la integración con Asana a nivel de equipo. Esta acción deshabilita la integración para todos los miembros del equipo. Para hacerlo, navega a **Configuración del equipo Apps e Integraciones**. Busca "Asana Ticketing" en la lista de aplicaciones instaladas, desplázate hacia abajo y haz clic en **Desinstalar para el equipo**.

### ¿Cómo se puede desactivar la integración (desinstalación individual)?

Los usuarios individuales pueden desinstalar la integración por sí mismos. Ve a **Aplicaciones e Integraciones** en tus configuraciones de Miro. Busca "Asana Ticketing" y haz clic en **Desinstalar para mí**.

### ¿Qué administradores pueden instalar la integración de Asana para su equipo?

Solo los administradores del equipo de Miro pueden instalar directamente la aplicación. Si un administrador del equipo de Miro pega una URL de Asana en un tablero de Miro, la aplicación se autorizará e instalará automáticamente sin requerir más acciones.

### ¿Cuáles son los requisitos de disponibilidad para la integración de Asana?

La integración de Asana está disponible para los planes Business y Enterprise de Miro.

### ¿Los administradores necesitan autorizar la integración de Asana para su equipo?

Sí, es posible que los administradores tengan que autorizar la integración de Asana para su equipo de Miro. Los miembros del equipo solo pueden usar la integración de Asana si se ha instalado a nivel del equipo.
