---
title: Vista general
article_id: 30969987585938
translation_id: 30969987585938
locale: es
sidebar_position: 1
created_at: '2025-11-11T12:42:45Z'
updated_at: '2026-01-12T16:04:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

En Canvas 25, anunciamos el espacio de innovación con IA, incluyendo flujos de trabajo visuales de IA y agentes colaborativos de IA en el lienzo. Además de las funciones para los usuarios, estamos introduciendo nuevas funcionalidades para los administradores que te brindan más visibilidad, controles más inteligentes y formas fluidas de desbloquear las herramientas de IA más recientes de Miro para tus equipos.

Usa esta página para explorar las funcionalidades de administración de IA disponibles para administradores en el nivel Enterprise. Cada sección comienza con una breve descripción, seguida de preguntas frecuentes expandibles que cubren diferentes aspectos de cada funcionalidad.

- [Controles de Miro IA para admin:](01-overview.md) decide qué funcionalidades de IA están disponibles en tu organización y gestiona quién puede utilizarlas.
- Moderación de IA: establece niveles de filtrado para toda la organización (Estricto, Predeterminado, Mínimo) para filtrar instrucciones que podrían generar resultados dañinos o inapropiados.
- Estadísticas de Admin: utiliza paneles dentro del producto (Vista general y Miro IA) para seguir la adopción y entender la actividad de la organización, la asignación de licencias, el uso de plantillas y el uso de Miro IA en toda tu organización.

:::note
Durante el periodo Beta de AI Workflows, las Condiciones del Servicio Personalizadas de IA y los controles granulares de admin de Miro AI estaban disponibles para los clientes de AI Workflows. Ahora que AI Workflows está en Disponibilidad General, estas funcionalidades están disponibles solo como parte de Enterprise Guard. Para más información, consulta [Gobernanza avanzada de IA con Enterprise Guard](01-overview.md).
:::

## Controles de admin de Miro AI

Los controles de admin de Miro AI te ayudan a decidir qué funcionalidades de IA están disponibles en tu organización y a gestionar quién puede usarlas. Para más información, consulta la [documentación de controles de admin de Miro AI](../managing-enterprise-teams-and-content/01-miro-ai-admin-controls.md).

**Propósito y alcance**

**¿Qué son los controles administrativos de Miro AI?**

Los controles administrativos de Miro AI permiten a los admins gestionar el acceso a las funcionalidades de Miro AI en toda la organización. Dependiendo de tu configuración, puedes habilitar el acceso para todos, restringir el acceso a equipos específicos o deshabilitar el acceso.

**¿Cuál es la diferencia entre una funcionalidad de IA y una función de IA?**

Una **funcionalidad** es una categoría de funcionalidad de IA (por ejemplo, crear contenido, trabajar con imágenes o resumir actividad). Una **función** es una acción específica dentro de una funcionalidad (por ejemplo, *crear notas adhesivas* o *eliminar fondo*).

Los controles a nivel de función (gestionar funciones individuales dentro de una funcionalidad) están disponibles con [Enterprise Guard](01-overview.md).

**Acceso y requisitos previos**

**¿Dónde gestiono los controles de administración de Miro AI?**

En la Consola de Administración, ve a **Miro AI** > **Funcionalidades**. Desde allí, puedes habilitar, restringir o eliminar el acceso a cada funcionalidad de IA (y, si está disponible, a funciones individuales de IA).

**¿Quién puede configurar estos ajustes?**

Los administradores de la empresa pueden gestionar el acceso a Miro AI en la Consola de Administración (la disponibilidad de funciones de IA depende de tu plan y de los complementos habilitados).

**Opciones de acceso y comportamiento**

**¿Qué significan las opciones de acceso (Todos, Nadie, Equipos específicos)?**

Usa el menú desplegable junto a una funcionalidad (o función, si está disponible) para elegir cómo se concede el acceso.

| Opción | Qué hace | Cuándo usarla |
| --- | --- | --- |
| **Todos** | Habilita acceso para todos los usuarios y equipos de tu organización (incluyendo equipos creados posteriormente). Cualquier restricción a nivel de equipo se anula. | Despliegue estándar en toda la organización. |
| **Nadie** | Elimina el acceso para todos. Se te pedirá confirmación para eliminar. | Restringir el uso en toda la organización. |
| **Equipos específicos** | Habilita acceso solo para los equipos que selecciones. | Piloto con un subconjunto de equipos o despliegue en fases. |

**¿Qué ocurre si desactivo una funcionalidad?**

Cuando se desactiva una funcionalidad, los usuarios ya no pueden acceder a esa funcionalidad y sus funciones asociadas en los tableros. Si todas las funcionalidades de Miro IA están desactivadas, **Crear con IA** aparece deshabilitado en el tablero.

**¿Estas configuraciones se aplican a los equipos creados posteriormente?**

Si estableces una funcionalidad (o función) para **Todos**, se aplica a toda tu organización, incluidos los equipos creados posteriormente. Si eliges **Equipos específicos**, deberás actualizar la selección a medida que se creen nuevos equipos (si deseas incluirlos).

**Enterprise Guard y Control a Nivel de Funciones**

**¿Cómo cambia Enterprise Guard lo que puedo controlar?**

Con [Enterprise Guard](01-overview.md), puedes gestionar el acceso al **nivel de funciones** dentro de cada funcionalidad (no solo a nivel de categoría). Esto te permite permitir algunas funciones mientras restringes otras dentro de la misma funcionalidad.

Ejemplo: Puedes permitir *crear imágenes* y restringir *eliminar fondo* (dentro de la funcionalidad de Imágenes).

**Visibilidad y disponibilidad**

**¿Por qué no puedo ver la configuración para flujos, compañeros de IA o prototipos?**

Algunas funcionalidades (como **flujos**, **compañeros de IA** y **prototipos**) son visibles y gestionables solo si están habilitadas para tu organización.

**¿Puedo ver qué modelo de IA impulsa una función?**

Sí. En la Consola de Administrador > **Miro IA** > **Funcionalidades**, los administradores pueden ver los modelos que impulsan cada función de IA.

**¿Pueden los invitados o visitantes usar Miro IA si lo habilito?**

Miro IA está disponible para **miembros**. Los invitados y los visitantes no pueden usar Miro IA.

**Resolución de problemas y mejores prácticas**

**Cambié la configuración de acceso, pero los usuarios aún ven Miro AI. ¿Qué debo verificar?**

- **Confirma el alcance:** Asegúrate de haber actualizado la funcionalidad correcta (o la función específica, si aplican controles a nivel de función).
- **Revisa la selección de equipos:** Si está configurado para *Equipos específicos*, confirma que esté seleccionado el equipo del usuario.
- **Permite tiempo para la propagación:** En algunos casos, los cambios pueden tardar un poco en aplicarse en todas las sesiones.
- **Actualiza la sesión:** Pide al usuario que actualice la pestaña del navegador, cierre y vuelva a iniciar sesión, o reinicie la app de escritorio (si aplica).

## Moderación de Miro AI

Con la moderación de IA en Miro, los admins de empresa pueden ajustar los niveles de filtrado de instrucciones que podrían contener texto potencialmente dañino o inapropiado. Puedes establecer una sensibilidad de moderación de Miro AI a nivel de organización para filtrar contenido, incluyendo odio, contenido sexual, violencia y autolesiones. Esto te ayuda a alinear el uso de Miro AI con los requisitos, políticas y tolerancia al riesgo de tu organización. Para más información, consulta la [documentación sobre moderación de Miro AI](../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Propósito y alcance**

**¿Qué es la Moderación de IA en Miro?**

La Moderación de IA permite a los admins de empresa establecer un nivel de filtrado a nivel organizacional (estricto, predeterminado o mínimo) que revisa instrucciones que podrían resultar en contenido dañino o inapropiado (por ejemplo, odio, contenido sexual, violencia, autolesiones).

**¿Quién puede configurarlo y en qué planes?**

Los admins de empresa en el plan Enterprise con el complemento de Flujos de Trabajo de IA de Miro pueden configurar la opción en la configuración de la organización.

**¿Funciona si mi organización conecta su propio LLM (por ejemplo, una integración directa con el proveedor)?**

Si se conecta un LLM personalizado, el selector de moderación puede estar deshabilitado para esa integración y cualquier nivel previamente elegido no se aplicará a ella.

**Acceso y requisitos previos**

**¿Quién puede activarlo y qué se necesita?**

Los admins de empresa con el complemento de Miro AI Workflows pueden configurar la moderación de IA en los ajustes de la organización.

**¿Cómo lo activo?**

Ve a Configuración → Miro AI → Moderación, elige Estricto/Predeterminado/Mínimo y luego haz clic en **Guardar cambios**. La aplicación es inmediata en toda la organización.

**Niveles y comportamiento**

**¿Qué significan los niveles?**

- **Estricto:** Bloquea contenido por defecto + contenido de riesgo bajo a moderado (ej., odio sutil/codificado, contenido sexual sugestivo, violencia no gráfica, menciones de autolesiones no explícitas).
- **Por defecto (recomendado):** Bloquea contenido moderada a severamente dañino.
- **Mínimo:** Bloquea sólo contenido severamente dañino.

**¿Cuándo entran en vigor los cambios?**

Inmediatamente para toda la organización.

**¿Se registran los cambios?**

Sí. Las actualizaciones se registran en el historial de auditoría de tu organización.

**Configuración e instalación**

**¿Dónde configuro o actualizo el nivel de moderación?**

Ve a Configuración → Miro AI → Moderación, elige Estricto/Predeterminado/Mínimo, y luego haz clic en **Guardar cambios**.

**¿Qué nivel inicial recomiendan?**

Por defecto, es adecuado para la mayoría de las organizaciones; ajústalo basado en los comentarios del piloto y la tolerancia al riesgo.

**Interacciones con otros controles**

**¿Cómo se relaciona la Moderación de IA con las barreras de protección y las instrucciones?**

- **Barreras de protección inteligentes:** Si un tablero está cubierto por la barrera de protección “Bloquear el uso de Miro AI”, la IA se deshabilita independientemente del nivel de moderación.
- **Bloqueo de instrucciones:** Funciona junto con la Moderación. El bloqueo de instrucciones detiene las instrucciones sensibles al momento de enviarse; la Moderación filtra categorías dañinas.
- **Controles administrativos granulares:** Las opciones de función determinan quién puede acceder a las funciones de IA cuando la IA está disponible.

**Solución de problemas y mejores prácticas**

**Estamos viendo demasiados falsos positivos.**

Considera cambiar de Estricto → Predeterminado (o Predeterminado → Mínimo) y publica ejemplos de uso aceptables. Si los problemas persisten después de ajustar la configuración, contacta a tu gerente de Customer Success de Miro para informar esto y que el equipo de producto pueda revisarlo.

**Estamos viendo que se está filtrando contenido dañino.**

Pasa a Predeterminado o Estricto y proporciona orientación interna. Revísalo después de actualizaciones de políticas/regulaciones. Si los problemas continúan después de estos cambios, contacta a tu gerente de Customer Success de Miro para informar esto y que el equipo de producto pueda revisarlo.

## Analytics del Admin

Las Estadísticas de administración ofrecen a los admins de empresa datos útiles y procesables sobre la adopción, uso y gestión de Miro a gran escala. Incluye dos paneles: **Resumen** y **Miro AI**. Para más información, consulta [visión general de Estadísticas](../getting-started/admin-analytics/01-analytics-overview.md), [panel de Resumen](../getting-started/admin-analytics/02-overview-dashboard.md), y [panel de Miro AI](../getting-started/admin-analytics/03-miro-ai-dashboard.md).

**Propósito y alcance**

**¿Qué son las estadísticas de administración?**

Las estadísticas de administración proporcionan métricas confiables dentro del producto para ayudarte a entender cómo se está usando Miro, gestionar tu organización, impulsar la adopción y apoyar las necesidades de seguridad y cumplimiento.

**¿Qué paneles se incluyen?**

Las estadísticas de administración incluyen dos paneles: **Resumen** (actividad organizativa y adopción a través de tableros, usuarios, equipos, licencias y plantillas) y **Miro AI** (adopción y uso de Miro AI en toda la organización).

**Paneles y navegación**

**¿Cómo cambio entre los paneles?**

Usa las pestañas en la parte superior de la página de Estadísticas para cambiar entre **Resumen** y **Miro AI**.

**¿Cómo cambio el rango de tiempo?**

Utiliza el **Selector de rango de tiempo** en la esquina superior derecha de la página de Estadísticas para ajustar el rango de tiempo mostrado (**diario**, **semanal**, **mensual** o **trimestral**).

**¿Cuándo se actualizan los datos?**

Las métricas se actualizan **diariamente**. Cada panel muestra una marca de tiempo de **Última actualización**.

**Panel de vista general**

**¿Qué puedo rastrear en el panel de vista general?**

El panel de vista general te ayuda a rastrear la adopción y entender la actividad de la organización usando estos grupos de métricas:

- **Tableros:** totales de tableros, tableros activos y tendencias históricas.
- **Usuarios:** tendencias de usuarios activos. También puedes seguir por rol, como miembros, admins de empresa, invitados o invitados de equipo.
- **Equipos:** conteo de equipos y niveles de actividad.
- **Licencias:** tipos de licencias asignadas y cómo cambia la asignación a lo largo del tiempo.
- **Plantillas:** qué plantillas se utilizan más en toda tu organización.

**¿Cómo debo interpretar los gráficos históricos?**

- En los widgets que muestran datos históricos, los valores representan los datos del **último día de cada periodo**.
- El **periodo actual en curso** no se muestra en los gráficos históricos.
- Los datos históricos están disponibles hasta por **un año** o hasta donde existan los datos.

**Panel de Miro AI**

**¿Qué puedo rastrear en el panel de Miro AI?**

El panel de Miro AI te ayuda a rastrear la adopción y a entender cómo se usa Miro AI en toda tu organización usando estas métricas:

- **Equipos usando IA:** equipos que utilizan activamente las funciones de IA, incluidos los totales de equipos que usan versus los que no usan IA. Puedes filtrar el uso por caso de uso.
- **Personas usando IA:** totales de adopción de personas que usan versus las que no usan IA, con historial de uso mensual.
- **IA por caso de uso:** uso a lo largo del tiempo dividido por **creación de IA** y **automatización de IA**.
- **Colaboraciones de compañeros de IA:** con qué frecuencia los equipos interactúan con los compañeros de IA a través de sesiones de chat (instrucciones, preguntas de seguimiento y respuestas). Las estadísticas muestran el número de sesiones iniciadas.
- **Flujos de IA ejecutados:** cuántas veces los usuarios han ejecutado un flujo de IA con al menos dos pasos o nodos consecutivos. La ejecución se contabiliza en la marca de tiempo del primer evento asociado con el flujo.

**¿Cómo se definen los casos de uso de IA?**

- **Creación de IA:** acciones como crear a partir de instrucciones y crear a partir de contexto visual.
- **Automatización de IA:** acciones como iterar a través del chat o del menú contextual, editar texto, agrupar y eliminar los fondos de las imágenes.

**¿El uso de Créditos de IA es lo mismo que las métricas de uso de IA?**

No. **Los Créditos de IA no están directamente correlacionados** con las métricas de uso de IA que se muestran en este panel.

**Consideraciones de datos**

**¿Por qué veo datos parciales?**

Si una función estuvo deshabilitada durante parte del periodo seleccionado, podrías ver datos parciales en el historial de métricas (por ejemplo, si una función fue habilitada a mitad de mes).

**¿Por qué los gráficos no muestran datos para un periodo?**

Si no se registró actividad durante un periodo dado (día, semana o mes), el gráfico no mostrará datos para ese periodo de tiempo.

**Parece faltar datos antiguos. ¿Qué debo hacer?**

Los datos históricos están disponibles por hasta un año o desde que los datos existen. Si los datos antiguos parecen faltar, contacta al Soporte de Miro para solicitar verificación de recuperación.

**Solución de problemas y mejores prácticas**

**Nuestros números parecen más bajos de lo esperado. ¿Qué debo verificar?**

- Confirma el **rango de tiempo** y el tipo de período (diario, semanal, mensual, trimestral).
- Recuerda que **los gráficos históricos muestran períodos completados**, no el período actual en curso.
- Si una funcionalidad se activó a mediados del período, espera **datos parciales** para ese periodo.

**¿Cómo uso estos conocimientos de manera efectiva?**

Utiliza las métricas de Overview para detectar equipos, plantillas o tendencias de licencias subutilizadas y luego ejecuta un habilitación específica. Usa las métricas de Miro AI para identificar dónde está creciendo la adopción de la IA, apoyar a los campeones y guiar un despliegue responsable.

## Gobernanza de IA avanzada con Enterprise Guard

Enterprise Guard proporciona capacidades adicionales de gobernanza avanzada de IA para los admins de Enterprise. Usa estos controles para ajustar el acceso, proteger información sensible y fortalecer la supervisión y el cumplimiento para el uso de IA en Miro. Para más información, consulta [capacidades de confianza de IA de Enterprise Guard y FAQs](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md).

- [Controles de administración detallados de Miro AI](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): establece el acceso a nivel de función (Todos/Nadie/Equipos específicos) dentro de cada categoría de funcionalidad.
- [Bloquear el uso de Miro AI con las Barreras de Protección Inteligentes](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): utiliza las Barreras de Protección Inteligentes para bloquear todas las interacciones potenciadas por IA en Miro cuando necesites proteger datos sensibles o clasificados.
- [Bloqueo de instrucciones](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): bloquea las instrucciones que contengan datos sensitivos o código fuente en el momento de la presentación; en lugar de enviarlas a un LLM, muestra un mensaje de política.
- [Enterprise Guard e integración de Microsoft Purview DSPM para IA](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): envía las instrucciones y respuestas a Purview para su monitoreo, auditoría y gobernanza centralizados.
