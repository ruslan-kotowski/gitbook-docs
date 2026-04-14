---
title: Funcionalidades de confiabilidad de IA y FAQ
article_id: 30943405232914
translation_id: 30943405232914
locale: es
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:34:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

En Canvas 25, anunciamos el espacio de innovación impulsado por IA con flujos de trabajo visuales de IA y agentes colaborativos de IA en el lienzo. Además de las funciones para el usuario, estamos introduciendo nuevas funcionalidades de admin para darte más visibilidad, controles más inteligentes y formas simples de desbloquear las herramientas de IA más recientes de Miro para tus equipos.

Utiliza esta página para explorar las funcionalidades de confianza de la IA disponibles con el complemento Enterprise Guard. Cada sección comienza con una breve descripción, seguida de un FAQ ampliable que cubre diferentes aspectos de cada funcionalidad.

- Controles administrativos granulares de Miro AI: establece el acceso a nivel de función (Todos/Nadie/Equipos específicos) dentro de cada categoría de funcionalidad.
- [Bloquear el uso de Miro AI con barreras de protección inteligentes](#h_block_ai_with_guardrails): utiliza las barreras de protección inteligentes para bloquear todas las interacciones impulsadas por IA en Miro cuando necesites proteger datos sensibles o clasificados.
- [Panel de Vista general de Estadísticas de Administración](#h_admin_analytics_overview): realiza un seguimiento de tableros, usuarios, equipos, licencias y plantillas con tendencias históricas y actualización diaria.
- Moderación de IA (también disponible en el nivel Enterprise): establece niveles de filtrado en toda la organización (Estricto, Predeterminado, Mínimo) para examinar las instrucciones que podrían conducir a resultados dañinos o inapropiados.
- Bloqueo de instrucciones: bloquea instrucciones que contengan datos sensibles o código fuente en el momento de la presentación; muestra un mensaje de política en lugar de enviarlas a un LLM.
- Enterprise Guard e integración con Microsoft Purview DSPM para AI: reenvía instrucciones y respuestas a Purview para monitoreo centralizado, auditoría y gobernanza.

## Controles administrativos detallados de Miro AI para el complemento Enterprise Guard

Los controles administrativos de Miro IA permiten a los admins de empresa del Enterprise decidir qué funcionalidades de IA están disponibles en su organización y gestionar quién puede usarlas. Los admins también pueden ver los modelos que impulsan cada función de IA. Con el complemento Enterprise Guard, los controles de Miro IA se extienden al nivel de función dentro de cada categoría de funcionalidades, lo que ayuda a priorizar las funciones según las necesidades organizativas y los requisitos de seguridad. Además de la categoría completa de funcionalidades de Miro IA, los admins también pueden habilitar, restringir o eliminar funciones específicas de Miro IA. Por ejemplo, dentro de la categoría de Imágenes, puedes habilitar la creación de imágenes con IA y deshabilitar la eliminación del fondo. Usa estos controles para implementar la IA de manera segura y cumplir con los requisitos de seguridad mientras fomentas la adopción de las capacidades de la IA.  Para más información, consulta la [documentación de los controles administrativos granulares de Miro IA](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Propósito y alcance**

**¿Qué es el control granular para Miro AI?**

Con el complemento Enterprise Guard, los admins de empresa pueden habilitar, restringir o eliminar el acceso a funciones individuales de IA dentro de cada categoría de funcionalidades. Esto te permite elegir exactamente qué funciones pueden utilizar los equipos.

**¿Por qué utilizar controles granulares?**

Para equilibrar la adopción con la seguridad. Por ejemplo, dentro de Imágenes puedes permitir Crear imágenes mientras deshabilitas Eliminar fondo.

**Acceso y requisitos previos**

**¿Quién puede configurar controles granulares y en qué planes?**

Los admins de empresa en planes Enterprise con el complemento Enterprise Guard, en el navegador.

**¿Dónde gestiono el acceso a nivel de función?**

Consola de administración → Miro AI → Funcionalidades. Amplía una funcionalidad para ver y establecer el acceso a sus funciones individuales.

**Controles y comportamiento**

**Controles granulares: ¿cuál es la diferencia entre el control a nivel de funcionalidad y a nivel de función, y qué sucede cuando los activo o desactivo?**

- **Nivel de funcionalidad:** Todos, Ninguno o Equipos específicos se aplica a toda la categoría. Si desactivas una funcionalidad, los usuarios pierden acceso a esa funcionalidad y a todas sus funciones en todos los tableros. Si desactivas todas las funcionalidades, Crear con IA aparece deshabilitado en el tablero.
- **Nivel de función:** Con Enterprise Guard, puedes configurar Todos, Ninguno o Equipos específicos por cada función individual. Desactivar una función elimina el acceso solo a esa función; otras funciones en la misma funcionalidad permanecen disponibles si están habilitadas.

**¿Qué opciones de acceso existen a nivel de función?**

Para cada función, elige Todos, Nadie o Equipos específicos. Todos habilita la función en toda la organización y anula las restricciones a nivel de equipo. Nadie elimina el acceso para todos los usuarios. Equipos específicos está dirigido únicamente a equipos seleccionados.

**¿Qué ocurre cuando desactivo una función individual?**

Los usuarios no pueden acceder a esa función en ningún tablero, pero otras funciones dentro de la misma capacidad siguen disponibles si están habilitadas.

**Referencias y ejemplos**

**¿Qué funciones puedo controlar individualmente?**

Consulta la referencia en el producto para la lista actual. Los ejemplos en Crear contenido incluyen Crear notas adhesivas, Agrupar notas adhesivas, Crear y editar documentos, tablas, diagramas, y operaciones de texto como reescribir, acortar, tono y traducir. Imágenes incluye Crear imágenes, Eliminar fondo y Añadir subtítulos. Resumir actividad incluye Ponerse al día y Resumen de conversación. Flujos, compañeros de IA y Prototipado aparecen si están habilitados para tu organización.

**¿Puedo ver qué modelos impulsan funciones específicas?**

Sí. Los admins pueden ver los modelos asociados con cada función de IA en el área de referencia para apoyar la revisión y la gestión.

## Bloquear el uso de Miro AI con Barreras de Protección Inteligentes

Usa las barreras de protección para bloquear todas las interacciones impulsadas por IA en Miro cuando necesites proteger datos sensibles o clasificados. Cuando esta barrera se aplica, todas las herramientas de Miro AI están deshabilitadas en los tableros afectados, mientras que la colaboración sin IA sigue disponible. Para más información sobre el contexto y la configuración, consulta la descripción general de las barreras de protección y cómo definirlas.

**Propósito y alcance**

**¿Qué hace "bloquear el uso de Miro AI"?**

Deshabilita todas las funciones de Miro AI (por ejemplo, generación de texto, generación/reconocimiento de imágenes, sugerencias inteligentes) donde se aplica este guardrail, evitando cualquier interacción con contenido sensible o clasificado a través de la inteligencia artificial.

**¿Qué permanece disponible para los usuarios?**

Los usuarios pueden continuar con la colaboración regular, sin IA. El contenido generado por IA que ya existe en los tableros puede ser visto, movido o editado manualmente, pero los usuarios no pueden utilizar Miro AI para modificarlo o regenerarlo.

**Acceso y requisitos previos**

**¿Quién puede configurar esta barrera de protección y dónde?**

Los admins de contenido sensible configuran las barreras de protección en *Enterprise Guard* bajo Clasificación de Datos → Barreras de Protección. (Los admins de empresa asignan el rol de admin de contenido sensible.)

**¿Qué necesito antes de asignar esta barrera de protección?**

Define tus niveles de clasificación y (opcionalmente) la auto-clasificación para que la barrera de protección se pueda aplicar por clasificación (por ejemplo, INTERNO, CONFIDENCIAL).

**Comportamiento e impacto**

**¿Quién se ve afectado cuando se aplica el guardarraíl?**

Todo el mundo, incluidos los propietarios y copropietarios de tableros, no pueden acceder ni invocar Miro AI en los tableros afectados.

**¿Elimina el contenido existente de IA?**

No. Evita interacciones futuras con la IA; el contenido existente de IA sigue disponible para ver y editar manualmente.

**¿Cuándo entran en vigor los cambios?**

Después de publicar las actualizaciones del guardarraíl, la aplicación es inmediata en los tableros afectados.

**Configuración y ajuste**

**¿Cómo activo "Bloquear el uso de Miro AI" para una clasificación?**

1. Ve a *Enterprise Guard* → Clasificación de datos → **Barreras de seguridad**.
2. Haz clic en el ícono de **Editar** para un nivel de clasificación (por ejemplo, CONFIDENTIAL).
3. Selecciona la casilla de verificación **Bloquear el uso de Miro AI** y **Hecho.**
4. Haz clic en **Siguiente** y revisa el impacto, luego **Publicar** para aplicar.

**¿Debería usar el modo Predeterminado o el modo Estricto?**

En el modo Predeterminado, las barreras de protección no anularán las configuraciones de uso compartido existentes. En el modo Estricto, las barreras de protección anulan el uso compartido activo y aplican los controles más estrictos. Elige según tus necesidades de gestión de cambios.

**Experiencia del usuario**

**¿Qué verán los usuarios en los tableros donde la IA está bloqueada?**

Los puntos de acceso de Miro IA aparecen deshabilitados o no disponibles, y los usuarios no pueden invocar herramientas de IA desde el lienzo o los menús en esos tableros.

**¿Pueden los usuarios solicitar excepciones en un solo tablero?**

No. La barrera de protección se aplica según la política de clasificación. Cambia la clasificación del tablero (o la política para ese nivel) para alterar la aplicación.

**Interacciones con otros controles**

**¿Cómo se relaciona esto con los controles avanzados de Miro AI?**

Los controles avanzados gestionan quién puede usar funciones específicas de IA. El mecanismo de protección es una capa de política: cuando está activo, bloquea la IA independientemente de los ajustes de funciones.

**¿En qué se diferencia de la instrucción de bloqueo o la moderación de IA?**

- **Bloqueo de instrucciones** detiene instrucciones sensibles al momento de envío; la IA sigue disponible para instrucciones no sensibles.
- **Moderación de IA** filtra contenido dañino o inapropiado.
- **Bloqueo del uso de Miro IA** deshabilita completamente la IA en tableros afectados.

**Resolución de problemas**

**La IA todavía aparece en algunos tableros. ¿Qué debo verificar?**

- Confirma que la clasificación del tablero es una donde la barrera de protección está habilitada, y que hiciste clic en **Publicar** después de editar las barreras de protección.
- Si usas la clasificación automática, verifica que la clasificación del tablero se ha actualizado según el contenido actual.
- En los modos Estricto vs Predeterminado, asegúrate de que tu expectativa coincida con el modo de implementación que seleccionaste.

**Necesitamos volver a habilitar la IA para un subconjunto de trabajo.**

Ajusta la barrera de protección para la clasificación relevante o reclasifica los tableros que deben permitir la IA, luego publica la actualización.

## Panel de estadísticas del admin

**Alcance y métricas**

**¿Qué cubre el panel de vista general?**

Tableros, usuarios, equipos, licencias y plantillas, con tendencias históricas donde corresponda.

**¿Cómo se define "Activo en este periodo" para tableros, usuarios y equipos?**

- **Tableros:** Tableros únicos abiertos desde el comienzo del período seleccionado. Incluye tableros que luego se movieron a la papelera.
- **Usuarios:** Usuarios únicos que abrieron un tablero al menos una vez desde el comienzo del período. Incluye a los usuarios que ahora están desactivados.
- **Equipos:** Equipos únicos con al menos un miembro que abrió un tablero desde el comienzo del período. Puede incluir equipos que luego se movieron a la papelera.

**¿Los totales excluyen elementos en la papelera?**

Sí. Los totales para tableros y equipos excluyen los elementos que actualmente están en la papelera. Las cuentas históricas "activas" pueden incluir elementos que posteriormente fueron movidos a la papelera.

**¿Qué muestra el gráfico de Licencias?**

Totales y historial de asignación para licencias Full, Free y licencias gratuitas limitadas, reflejando cuántas licencias están en uso actualmente.

**¿Qué muestran hoy las plantillas?**

Las plantillas más populares utilizadas desde dentro de un tablero. Se pueden añadir otras fuentes en futuras actualizaciones.

**Comportamiento de tiempo e historial**

**¿Cómo se muestran los valores históricos en los gráficos del Resumen?**

Los widgets históricos muestran los valores al último día de cada período. Hay hasta un año de historial disponible o desde que existen los datos.

**Actualización y controles de los datos**

**¿Con qué frecuencia se actualizan los datos del panel y dónde los veo?**

Al menos una vez cada 24 horas. Una marca de tiempo "Última actualización" está disponible en el panel.

**¿Cómo cambio el rango de tiempo?**

Usa el selector de rango de tiempo en la parte superior derecha de la página de Estadísticas.

## Moderación con Miro AI

Con la moderación de Miro AI, los admins de empresa pueden ajustar los niveles de filtro para las instrucciones que podrían contener texto potencialmente perjudicial o inapropiado. Puedes establecer la sensibilidad de moderación de Miro AI para toda la organización, a fin de filtrar contenido, incluyendo odio, contenido sexual, violencia y autolesiones. Esto te ayuda a alinear el uso de Miro AI con los requisitos, políticas y tolerancia al riesgo de tu organización. Para más información, consulta la [documentación sobre moderación de Miro AI](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Propósito y alcance**

**¿Qué es la Moderación de IA en Miro?**

La Moderación de IA permite a los admins de empresa establecer un nivel de filtro a nivel organizacional (estricto, predeterminado o mínimo) que revise las instrucciones que puedan generar contenido dañino o inapropiado (por ejemplo, odio, contenido sexual, violencia, autolesiones).

**¿Quién puede configurarlo y en qué planes?**

Los admins de empresa en Enterprise con Enterprise Guard pueden configurar la configuración en los parámetros de la organización.

**¿Funciona si mi organización conecta su propio LLM (por ejemplo, una integración directa con un proveedor)?**

Si se conecta un LLM personalizado, el selector de moderación puede estar deshabilitado para esa integración y cualquier nivel previamente elegido no se aplicará a ella.

**Acceso y requisitos previos**

**¿Quién puede activarlo y qué necesito?**

Los admins de empresa con el complemento Enterprise Guard pueden configurar la Moderación de IA en la configuración de la organización.

**¿Cómo lo activo?**

Ve a Configuración → Miro AI → Moderación, elige Estricto/Predeterminado/Mínimo y luego haz clic en **Guardar cambios**. La aplicación es inmediata en toda la organización.

**Niveles y comportamiento**

**¿Qué significan los niveles?**

- **Estricto:** Bloquea contenido predeterminado + de bajo a moderado riesgo (por ejemplo, odio sutil/codificado, contenido sexual sugestivo, violencia no gráfica, menciones de autolesiones no explícitas).
- **Predeterminado (recomendado):** Bloquea contenido de moderado a severamente dañino.
- **Minimal:** Bloquea solo contenido severamente dañino.

**¿Cuándo tienen efecto los cambios?**

Inmediatamente para toda la organización.

**¿Se registran los cambios?**

Sí. Las actualizaciones se registran en el historial de auditoría de su organización.

**Configuración de preferencias**

**¿Dónde puedo establecer o actualizar el nivel de moderación?**

Ve a Preferencias → Miro AI → Moderación, elige Estricto/Predeterminado/Mínimo, y luego haz clic en **Guardar cambios**.

**¿Qué nivel inicial recomiendas?**

Predeterminado se adapta a la mayoría de las organizaciones; ajusta basado en comentarios durante el piloto y tolerancia al riesgo.

**Interacciones con otros controles**

**¿Cómo se relaciona la Moderación de IA con las barreras de protección y los controles de instrucciones?**

- **Barreras de protección inteligentes:** Si un tablero está cubierto por la barrera de protección “Bloquear el uso de Miro AI”, la IA se deshabilita independientemente del nivel de moderación.
- **Bloqueo de instrucciones:** Funciona junto con la Moderación. El bloqueo de instrucciones detiene las instrucciones sensibles al enviarse; la Moderación filtra categorías perjudiciales.
- **Controles de administración detallados:** Los interruptores de funciones gobiernan quién puede acceder a las funciones de IA cuando la IA está disponible.

**Solución de problemas y mejores prácticas**

**Estamos viendo demasiados falsos positivos.**

Considera cambiar de Estricto a Predeterminado (o de Predeterminado a Mínimo) y publica ejemplos de uso aceptable. Si los problemas persisten después de ajustar la configuración, contacta a tu gerente de Customer Success de Miro para reportarlo y que nuestro equipo de producto lo revise.

**Estamos viendo que pasa contenido dañino.**

Cambia a Predeterminado o Estricto y proporciona orientación interna. Revisa nuevamente después de actualizaciones de políticas/regulaciones. Si los problemas continúan después de estos cambios, contacta a tu gerente de Customer Success de Miro para reportarlo y que nuestro equipo de producto lo revise.

## Bloqueo de instrucciones

El bloqueo de instrucciones permite a los administradores de contenido evitar que los usuarios envíen instrucciones de IA que incluyan información sensible, ayudándote a mantener los datos confidenciales fuera de Miro AI en toda tu organización. Miro escanea el texto que un usuario ingresa en el campo de instrucciones y cualquier contenido basado en texto que agreguen desde el tablero. Si ese contenido coincide con las etiquetas de sensibilidad o patrones de código fuente seleccionados en la configuración de bloqueo de instrucciones, Miro bloquea el envío de la instrucción.  Para más información, consulta la [documentación sobre el bloqueo de instrucciones](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Propósito y alcance**

**¿Qué es el Bloqueo de Instrucciones?**

El Bloqueo de Instrucciones impide que los usuarios envíen instrucciones de IA que incluyan información sensible. Miro escanea el texto que un usuario escribe en el campo de instrucciones y cualquier contenido basado en texto que agreguen desde el tablero; si coincide con las etiquetas de sensibilidad seleccionadas o patrones de código fuente, se bloquea el envío y se muestra un mensaje de política. En este momento, solo se admite contenido basado en texto.

**¿Cómo es diferente el Bloqueo de Instrucciones de la exploración del tablero?**

La exploración del tablero encuentra contenido sensible en los tableros y puede clasificar automáticamente los tableros; el Bloqueo de Instrucciones verifica lo que los usuarios intentan enviar a Miro AI en el momento del envío.

**¿Qué etiquetas de sensibilidad son compatibles?**

Usa las categorías a nivel de organización listadas en referencia a las etiquetas de sensibilidad e infotipo.

**¿Qué es el Escaneo de Código?**

El Escaneo de Código bloquea instrucciones que contienen código fuente reconocible; por diseño, requiere un bloque mínimo de código (por ejemplo, más de 5 líneas) para activarse. Actívalo/desactívalo en la configuración de bloqueo de instrucciones.

**¿Se escanea contenido no textual (por ejemplo, imágenes)?**

No. En este momento, el bloqueo de instrucciones solo admite contenido basado en texto.

**Acceso y requisitos previos**

**¿Quién puede activarlo y qué necesito?**

Los admins de contenido sensible en Enterprise con el complemento Enterprise Guard pueden activarlo en Configuración → Enterprise Guard → Descubrimiento de datos → Configuración.

**¿Cómo lo enciendo?**

Abre el bloqueo de instrucciones → Habilitar, elige Seleccionar todas o categorías específicas de etiquetas, opcionalmente habilita el escaneo de código, y luego Activa. La aplicación es inmediata a nivel de la organización.

**Gestión y cambios**

**¿Cómo ajusto las etiquetas o la exploración de código más tarde?**

Ve a Configuración → Enterprise Guard → Descubrimiento de datos → Configuración → Bloqueo de instrucciones → Administrar,

- **Etiquetas:** Marca la casilla *Seleccionar todo* para seleccionar todas las categorías o selecciona las casillas de categorías de etiquetas específicas.
- **Exploración de código:** Activa la exploración de código para bloquear instrucciones que incluyen código fuente (mínimo 5 líneas). Para más información, consulta Exploración de código.

Los cambios surten efecto de inmediato.

**¿Qué pasa con las instrucciones después de cambiar la configuración?**

Los elementos recién desbloqueados pasarán. Los elementos que aún coincidan con patrones bloqueados permanecerán detenidos.

**Experiencia del usuario**

**¿Qué ve un usuario cuando una instrucción es bloqueada?**

Aparece un mensaje de política donde ingresaron la instrucción, y la solicitud no se envía a ningún LLM.

**¿Se escanea el contenido no textual (por ejemplo, imágenes)?**

No. Por el momento, el Bloqueo de Instrucciones solo soporta contenido basado en texto.

**Interacciones con otros controles**

**¿Cómo funciona el Bloqueo de Instrucciones con las barreras de protección y la moderación?**

- **Barreras de protección inteligentes:** Si se aplica "Bloquear uso de Miro AI", la IA se deshabilita; el bloqueo de instrucciones no se activa porque no se pueden enviar.
- **Moderación de IA:** Ambos se pueden aplicar cuando la IA está disponible: el bloqueo de instrucciones evita el uso de datos sensibles; la moderación filtra categorías dañinas.
- **Controles administrativos granulares:** El acceso a las funciones se aplica solo cuando la IA está disponible y las instrucciones no están bloqueadas.

##

## Integración de Enterprise Guard y Microsoft Purview DSPM para IA

Para las organizaciones que usan Microsoft Entra ID (anteriormente Azure AD) como su proveedor de identidad, Enterprise Guard reenvía de forma segura las instrucciones y respuestas de la IA a Microsoft Purview Data Security Posture Management (DSPM) para IA. Los equipos de seguridad y cumplimiento pueden luego monitorear, auditar y controlar el uso de la IA generativa desde una única plataforma confiable, reduciendo los costos operativos, mitigando riesgos como fuga de datos y uso indebido, y fortaleciendo la gestión de IA de nivel empresarial de Miro. Para más información, consulta la [documentación de integración de Enterprise Guard y Microsoft Purview DSPM para IA](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Propósito y alcance**

**¿Qué es la integración de Microsoft Purview DSPM para IA en Miro?**

Una integración que envía las instrucciones y respuestas de Miro AI a DSPM para IA de Microsoft Purview, permitiendo a los equipos de seguridad y cumplimiento monitorear, auditar y gobernar la actividad de IA en un solo lugar.

**¿Quién puede usar esta integración?**

Planes Enterprise con Enterprise Guard, gestionados por admins de empresa con acceso a integraciones Enterprise. Tu organización de Miro debe usar Microsoft Entra ID para inicio de sesión único. Se requiere una licencia de Microsoft Purview.

**¿Cuáles son los beneficios?**

Visibilidad centralizada del uso de Miro AI en el centro de IA de Purview, auditabilidad de instrucciones y respuestas, y alineación con tus políticas de gobernanza existentes en Purview.

**¿Qué actividad de Miro AI se incluye hoy?**

Por el momento, las instrucciones basadas en texto y las respuestas a través de las funciones de Miro AI son enviadas. El contenido de imágenes no está incluido.

**¿Se registran todas las actividades de los usuarios?**

Solo se reenvía la actividad de los usuarios que inician sesión en Miro a través del inquilino configurado de Microsoft Entra a Purview.

**¿Cuánto tiempo tarda la actividad en aparecer en Purview?**

Normalmente de 10 a 30 minutos después de la acción de IA en Miro. Puedes verla en Microsoft Purview → DSPM para IA → Explorador de Actividad, o verificar los registros de auditoría.

**¿Existen limitaciones notables?**

Por el momento, solo un inquilino de Entra puede ser configurado a la vez. En entornos con múltiples IdP o múltiples inquilinos, solo se registra a los usuarios que se autentican a través del inquilino configurado. Las imágenes no están incluidas.

**Configuración y ajuste**

**¿Cómo habilito la integración?**

En Miro: Configuración de Enterprise → Integraciones de Enterprise → activar Microsoft Purview DSPM para IA → ingresar tu ID de tenant de Entra → Conectar → iniciar sesión con una cuenta que pueda otorgar consentimiento de admin a nivel de tenant → aceptar la aplicación de gobernanza de Miro AI → confirmar Conectado en Miro.

**¿Cuáles son los requisitos previos?**

- **Miro:** Plan Enterprise con Enterprise Guard, rol de admin de empresa, ID de Entra configurado para inicio de sesión único. Para habilitar esta función, contacta a tu gerente de Customer Success.
- **Microsoft:** Licencia Microsoft Purview, el ID de tenant de Entra utilizado para el inicio de sesión único de Miro y un rol de Entra que pueda otorgar consentimiento de admin a nivel de tenant.

**¿Cómo verifico que la configuración funciona?**

Realiza una acción simple con Miro AI, espera 10–30 minutos, luego verifica en Microsoft Purview → DSPM para IA → Explorador de actividad para ver nuevas entradas de Miro.

**¿Cómo desconecto o cambio de inquilinos?**

En Miro: Integraciones Enterprise → Microsoft Purview para IA → Desconectar. Para cambiar de inquilinos, primero desconéctate, luego reconéctate usando el nuevo ID de inquilino.

**Uso y gobernanza**

**¿Dónde puedo ver los datos enviados en Purview?**

Microsoft Purview → DSPM para IA → Explorador de actividades. También puedes revisar los detalles en los registros de auditoría.

**¿Puedo exportar o archivar los registros de actividad de IA?**

Usa las herramientas de exportación de Microsoft Purview. Miro envía la actividad a tu tenant de Microsoft donde se aplican tus políticas.

**¿Puedo aplicar políticas de Purview a los datos de Miro AI?**

Sí. Una vez ingeridos, los datos siguen el modelo de gobernanza de Purview de tu organización.

**¿Qué pasa con las responsabilidades de privacidad y seguridad?**

Miro envía las instrucciones y respuestas a tu tenant de Microsoft. La gobernanza y los controles de acceso se gestionan en Purview dentro de tu entorno.

**Resolución de problemas y soporte**

**El paso de consentimiento falla o se repite. ¿Qué debo verificar?**

Asegúrate de que la cuenta usada para Connect pueda otorgar consentimiento administrativo a nivel del inquilino en Entra, o involucra a un administrador global de Microsoft.

**No veo actividad en Purview. ¿Qué hago ahora?**

Confirma que Enterprise Guard está habilitado y que tienes acceso a las integraciones de Enterprise. Verifica que el ID de tu inquilino coincida exactamente con tu inquilino de inicio de sesión único de Miro. Asegúrate de que un usuario haya realizado una acción de IA de prueba autenticándose a través de ese inquilino. Revisa las licencias y filtros de Purview. Permite hasta 30 minutos para la ingestión.

**Usamos múltiples IdP o inquilinos. ¿Se registrarán todos los usuarios?**

No. Solo se reenvía la actividad de los usuarios que inician sesión a través del único inquilino de Entra configurado.

**¿Quién brinda soporte para qué?**

Contacta el Soporte de Miro para la configuración o conectividad en Miro. Para incidencias dentro de Microsoft Purview, contacta el Soporte de Microsoft.
