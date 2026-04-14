---
title: Configurar integraciones de Microsoft y Power BI
article_id: 25132703621394
translation_id: 25132703621394
locale: es
sidebar_position: 3
created_at: '2025-03-06T10:27:14Z'
updated_at: '2025-11-25T15:49:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
---

:::note
Para obtener documentos de administrador completos específicamente sobre la integración de Miro con Microsoft o Power BI, incluidos diagramas detallados y más preguntas frecuentes, consulta la [documentación de administración de Microsoft](https://docs.google.com/document/d/1Gw94z5Pc-elS-pRXKGZVBWKKNEIFR9y9yzAAkbXKwMM/edit?usp=sharing) o la [documentación de administración de Power BI](https://docs.google.com/document/d/1hMepF163jQF8LI-U8ES8DzHVMW4TltXDr14fJ2KU29k/edit?tab=t.0#heading=h.gu9ng058yy7y).
:::

Este artículo explica cómo configurar una integración con Microsoft o Power BI en Miro.

## Configura una integración de Microsoft o Power BI

Para configurar una integración de Microsoft o Power BI, debes habilitar que los usuarios autoricen su propio contenido de Microsoft o Power BI en Miro.

### Requisitos previos

- Asegúrate de tener acceso de admin a Microsoft Entra.
- Un admin de empresa ha aprobado Microsoft o Power BI para tu organización de Miro (esto se refiere a las políticas de aprobación de aplicaciones en Miro si tu organización restringe las instalaciones de aplicaciones).

### Procedimiento

Estos pasos se centran en configurar Microsoft Entra para permitir la integración de Miro.

1. Inicia sesión en **Entra** como admin.
2. Ir a **aplicaciones empresariales** > **Consentimientos y permisos**.
3. Para **Los usuarios pueden solicitar el consentimiento del admin para las aplicaciones a las que no pueden consentir**, selecciona **Sí**.
4. Bajo **Quién puede revisar las solicitudes de consentimiento de administrador**, elige los usuarios, roles o grupos que desees permitir para revisar las solicitudes de consentimiento de administrador para aplicaciones.

:::note
Los administradores de Entra designados en el paso 4 anterior pueden ir a **Enterprise applications > Solicitudes de consentimiento de admin** en Microsoft Entra para revisar y aprobar la aplicación "Contenthub PowerBI Integratio" (o una con nombre similar) para la organización.
:::

## Valida tu integración de Microsoft o PowerBI

Copia y pega un enlace a tu tablero de Miro.

Si la aplicación es preaprobada por tu admin de empresa, sigue las instrucciones modales en pantalla. Miro añade el contenido de tu aplicación al tablero como un iFrame.

Si la aplicación no está preaprobada, entonces el modal **Agregar y permitir** se abre y te habilita para enviar una solicitud a tu admin de empresa. Enviar tu solicitud.

Cuando el admin de empresa responda, recibirás una notificación.

**Más información:** Consulta la [gestión de aplicaciones](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).
