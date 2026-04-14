---
title: Registros de contenido
article_id: 17774729839378
translation_id: 17774729839378
locale: es
sidebar_position: 5
created_at: '2024-03-19T13:00:06Z'
updated_at: '2026-03-15T21:32:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
availability:
  notes: 'Configurado por: Admins de empresa, Admins de seguridad'
---

Los registros de contenido permiten a los clientes empresariales recopilar registros detallados de la actividad de los usuarios en los tableros y utilizarlos para investigaciones o archivado regulatorio.

Los registros de contenido pueden integrarse en diversas herramientas especializadas con fines legales, de cumplimiento y seguridad. Al proporcionar una solución para exportar datos de actividad de usuarios a gran escala, Miro reduce los riesgos para el cliente y abre oportunidades para que más trabajadores del conocimiento en la empresa experimenten el poder colaborativo de Miro mientras cumplen con estrictos requisitos de seguridad y cumplimiento.

## Datos de los registros de contenido

Cuando un usuario actualiza un widget en el tablero, se crea una entrada de registro con información como la hora de la acción del usuario, detalles del usuario, tipo de acción (crear, actualizar, eliminar), ID del tablero y del widget, y otra información relevante sobre el estado del widget como resultado de las acciones de los usuarios. Los registros de contenido *no* registran actualizaciones en la posición, tamaño o rotación de los widgets.

## Recopilación de registros de contenido

Los eventos se registran desde el momento en que un admin habilita la recopilación de registros de contenido. Los eventos recolectados se almacenan durante 30 días, por defecto.

Para habilitar la recopilación de registros de contenido, realiza los siguientes pasos:

1. Ve a Configuración de la empresa.
2. En el panel izquierdo, haz clic en **Seguridad** > **Registros de auditoría**.
3. En **Registros de auditoría**, haz clic en la pestaña **Configuración**.
4. En la sección de **Registros de contenido**, haz clic para activar el interruptor para **Recopilar registros de contenido**.
   ![content_logs.png](images/24937042282514_content_logs.png)
   *Activar la recopilación de registros de contenido*

## Acceder a los registros de contenido a través de la API

Los admins pueden usar la [API de registros de contenido](https://developers.miro.com/reference/board-content-logs) para acceder programáticamente a los datos de registros de contenido dentro de su organización. Los admins también pueden recopilar datos de registros de contenido usando integraciones compatibles, como Smarsh o Theta Lake.

Para autenticar el acceso a la API, los admins pueden elegir entre las siguientes opciones:

- Habilitar el toggle de eDiscovery en Integraciones de Enterprise.
- Crear una aplicación de plataforma y otorgarle acceso al scope Content log:read.
- Instalar y autorizar una de las integraciones de eDiscovery desde el Marketplace.

## Eliminar registros de contenido

Los admins pueden establecer una política de retención para los registros de contenido, escogiendo entre 30, 90, 180 o 365 días. Por defecto, el periodo de retención está fijado en 30 días.

:::note
Una vez eliminados los registros de contenido, no pueden ser recuperados.
:::

Para establecer un período de eliminación, realiza los siguientes pasos:

1. Ve a Configuración de la empresa.
2. En el panel izquierdo, haz clic en **Seguridad** > **Registros de auditoría**.
3. En **Registros de auditoría**, haz clic en la pestaña **Configuración**.
4. En **Registros de contenido**, elige una opción de la lista desplegable. Se te pedirá que confirmes tu elección.
   ![content_logs_duration.png](images/24937068869650_content_logs_duration.png)
   *Establecer política de retención de registros de contenido*
