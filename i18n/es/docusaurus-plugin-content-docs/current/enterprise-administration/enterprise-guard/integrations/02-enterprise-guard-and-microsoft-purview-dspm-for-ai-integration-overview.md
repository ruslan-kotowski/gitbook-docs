---
title: "Vista general de la integraci\xF3n entre Enterprise Guard y Microsoft Purview\
  \ DSPM para IA (Beta)"
article_id: 28617278171154
translation_id: 28617278171154
locale: es
sidebar_position: 0
created_at: '2025-08-07T15:17:38Z'
updated_at: '2026-01-12T11:27:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Para las organizaciones que utilizan Microsoft Entra ID (anteriormente Azure AD) como su proveedor de identidad, Enterprise Guard reenvía de manera segura instrucciones y respuestas de IA a Microsoft Purview Data Security Posture Management (DSPM) para IA. Los equipos de seguridad y cumplimiento pueden así monitorear, auditar y controlar el uso de IA generativa desde una plataforma de confianza única, reduciendo el gasto operativo, mitigando riesgos como la fuga y uso indebido de datos, y fortaleciendo la gobernanza de IA empresarial de Miro.

:::note
La versión Beta admite formatos de Miro AI, incluidos diagramas, mapas mentales, documentos, prototipos, notas adhesivas y tablas, pero no imágenes. Estamos trabajando para añadir soporte para imágenes y más funciones de IA en próximas versiones.
:::

## **Para quién es**

Esta función está disponible en la versión Beta para los clientes de Enterprise Guard que administran Miro y Microsoft Entra ID (anteriormente Azure AD)/Microsoft Purview.

## **Lo que obtienes**

- **Visibilidad centralizada:** Ver el uso de Miro AI en el AI hub de Microsoft Purview.
- **Auditabilidad:** Las instrucciones (entradas de usuario) y las respuestas (salidas de IA) se registran para revisión.
- **Alineación de gobernanza:** Usa tus flujos de trabajo existentes de Purview para monitoreo, alertas y retención.

## **Requisitos**

### **Miro**

- Plan Enterprise con **Enterprise Guard** habilitado.
- Eres un **admin de empresa**.
- Microsoft **Entra ID** configurado como proveedor de inicio de sesión único en Miro.
- Acceso a la página de **Integraciones de Enterprise** (si no puedes verla, pide a un **admin de empresa** que te conceda acceso).
- Para habilitar esta función en Beta, contacta a tu Customer Success Manager.

### **Microsoft**

- Licencia activa de **Microsoft Purview**.
- Tu **Microsoft Entra ID tenant ID** (el mismo inquilino utilizado para el inicio de sesión único de Miro; el GUID que identifica tu organización/inquilino de Microsoft).
- Un rol de Entra que puede **otorgar consentimiento de administrador a nivel de inquilino** para una aplicación.

## **Cómo funciona**

1. Un admin de Miro conecta tu inquilino de Microsoft Entra desde la página de **Integraciones de Enterprise** en Miro.
2. Esto instala la aplicación de **gobernanza de Miro AI** en tu inquilino de Microsoft (mediante el consentimiento de administrador a nivel de inquilino).
3. Cuando los usuarios inician sesión en Miro a través de ese inquilino y usan Miro AI, Miro reenvía la instrucción/respuesta a Microsoft Purview.
4. Las actividades aparecen en el **DSPM para AI → Activity explorer** (vista de Purview que lista las actividades de IA) en Microsoft Purview (permitir tiempo de ingestión).

## **Visibilidad de datos y latencia**

- Datos registrados: **Instrucciones y respuestas de IA** generadas en Miro por usuarios que inician sesión a través del inicio de sesión único para el inquilino configurado.
- Dónde verlo: **Microsoft Purview → DSPM para IA → Explorador de actividades** (la vista de Purview que muestra las actividades de IA). También puedes ver información en los registros de auditoría.
  **Nota:** Todas las instrucciones y respuestas basadas en texto a través de las funciones de Miro AI se envían a Purview. Actualmente, el contenido de imágenes no se envía a Microsoft Purview.
- Latencia: Los registros suelen aparecer **dentro de 10-30 minutos** después de la acción de IA en Miro.

## **Limitaciones conocidas**

- La versión Beta es compatible con los formatos de Miro AI, incluidos diagramas, mapas mentales, documentos, prototipos, notas adhesivas y tablas, pero no con imágenes. Estamos trabajando para añadir soporte para imágenes y más funciones de IA en próximas versiones.
- Puedes configurar **un ID de inquilino de Microsoft Entra** en Miro a la vez.
- En entornos con múltiples IdP o múltiples inquilinos, **solo** la actividad de los usuarios que inician sesión en Miro a través del **inquilino configurado** se registra en Microsoft Purview.

## **Seguridad y privacidad**

Miro envía las instrucciones y respuestas de IA a **tu inquilino de Microsoft** para que puedan ser monitoreadas en Purview. **La gobernanza, retención y controles de acceso** se gestionan en tu entorno de Microsoft.

##

## **Preguntas frecuentes**

- **P: ¿Qué funciones de Miro AI se registran?**
  **R:** Todas las instrucciones y respuestas basadas en texto de las funciones de Miro AI se envían a Purview. Actualmente, el contenido de imágenes no se envía a Microsoft Purview.
- **P: ¿Esto cubre a todos los usuarios?**
  **R:** Solo los usuarios que se autentican en Miro usando el inquilino de Microsoft Entra configurado están cubiertos.
- **P: ¿Puedo exportar registros desde Miro?**
  **A:** Usa Microsoft Purview para exportación y retención. Miro envía la actividad a tu inquilino de Microsoft donde está gobernada por tus políticas.
- **P: ¿Qué pasa con la seguridad y privacidad?**
  **A:** Miro envía instrucciones y respuestas de IA a **tu inquilino de Microsoft** para que puedan ser monitoreadas en Purview. **La gobernanza, la retención y los controles de acceso** son gestionados en tu entorno de Microsoft.

## **Soporte y recursos**

- Para los requisitos previos de consentimiento de Entra, consulta la documentación de Microsoft sobre **otorgar consentimiento de admin a nivel de inquilino** a una aplicación.
- Para obtener instrucciones de configuración de Enterprise Guard, consulta [esta documentación](../../enterprise-subscription-management/integrations/03-set-up-microsoft-purview-dspm-for-miro-ai.md).
