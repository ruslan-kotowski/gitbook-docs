---
title: "Registros de interacci\xF3n de IA (Beta)"
article_id: 34049604547858
translation_id: 34049604547858
locale: es
sidebar_position: 1
created_at: '2026-03-15T21:28:41Z'
updated_at: '2026-03-16T09:09:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Los registros de interacción con IA permiten a los admins con el complemento Enterprise Guard recopilar y revisar los registros del uso de Miro AI en toda su organización. Al habilitar los registros de interacción con IA, los admins pueden proporcionar a los equipos de seguridad, cumplimiento y gobernanza una mayor visibilidad sobre cómo se utilizan las funciones de IA y qué información es procesada por los sistemas de IA.

Los registros de interacción con IA ayudan a las organizaciones a:

- Monitorear cómo se utilizan las funciones de IA en toda la organización
- Soportar revisiones de gobernanza, cumplimiento y seguridad
- Proporcionar visibilidad sobre la información compartida con los sistemas de IA
- Fortalecer la confianza y la adopción responsable de herramientas de IA

Los registros de interacción con IA capturan los registros de las interacciones entre los usuarios y las funciones impulsadas por IA en Miro. Estos registros ayudan a las organizaciones a revisar cómo se usa la IA en toda la organización y a respaldar los procesos internos de auditoría, gobernanza y cumplimiento.

Cuando están habilitados, los registros de interacción con IA capturan:

- Instrucciones del usuario enviadas a las funciones de IA
- Respuestas generadas por IA devueltas por el sistema
- Contexto del sistema asociado con la interacción

## Antes de comenzar

- Debes ser admin para habilitar o configurar los registros de interacción de IA.
- El complemento Enterprise Guard es necesario para usar esta función.
- Se deben habilitar los registros de interacción de IA antes de que comience la recopilación de datos.
- Solo se registran las interacciones que ocurren después de habilitar los registros.

## Habilitar registros de interacción de IA

1. Ve a la **consola de administración**.
2. Selecciona **Seguridad**.
3. Haz clic en **Registros de auditoría**.
4. Abre la pestaña de **Configuración**.
5. En la sección de **Registros de interacción con IA**, habilita la opción **Recopilar registros de interacción con IA**.
6. Selecciona el **período de retención de registros**.
7. Guarda tus cambios.

Después de habilitar esta configuración, Miro comenzará a recopilar registros de interacción con IA para nuevas interacciones con IA.

## Configurar la retención de registros

Los administradores pueden configurar cuánto tiempo se almacenan los registros de interacción de IA.

1. Ve a **Consola de administración > Seguridad > Registros de auditoría**.
2. En la sección de **Registros de interacción de IA**, selecciona el **período de retención** deseado.
3. Guarda tus cambios.

Los registros se eliminan automáticamente cuando el período de retención configurado expira.

## Acceder a los registros de interacción de IA a través de APIs

Los registros de interacción de IA pueden recuperarse utilizando la API de registros de interacción de IA.

Esto permite a las organizaciones exportar y analizar los datos de interacción de IA usando sus sistemas de monitoreo de gobernanza, cumplimiento o seguridad existentes.

Los casos de uso comunes incluyen:

- Gobernanza y supervisión de IA
- Monitoreo de seguridad
- Auditoría de cumplimiento
- Investigaciones internas

Para más información, consulta la [documentación para desarrolladores](https://developers.miro.com/reference/enterprise-get-ai-interaction-logs).

## Limitaciones

La versión actual incluye la versión inicial del registro de interacciones de IA. Las siguientes limitaciones se aplican:

- Las invocaciones de herramientas de funciones de IA no se registran actualmente.
- Las interacciones relacionadas con las integraciones de Miro MCP no se registran actualmente.
- Los eventos de moderación y los bloqueos de instrucciones sensibles no se registran actualmente.
- Las imágenes no están incluidas en los registros de interacción de IA.
