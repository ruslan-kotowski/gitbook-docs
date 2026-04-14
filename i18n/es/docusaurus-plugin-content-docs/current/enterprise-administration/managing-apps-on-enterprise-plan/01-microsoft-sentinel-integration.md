---
title: "Integraci\xF3n con Microsoft Sentinel"
article_id: 31325908249362
translation_id: 31325908249362
locale: es
sidebar_position: 1
created_at: '2025-11-24T18:16:15Z'
updated_at: '2025-12-16T15:49:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: audit-logs
---

## Vista general

El conector de [Miro](https://miro.com/) ingiere registros de auditoría y registros de actividad de contenido desde las [API REST de Miro](https://developers.miro.com/reference/overview) en Microsoft Sentinel utilizando el Codeless Connector Framework (CCF). Esto centraliza el monitoreo de la actividad del espacio de trabajo de Miro en Microsoft Sentinel para la detección de amenazas de seguridad, la investigación de incidentes y el informe de cumplimiento.

## Conectores de datos

Esta solución incluye dos conectores de datos.

| Conector | Requisitos del plan | Qué captura | Referencias |
| --- | --- | --- | --- |
| **Registros de auditoría de Miro (Plan Enterprise)** | Plan Enterprise | Eventos de auditoría a nivel organizacional, incluyendo autenticación de usuarios, acceso a contenido, cambios de equipo y acciones administrativas. | [Documentación de la API](https://developers.miro.com/reference/enterprise-get-audit-logs) | [Descripción general de los registros de auditoría](https://developers.miro.com/reference/audit-logs) |
| **Registros de Contenido de Miro (Plan Enterprise + Enterprise Guard)** | Plan Enterprise + complemento Enterprise Guard | Seguimiento de actividad de contenido, incluyendo la creación, actualizaciones y eliminaciones de elementos para cumplimiento y eDiscovery. | [Documentación del API](https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch) | [Descripción general de los registros de contenido](https://developers.miro.com/reference/board-content-logs) |

## Requisitos previos

### Requisitos generales

- Espacio de trabajo activo de Microsoft Sentinel.
- Rol de admin de empresa en tu organización de Miro.
- Token de acceso de OAuth de Miro (sin fecha de expiración).

### Requisitos específicos del conector

#### Para el conector de registros de auditoría

- Plan Enterprise de Miro.
- Alcance OAuth: `auditlogs:read`.
- Token de acceso.

#### Para el conector de registros de contenido

- Plan Enterprise de Miro + complemento Enterprise Guard.
- Alcance OAuth: `contentlogs:export`.
- Token de acceso.
- ID de la organización de Miro.

## Instalación

Hay dos maneras de configurar los conectores de Miro.

- **Opción 1 (recomendada):** Usa integraciones empresariales. Configuración más simple con generación automática de tokens.
- **Opción 2 (alternativa):** Crea una aplicación OAuth personalizada. Más control sobre la configuración de la aplicación OAuth.

**Nota:** cuando usas la Opción 1, la integración se vincula automáticamente al equipo con el mayor número de usuarios en tu organización. Al usar la Opción 2, puedes elegir a qué equipo instalar la aplicación. Sin embargo, la selección del equipo no afecta qué registros se recopilan. Ambas opciones proporcionan acceso a registros a nivel de organización. Todos los eventos relevantes para la integración de todos los equipos se incluyen en tus registros.

### Opción 1: Usar integraciones de Enterprise (recomendado)

Esta es la opción más sencilla para la mayoría de los usuarios. Automáticamente crea una aplicación OAuth y genera un token de acceso para ti a través de la configuración de integraciones de Enterprise de Miro.

#### Para el conector de registros de auditoría

1. Abre [la configuración de Miro](https://miro.com/app/settings/).
2. Expande la sección de **Aplicaciones e integraciones**.
3. Haz clic en **Integraciones de empresa**.
4. Habilita el interruptor de **SIEM**.
5. Copia el valor del **Token de acceso** que aparece.
6. Guarda el token de forma segura.

#### Para el conector de registros de contenido

1. Abre [la configuración de la empresa en Miro](https://miro.com/app/settings/).
2. Expande la sección **Aplicaciones e integraciones**.
3. Haz clic en **Integraciones empresariales**.
4. Habilita la opción de **eDiscovery**.
5. Copia el valor del **Token de Acceso** que aparece.
6. Obtén tu **ID de organización** de la URL del navegador:
   - Observa la URL del navegador para encontrar tu ID de organización.
   - El formato de URL es: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Copia tu ID de organización de la URL (el valor numérico).
7. Guarda de manera segura tanto el token como el ID de organización.

### Opción 2: Usar aplicación de OAuth personalizada (alternativa)

Esta opción te da más control sobre la configuración de la aplicación OAuth. Úsala si necesitas personalizar alcances, gestionar múltiples integraciones o prefieres la gestión manual de aplicaciones OAuth.

#### Paso 1: Crear aplicación OAuth de Miro

1. Inicia sesión en tu cuenta de Miro.
2. Ve a [configuración de aplicaciones de Miro](https://miro.com/app/settings/user-profile/apps).
3. Haz clic en **Crear nueva aplicación**.
4. Selecciona la opción de **Token de acceso no expirable** durante la creación de la aplicación ([más información sobre tokens OAuth](https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens)).
5. Habilita los alcances de OAuth requeridos:
   - `auditlogs:read` para el conector de registros de auditoría.
   - `contentlogs:export` para el conector de registros de contenido (requiere Enterprise Guard).
6. Haz clic en **Instalar la aplicación y obtener el token de OAuth**.
7. Copia el **Token de acceso** y guárdalo de manera segura.

Para obtener instrucciones detalladas sobre la configuración de OAuth, consulta [Comenzando con OAuth](https://developers.miro.com/docs/getting-started-with-oauth).

#### Paso 2: Obtener ID de organización (solo para registros de contenido)

1. Ve a [configuración de la empresa en Miro](https://miro.com/app/settings/).
2. Mira la URL del navegador para encontrar tu ID de organización:
   - El formato de la URL es: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Copia tu ID de organización de la URL (el valor numérico).

### Implementar la solución en Microsoft Sentinel

1. En Microsoft Sentinel, navega a **Content Hub**.
2. Busca **"Miro"** y haz clic en la solución.
3. Haz clic en **Instalar** y sigue el asistente de implementación.
4. Selecciona tu espacio de trabajo de Log Analytics.
5. Completa la instalación.

### Configurar conectores de datos

#### Conector de registros de auditoría de Miro

1. En Microsoft Sentinel, ve a **Conectores de datos**.
2. Encuentra **Registros de auditoría de Miro (Plan Enterprise)** y haz clic en **Abrir página del conector**.
3. Haz clic en **Conectar**.
4. Introduce tu **Token de acceso**.
5. Haz clic en **Conectar** para activar el conector.

#### Conector de registros de contenido de Miro

1. En Microsoft Sentinel, ve a **Conectores de datos**.
2. Encuentra **Miro Content Logs (Enterprise Plan + Enterprise Guard)** y haz clic en **Abrir página del conector**.
3. Haz clic en **Conectar**.
4. Ingresa tu **ID de Organización**.
5. Ingresa tu **Token de Acceso**.
6. Haz clic en **Conectar** para activar el conector.

La ingesta de datos comienza de 5 a 10 minutos después de la activación del conector.

## Tablas de datos

### MiroAuditLogs_CL

Eventos de auditoría a nivel de organización que incluyen:

- Autenticación y acceso de usuarios.
- Operaciones de contenido.
- Cambios en el equipo y la organización.
- Modificaciones en el perfil de usuario.
- Acciones administrativas.

**Columnas clave**

| Columna | Descripción |
| --- | --- |
| `TimeGenerated` | Marca de tiempo del evento. |
| `event` | Nombre del evento que identifica la acción o actividad específica. |
| `logType` | Tipo de entrada de log. |
| `category` | Categoría del evento que agrupa eventos relacionados. |
| `createdBy_email` | Usuario que desencadenó el evento. |
| `context_ip` | Dirección IP del evento. |
| `details` | Información adicional específica del evento (JSON). |

### MiroContentLogs_CL

Log de actividad a nivel de contenido que incluye:

- Operaciones a nivel de ítem con atribución de usuario y marcas de tiempo.
- Transiciones de estado y modificaciones.
- Seguimiento de actividades para cumplimiento y eDiscovery.

**Columnas clave**

| Columna | Descripción |
| --- | --- |
| `TimeGenerated` | Marca de tiempo del evento. |
| `actionType` | Tipo de acción realizada sobre el contenido. |
| `actor_email` | Usuario que realizó la acción. |
| `itemType` | Tipo de elemento de contenido afectado. |
| `contentId` | Identificador único del contenido. |
| `state` | Información del estado del elemento (JSON). |

## Consultas de ejemplo

### Ver eventos de auditoría recientes

```
MiroAuditLogs_CL
| sort by TimeGenerated desc
| project TimeGenerated, event, category, createdBy_email, context_ip
| take 20
```

### Actividad por usuario y tipo de evento

```
MiroAuditLogs_CL
| summarize EventCount = count() by createdBy_email, event, category
| order by EventCount desc
```

### Cambios de contenido por usuario

```
MiroContentLogs_CL
| where TimeGenerated > ago(7d)
| summarize Changes = count() by actor_email, actionType
| order by Changes desc
```

### Tendencias de eventos a lo largo del tiempo

```
MiroAuditLogs_CL
| summarize count() by event, bin(TimeGenerated, 1h)
| render timechart
```

### Usuarios más activos (cambios de contenido)

```
MiroContentLogs_CL
| where TimeGenerated > ago(30d)
| summarize TotalActions = count() by actor_email
| top 10 by TotalActions desc
```

## Resolución de problemas

### No hay datos disponibles

- Verifica que el token de acceso sea válido y tenga los alcances correctos.
- Para los registros de contenido, confirma que tu organización tenga el complemento Enterprise Guard.
- Confirma que el ID de la organización sea correcto (para los registros de contenido).
- Espera de 5 a 10 minutos para la ingestión inicial de datos.
- Verifica el estado del conector en la página de **Conectores de datos**.

### Errores de autenticación

#### Si se utiliza la Opción 1 (alternador de integraciones de Enterprise)

- Dirígete a [configuración de la empresa en Miro](https://miro.com/app/settings/), expande **Apps y integraciones** y haz clic en **Integraciones de Enterprise**.
- Verifica que el alternador (SIEM para registros de auditoría, eDiscovery para registros de contenido) siga habilitado.
- Si otro admin deshabilitó el alternador, el token será invalidado.
- Vuelve a habilitar el alternador para generar un nuevo token y actualizar la configuración del conector.
- Verifica que tengas el rol de admin de empresa en Miro.

#### Si usas la Opción 2 (aplicación OAuth personalizada)

- Verifica que el token no haya sido revocado en [configuración de la aplicación Miro](https://miro.com/app/settings/user-profile/apps).
- Asegúrate de que la aplicación OAuth tiene habilitados los alcances requeridos.
- Regenera el token si es necesario y actualízalo en la configuración del conector.
- Verifica que tengas el rol de admin de empresa en Miro.

### Los registros de contenido no funcionan

- Verifica que tu plan de Miro incluya el complemento **Enterprise Guard** (no disponible en el plan base Enterprise).
- Confirma que el alcance OAuth `contentlogs:export` esté habilitado.
- Verifica que el ID de la organización sea correcto.
- Contacta a tu gerente de cuentas de Miro en caso de que necesites mejorar a Enterprise Guard.

## Recursos

### Recursos del Centro de Ayuda de Miro

- **Registros de auditoría de Miro:** `../security-integrations/security-management/01-audit-logs.md
- **Registros de contenido de Miro:** `../canvas-25-admin-features/ediscovery/06-content-logs-overview.md
- **Guía de integración de Miro Sentinel:** `01-microsoft-sentinel-integration.md`.

### Documentación para desarrolladores de Miro

- **Comenzando con la API Enterprise:** `https://developers.miro.com/docs/getting-started-with-enterprise-api`.
- **Comenzando con OAuth:** `https://developers.miro.com/docs/getting-started-with-oauth`.
- **Autorización de token OAuth:** `https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens`.
- **API de registros de auditoría:** `https://developers.miro.com/reference/enterprise-get-audit-logs`.
- **API de registros de contenido:** `https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch`.
- **Referencia de la API:** `https://developers.miro.com/reference`.

### Microsoft Sentinel

- **Documentación de Microsoft Sentinel:** `https://docs.microsoft.com/azure/sentinel/`.
