---
title: Configurar Linear (Beta) para tu equipo
article_id: 30630697364626
translation_id: 30630697364626
locale: es
sidebar_position: 2
created_at: '2025-10-29T14:09:41Z'
updated_at: '2026-02-23T11:23:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

La integración de Linear se implementa técnicamente a través de una API REST. Con fines de autenticación y autorización, se utiliza el protocolo estándar de la industria OAuth 2.0. Un componente clave de esta arquitectura es una plataforma API unificada que se utiliza como sub-procesador para datos de terceros, gestionando la autenticación, normalización y sincronización entre diferentes proveedores de API.

## Flujos de datos

Entender el flujo de datos es crucial para gestionar la seguridad y el cumplimiento.

### Diagrama de secuencia de alto nivel

Creación de un widget de tarjeta de Linear

![Asana Cards (BETA) (1).jpg](images/30631712515474_Asana%20Cards%20(BETA) (1).jpg)

Actualización de un widget de tarjeta de Linear

![Asana Cards (BETA) (1).jpg](images/30631712515474_Asana%20Cards%20(BETA) (1).jpg)

### Datos de Linear en Miro

Cuando los usuarios importan incidencias de Linear a un tablero de Miro, los siguientes datos son esenciales para el lienzo de Miro:

- Título
- Descripción
- Asignado a (nombre/correo electrónico)
- Estado
- Prioridad

Esta enumeración es vital para la gobernanza de datos, confirmando qué datos confidenciales entran en el entorno de Miro. Ten en cuenta que los campos personalizados no son compatibles.

### Retención de datos

Todos los datos importados de Linear se adhieren estrictamente a la política estándar de retención de datos de Miro, aplicada consistentemente a todos los datos de los clientes.

## Autenticación y autorización

Al primer contacto, la integración de Linear inicia un flujo de autenticación. Para cada usuario, Miro crea credenciales con el servicio de integración para interacciones posteriores.

La integración generalmente requiere la aprobación de un administrador de Linear.

### Autorización de flujos requerida

| Alcance | Descripción |
| --- | --- |
| Colecciones | Acceder a colecciones de incidencias. |
| Usuarios | Leer información de usuario para asignación/visualización. |
| Incidencias | Leer, crear, modificar incidencias en Linear. |

## Qué se almacena en Miro y cómo

- **Datos relacionados con la autorización:** Los tokens se almacenan en la base de datos de Miro durante varios días, encriptados con AES-256.
- **Datos relacionados con la expansión:** Los títulos de las incidencias se almacenan con referencias encriptadas.

### Revocar un token

La revocación de tokens puede ocurrir a través de **Configuración de Integración** o **Aplicaciones** seleccionando **Desconectar**. Esta acción elimina el acceso a Linear y borra las credenciales del usuario.

## Cómo configurar la integración de Linear

Los pasos tanto para administradores como para usuarios finales aseguran un despliegue controlado.

1. **Asegura Cuentas Activas:** Las cuentas de Miro y Linear deben estar activas.
2. **Instalación a Nivel de Equipo (Acción del admin):**
   - Los administradores deben autorizar la integración con Linear a nivel de equipo.
   - Instalación a través de **Herramientas Medios & Integraciones**, buscando "Linear" y conectando.
3. **Solicitud de usuario y aprobación del admin:**
   - En organizaciones con consentimiento estricto, pegar un enlace de Linear puede desencadenar una solicitud de aprobación del admin.
   - Los admins pueden aprobar a través de las consolas de Miro o Linear.
4. **Conexión de usuario individual:**
   - Los usuarios se conectan a través del widget de Linear y la autorización de OAuth.

## Seguridad y cumplimiento

### Restricción de acceso al archivo fuente

El mantenimiento de estrictos controles para compartir tableros alinea los permisos de Linear con Miro.

### Manejo de errores

La integración cuenta con una interfaz de usuario de respaldo amable para rechazos de terceros.

### Anexo de procesamiento de datos de Miro (DPA)

Consulta [el Anexo de Procesamiento de Datos de Miro](https://miro.com/legal/customer-data-processing-addendum/) para más información detallada sobre aspectos legales y de cumplimiento.

## Resolución de problemas y preguntas frecuentes

### Cómo desactivar la integración (a nivel de equipo)

Los administradores pueden desinstalar desde **Aplicaciones e Integraciones de configuración de equipo** seleccionando "Linear" y haciendo clic en **Desinstalar para el equipo**.

### Cómo desactivar la integración (individual)

Los usuarios pueden navegar a **Aplicaciones e Integraciones** y seleccionar "Desinstalar para mí" para Linear.

### Permisos del administrador

Solo los administradores del equipo de Miro pueden instalar directamente la aplicación. Las configuraciones automáticas ocurren al pegar una URL de Linear en un tablero.

### Requisitos de disponibilidad

La integración de Linear está disponible para los planes Business y Enterprise.

### Requisito de autorización del administrador

Sí, la autorización a nivel de equipo por parte de los administradores es necesaria para el acceso del equipo.
