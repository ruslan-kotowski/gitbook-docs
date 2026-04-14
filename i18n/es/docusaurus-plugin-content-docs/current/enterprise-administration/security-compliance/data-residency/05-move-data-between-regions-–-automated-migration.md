---
title: Mover datos entre regiones – Migración automatizada
article_id: 24866660560402
translation_id: 24866660560402
locale: es
sidebar_position: 5
created_at: '2025-02-24T08:47:08Z'
updated_at: '2025-10-29T14:40:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '¿Quién puede hacerlo: Administradores de la compañía Qué planes: Enterprise
    Qué plataformas: Navegador, Escritorio'
---

:::note
La migración automatizada es un servicio de pago con servicios profesionales. Para obtener una cotización, comunícate con tu contacto de Miro dedicado.
:::

Este artículo explica la migración automatizada de datos. Para conocer más sobre otras opciones para mover datos entre regiones, consulta [Mover datos entre regiones](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Datos incluidos en una migración automatizada entre regiones

La siguiente lista muestra qué datos incluye una migración automatizada entre regiones:

- Tableros, contenido de los tableros y configuraciones de compartición de los tableros
- Jerarquía de contenido, incluyendo equipos, espacios y secciones de espacios
- Configuraciones de organización, equipo y tablero
- Usuarios, perfiles de usuario y configuraciones de usuario, incluidos los invitados
- Registros de auditoría, clasificación de datos y configuraciones de seguridad de contenido

## Prepararse para una migración de datos entre regiones

Para prepararte para una migración de datos entre regiones, sigue estos pasos:

1. Para asegurarte de que puedes gestionar a todos los usuarios en tu dominio, verifica todos los dominios que posees con la verificación DNS.
2. Activa la política de control de dominio **Bloquear suscripciones propias**, que asegura que los usuarios no creen suscripciones gratuitas de Miro por accidente en tu antigua región.
3. Consolida equipos y/o organizaciones en una sola organización con una sola suscripción.
4. Audita qué integraciones utiliza y necesita tu organización en la nueva región, luego planifica un cronograma para reconfigurar cada integración en tu nueva región.

## Cómo funciona y cuánto dura una migración de datos entre regiones

Una migración entre regiones incluye los siguientes cinco pasos:

- **Preparación**
  Normalmente de 4 a 8 semanas. El admin de empresa, con el soporte de Miro, prepara su organización para la migración, programa el tiempo de inactividad de la migración y comunica a los usuarios finales
- **Migración**
  Generalmente <8 horas de inactividad. La organización y sus datos se migran a la nueva región.

  > ✏️ El equipo de Miro coordina contigo para elegir la fecha de la migración. Si la migración no tiene éxito por alguna razón, se restablece el acceso a tu región de origen, y Miro coordina una nueva fecha de migración contigo para reintentar la migración.
- **Verificación y configuración**
  Normalmente de 2 a 3 semanas. El admin debe reconfigurar ciertas integraciones, como el inicio de sesión único, en la nueva región. Admin y los usuarios verifican que sus tableros y datos hayan llegado a la nueva región como se esperaba.
- **Capacitación**
  Normalmente de 2 a 3 semanas. Se capacita a los usuarios sobre dónde acceder a su nueva organización de Miro.
- **Conformidad**
  Dentro de los 120 días posteriores a la fecha de migración, Miro verifica que los datos de la organización hayan sido eliminados de la región de origen.

## Qué hacer después de una migración de datos entre regiones

Después de una migración de datos entre regiones, asegúrate de hacer lo siguiente:

- Reconfigura inmediatamente el inicio de sesión único, si corresponde, para los nuevos subdominios regionales. Por ejemplo, au.miro.com.

  > ✏️ Tus usuarios no podrán iniciar sesión en la nueva región hasta que el inicio de sesión único esté reconfigurado del lado del IdP.
- Reconfigura SCIM para los nuevos subdominios regionales. Por ejemplo, au.miro.com.
- Verifica que **Bloquear suscripciones propias** en la configuración de control de dominio esté activado.
- Valida tus otras configuraciones de control de dominio.
- Reinstala y configura las aplicaciones e integraciones relevantes.

## Preguntas frecuentes sobre las migraciones automatizadas de datos entre regiones

**¿Qué es una migración de datos entre regiones?**

Las migraciones de datos entre regiones automatizan el movimiento de datos de clientes de una región geográfica a otra. El resultado final de una migración entre regiones es que tus datos de cliente de Miro dentro del alcance estarán almacenados y procesados en la nueva región.

**¿Cómo funciona y cuánto tiempo dura?**

Consulta Cómo funciona una migración de datos entre regiones y cuánto tiempo dura.

**¿Quién es elegible y quién no?**

Para automatizar una migración entre regiones, debes ser un cliente Enterprise. Sin embargo, un cliente Enterprise que usa Enterprise Guard y EKM no es elegible. Para obtener más información, comunícate con tu persona de contacto de Miro.

**¿Qué datos se incluyen en una migración automatizada entre regiones?**

Para saber qué datos se incluyen en una migración automatizada entre regiones, consulta Datos incluidos en una migración automatizada entre regiones.

**¿Qué datos no están incluidos en una migración de datos automatizada entre regiones?**

Una migración automatizada entre regiones no incluye los siguientes datos:

- Aplicaciones e integraciones, incluido el inicio de sesión único (SSO) y SCIM, que deben reconfigurarse para la nueva región
- Talktracks
- Las notificaciones dentro de la aplicación se borran

**¿Tiene un costo adicional?**

Sí. Una migración automatizada entre regiones es un servicio de pago de Miro Services. Para más información, comunícate con tu persona de contacto de Miro.

**¿Cómo garantiza Miro que los datos de mi organización se eliminen de la región de origen?**

Para eliminar tus datos de la región de origen después de una migración entre regiones, Miro sigue el siguiente protocolo:

- Los datos permanecen en la región de origen durante 30 días, lo que asegura que haya una copia de seguridad confiable en caso de que haya una incidencia con la migración.
- Después de 30 días, Miro comienza a eliminar tus datos de la región de origen.
- Después de un máximo de 120 días desde la fecha inicial de la migración, Miro ha eliminado todos los datos de la región de origen.

**¿Qué ven los usuarios durante una migración entre regiones?**

Para conocer la experiencia del usuario durante una migración, consulta [Experiencia del usuario al mover datos entre regiones](../../canvas-25-admin-features/data-residency/04-user-experience-while-moving-data-between-regions.md).

**¿Qué sucede si la migración no tiene éxito?**

Si la migración no tiene éxito por cualquier motivo, Miro restablece el acceso a tu región de origen y coordina una nueva fecha para reintentar la migración.
