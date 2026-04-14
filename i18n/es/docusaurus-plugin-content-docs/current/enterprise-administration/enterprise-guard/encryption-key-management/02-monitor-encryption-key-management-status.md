---
title: "Monitorear el estado de la gesti\xF3n de claves de cifrado"
article_id: 31325531757970
translation_id: 31325531757970
locale: es
sidebar_position: 1
created_at: '2025-11-24T17:59:06Z'
updated_at: '2026-02-04T20:46:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

Los administradores pueden monitorear y rastrear el estado de la configuración de la gestión de claves de cifrado (EKM) en la consola de administración de Miro. Esto aporta una mayor transparencia en la incorporación de claves y el progreso de cifrado, ayudándote a mantenerte informado sin necesidad de asistencia adicional.

## Verificar el estado de EKM

1. En la consola de administración de Miro, dirígete a **Enterprise Guard**.
2. Selecciona **Gestión de claves de cifrado**.
3. En la sección de **Estado**, revisa el estado y el mensaje actuales.

## Entender el estado de EKM

La sección de **Estado** muestra en qué parte del proceso de configuración y cifrado del EKM te encuentras.

| Estado | Qué significa |
| --- | --- |
| **Claves personalizadas añadidas** | Miro está configurando el cifrado con tus claves personalizadas. Una vez listo, tus claves comenzarán automáticamente a cifrar el contenido. |
| **Activación de clave en progreso** | El nuevo contenido se cifra con tus claves personalizadas. Se está re-cifrando el contenido existente. |
| **Claves personalizadas activas** | Todo el contenido está cifrado con tus claves personalizadas. |
| **Cambiando a claves predeterminadas** | Miro está cambiando tu cifrado de nuevo a las claves predeterminadas de Miro. Tus claves personalizadas serán eliminadas. |

## Revisar claves configuradas

En la sección de Llaves, puedes ver los identificadores de las llaves actualmente configuradas para EKM. Si Miro gestiona tus llaves personalizadas, es posible que veas una notificación en lugar de un ARN de llave.

- **Llave primaria**

  Cifra los tableros de tu organización, comentarios y otro contenido.
- **Clave de almacenamiento de copia de seguridad**

  Cifra versiones archivadas y copias de seguridad.
- **ARN de llave**

  El identificador de la llave en [AWS KMS](https://aws.amazon.com/kms/). Si Miro gestiona tus llaves personalizadas, es posible que veas una notificación en lugar de un ARN de llave.

(Opcional) Para realizar cambios en tus claves (por ejemplo, si ves la clave incorrecta o deseas volver a la encriptación predeterminada), puedes contactar a tu gerente de Customer Success o a [support@miro.com](mailto:support@miro.com).
