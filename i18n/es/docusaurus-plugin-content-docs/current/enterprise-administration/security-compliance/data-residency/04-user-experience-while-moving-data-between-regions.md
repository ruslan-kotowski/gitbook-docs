---
title: Experiencia del usuario al mover datos entre regiones
article_id: 25075857856658
translation_id: 25075857856658
locale: es
sidebar_position: 4
created_at: '2025-03-04T08:51:38Z'
updated_at: '2025-05-09T08:47:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Quién puede hacerlo: Todos los usuarios Qué planes: Enterprise Qué plataformas:
    Navegador, escritorio, móvil'
---

Este artículo describe la experiencia del usuario durante una migración de datos entre regiones para exportaciones e importaciones tanto [automatizadas](../../canvas-25-admin-features/data-residency/05-move-data-between-regions-–-automated-migration.md) como [manuales](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## Experiencia del usuario durante la migración automatizada (beta)

Las siguientes secciones describen qué esperar antes, durante y después de un traslado automatizado de datos entre regiones.

### Antes de la migración automatizada

Dos semanas antes de la migración, todos los usuarios de tu organización Enterprise recibirán las siguientes notificaciones:

- **Banner dentro del producto**
  Muestra la fecha y la duración esperada de la migración en la zona horaria local.
- **Notificación por correo electrónico**
  Describe el próximo mantenimiento programado para todos los usuarios de la organización Enterprise.

:::note
Si eres miembro de varias cuentas de Miro, podrás seguir accediendo a tus otras cuentas durante la migración.
:::

### Durante la migración automatizada

Una migración automatizada requiere aproximadamente 8 horas de tiempo de inactividad.

Durante la migración automatizada, no podrás acceder a los datos de la organización Enterprise, incluidos los tableros, los equipos y la configuración.

El panel de Miro mostrará una notificación que indicará que se encuentra en curso una migración de datos de la organización. Durante el proceso de migración, no tendrás acceso a los tableros, los equipos ni la configuración de la organización.

:::tip
Si eres miembro de varias organizaciones, puedes cambiar a otra organización desde el panel y seguir usando Miro.
:::

### Después de la migración automatizada

Cuando la migración se complete correctamente, recibirás un correo electrónico de confirmación. Aparecerá un mensaje en el panel de Miro que confirmará la migración exitosa.

Si la migración no se completa correctamente, recibirás una notificación por correo electrónico. Podrás seguir usando Miro en la región de la UE iniciando sesión desde [miro.com](https://miro.com).

### Redirección de tableros después de la migración automatizada

Cualquier tablero que hayas agregado a los marcadores en la región anterior se redirigirá automáticamente a la nueva región y usará una URL actualizada.

## Experiencia del usuario durante la exportación e importación manuales

Los usuarios deben exportar manualmente las copias de seguridad de los tableros desde la región de origen e importarlas en la región de destino.

**Más información:** Consulta [Mover datos entre regiones – Exportación e importación manuales](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## Colaboración entre regiones

Los usuarios de Miro son regionales. Para colaborar con usuarios de organizaciones fuera de tu región, debes tener un perfil de usuario en cada región respectivamente.

Por ejemplo, si eres usuario de la región de la UE y quieres colaborar con usuarios de una organización de la región de AU, debes crear un perfil de usuario independiente en [au.miro.com](https://au.miro.com/).
