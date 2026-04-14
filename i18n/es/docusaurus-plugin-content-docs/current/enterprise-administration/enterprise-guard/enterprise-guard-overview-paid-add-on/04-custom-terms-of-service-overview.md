---
title: Resumen de las Condiciones del Servicio personalizadas
article_id: 27375760557330
translation_id: 27375760557330
locale: es
sidebar_position: 2
created_at: '2025-06-13T08:24:28Z'
updated_at: '2025-11-04T14:10:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

La función de condiciones del servicio personalizadas permite a los admins mostrar un diálogo de Condiciones del Servicio personalizado para todos los miembros internos de su organización en Miro. Esto asegura que los usuarios revisen y reconozcan las condiciones y políticas de la organización antes de usar Miro. Utiliza esta función para informar a los usuarios sobre las políticas de uso aceptable de las funciones de Miro, incluyendo Miro AI. Los admins pueden añadir múltiples enlaces a políticas alojadas externamente y configurar la recurrencia para que los usuarios sean alertados según un horario que coincida con los requisitos internos. Todas las acciones relacionadas con las condiciones del servicio personalizadas se registran en los registros de auditoría para asegurar la trazabilidad.

:::note
Las Condiciones del Servicio Personalizadas están actualmente disponibles solo en la aplicación web y navegadores.
:::

## Beneficios clave

- Mostrar las condiciones del servicio en toda tu organización.
- Presentar el diálogo de condiciones del servicio personalizado en los puntos de uso relevantes: después de un inicio de sesión exitoso o al interactuar con Miro AI.
- Aplicar la aceptación del usuario en un horario que configures (días, semanas o meses) o al realizar actualizaciones.
- Vincular hasta tres políticas alojadas interna o externamente en tu idioma o formato preferido.
- Mantener la capacidad de auditoría en los registros de auditoría.

## Alcance

- Se aplica a: solo usuarios internos, todos los miembros de la organización y admins.
- Excluidos: invitados y colaboradores externos.
- Desencadenadores:
  - Inicio de sesión exitoso: mostrado inmediatamente después de iniciar sesión.
  - Uso de Miro AI: mostrado cuando un usuario interactúa con Miro AI (por ejemplo, activando el layout de IA, abriendo el panel lateral de IA o comenzando una acción de IA como los compañeros de IA).
- Recurrencia: configurable por el admin en días, semanas o meses. Cada condición del servicio personalizada tiene su propio estado y recurrencia. Predeterminada: dos semanas.
- Formato de condiciones: el contenido debe estar alojado externamente. Miro hace referencia a los enlaces y no almacena el texto completo de las políticas.
- Enlaces: hasta tres enlaces de políticas, cada uno con una etiqueta clara.
- Configuración: puedes configurar un conjunto de condiciones personalizadas para cada desencadenante (inicio de sesión exitoso y uso de Miro AI). Cada conjunto de condiciones tiene su propio estado y recurrencia.

## ¿Quién puede usar esta función?

Los administradores deben tener los siguientes privilegios de Enterprise Guard para ver y gestionar las condiciones personalizadas del servicio:

- **Admin de contenido sensible:** tiene permisos integrados.
- **Roles de admin personalizados**, deben incluir:
  - Ver Condiciones del Servicio personalizadas
  - Administrar Condiciones del Servicio personalizadas

## Cómo funciona

1. **Configura las condiciones:** elige el detonante (inicio de sesión exitoso o uso de IA), el alcance (miembros internos) y la recurrencia.
2. **Agrega contenido:** proporciona un título conciso, una breve descripción y hasta tres enlaces etiquetados a políticas alojadas externamente.
3. **Revisa y habilita:** previsualiza el diálogo para el usuario final y habilita la configuración.
4. **Aplicación:**

- **Inicio de sesión exitoso:** el diálogo no se puede descartar. Los usuarios deben aceptar para continuar o cerrar sesión.
- **Uso de IA:** el diálogo permite **Continuar** o **Cancelar**. Cancelar mantiene al usuario conectado con las funciones de IA deshabilitadas.

5. **Registro:** los cambios de configuración y las aceptaciones de los usuarios se registran en los registros de auditoría.

### Experiencia del usuario

- **Inicio de sesión exitoso**

  - El diálogo aparece inmediatamente después del inicio de sesión.
  - Los usuarios pueden hacer clic en **Continuar** para aceptar y proceder, o en **Cerrar sesión**.
- **Uso de Miro AI**

  - El cuadro de diálogo aparece cuando el usuario interactúa con Miro AI, como al activar el diseño AI, abrir el panel lateral de AI o iniciar una herramienta o acción de AI (por ejemplo, Compañero de IA).
  - Los usuarios pueden hacer clic en **Continuar** para aceptar y usar las funciones de AI. Si los usuarios hacen clic en **Cancelar**, permanecen conectados y pueden seguir usando todas las funciones que no sean de AI.
- A los usuarios no se les vuelve a solicitar hasta que finalice la ventana de recurrencia o se actualicen las condiciones.

## Comportamiento de aceptación

- **Disparador de inicio de sesión:** los usuarios deben aceptar según el horario configurado o cerrar la sesión. No se puede omitir el diálogo.
- **Disparador de uso de IA:** los usuarios pueden aceptar para habilitar las funciones de IA o cancelar para mantenerlas deshabilitadas. Cancelar mantiene al usuario conectado y con la capacidad de usar las funciones no relacionadas con IA.
- **Recurrencia y versiones:** los usuarios no reciben indicaciones nuevamente hasta que finalice el período de recurrencia o se publique una nueva versión, de acuerdo con el disparador configurado.

##

###
