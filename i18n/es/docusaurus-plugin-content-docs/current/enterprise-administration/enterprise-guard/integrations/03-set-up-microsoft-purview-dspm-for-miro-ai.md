---
title: Configurar Microsoft Purview DSPM para Miro AI (Beta)
article_id: 28698434922386
translation_id: 28698434922386
locale: es
sidebar_position: 8
created_at: '2025-08-11T19:20:50Z'
updated_at: '2026-01-12T11:28:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Usa este procedimiento para configurar Microsoft Purview Data Security Posture Management (DSPM) para Miro AI de modo que las instrucciones y respuestas de AI de Miro aparezcan en el DSPM para AI de Microsoft Purview. Después de la configuración, validarás los eventos y aprenderás a gestionar la integración.

## **Requisitos previos**

### **Miro**

- Plan Enterprise con **Enterprise Guard** habilitado.
- Eres un **Company Admin**.
- **Microsoft Entra ID** está configurado como un **proveedor de SSO** en Miro.
- Para habilitar esta función en Beta, contacta a tu CSM.

### **Microsoft**

- Licencia activa de Microsoft Purview con soporte para DSPM para IA.
- ID de inquilino de Microsoft Entra ID utilizado para el inicio de sesión único (SSO) de Miro (el GUID que identifica a tu organización o inquilino de Microsoft).
- Un rol de Entra que pueda otorgar consentimiento de administración a nivel de inquilino a una aplicación.

## **Configura la integración en Miro**

1. En Miro, abre **Configuración de Enterprise → Integraciones de Enterprise**.
2. Desplázate hacia abajo y luego haz clic para activar **Microsoft Purview DSPM para IA.**
3. En el cuadro de Tenant ID, ingresa tu **Microsoft Entra tenant ID**.
4. Haz clic en **Conectar**.
5. Cuando se te solicite, inicia sesión en Microsoft Entra con una cuenta que pueda otorgar **consentimiento de administrador a nivel de tenant**.
6. Revisa el consentimiento para la aplicación de **gobernanza de Miro AI** y haz clic en **Aceptar**.
7. Regresa a Miro y confirma que la integración muestra **Conectado.**

## **Validar actividad en Microsoft Purview**

1. En Miro, realiza una acción sencilla de IA (por ejemplo, **resume** notas adhesivas en un tablero).
2. Espera **hasta 10–30 minutos** para la ingesta.
3. En Microsoft Purview, ve a **Microsoft Purview → DSPM para IA → Explorador de actividades** (la vista de Purview que lista las Actividades de IA). También puedes ver información en los registros de auditoría.
   Nota: Todas las instrucciones y respuestas basadas en texto de las funciones de Miro AI se envían a Purview. Actualmente, el contenido de imagen no se envía a Microsoft Purview.
4. Filtra por eventos **Recientes** y localiza la actividad de Miro (por ejemplo, instrucción y respuesta).

## **Gestionar la integración**

- **Desconectar**: En Miro, ve a **Integraciones para empresas → Microsoft Purview para AI → Desconectar**.
- **Cambiar de inquilino**: **Desconectar** primero, luego **Conectar** nuevamente utilizando un **ID de inquilino** diferente.

## **Resolución de problemas**

- **Opción de integración no disponible**: Asegúrate de que tu organización tenga **Enterprise Guard** y que tu cuenta pueda acceder a **Integraciones para empresas**. Pide a un **admin de la empresa** que te otorgue acceso.
- **ID de inquilino incorrecto o error de conexión**: El ID de inquilino debe **coincidir exactamente** con el inquilino de Microsoft Entra utilizado para el **SSO** de Miro.
- **Fallo en el consentimiento o bucle de inicio de sesión**: Inicia sesión con una cuenta que pueda otorgar **consentimiento admin a nivel inquilino** (colabora con tu administrador de Microsoft).
- **No se ve actividad**: Confirma que un usuario haya realizado una prueba de acción de IA que inicie sesión en Miro a través del **tenant configurado**; espera **de 10 a 30 minutos**; verifica tu **licencia de Purview**; y revisa el **Explorador de actividades de DSPM para AI**.
- **Múltiples tenants/IdPs**: Solo se puede configurar **un tenant** en Miro. La actividad de los usuarios que inician sesión a través de inicio de sesión único para otros tenants/IdPs **no** se reenvía.

## **Limitaciones conocidas**

Para más información, consulta la [sección de limitaciones conocidas en la documentación de descripción general](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).
