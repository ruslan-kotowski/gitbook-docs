---
title: Funcionalidades de confianza de la IA y FAQ
article_id: 30943405198994
translation_id: 30943405198994
locale: es
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:32:10Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-granular-admin-settings
---

En Canvas 25, anunciamos el espacio de innovación impulsado por IA con flujos de trabajo visuales de IA y agentes colaborativos de IA en el lienzo. Además de las funciones para el usuario final, estamos introduciendo nuevas capacidades de administrador para brindarte mayor visibilidad, controles más inteligentes y formas sencillas de desbloquear las herramientas más recientes de IA de Miro para tus equipos.

Utiliza esta página para explorar las funcionalidades de confianza de IA disponibles con el complemento Enterprise Guard. Cada sección comienza con una breve descripción general, seguida de preguntas frecuentes expandibles que cubren diferentes aspectos de cada funcionalidad.

- Controles de admin granulares de Miro AI: establece acceso a nivel de funciones (Todos/Nadie/Equipos específicos) dentro de cada categoría de funcionalidades.
- [Bloquear el uso de Miro AI con Barreras de Protección Inteligentes](#h_block_ai_with_guardrails): usa Barreras de Protección Inteligentes para bloquear todas las interacciones impulsadas por IA en Miro cuando necesites proteger datos sensibles o clasificados.
- [Panel de Estadísticas generales de admin](#h_admin_analytics_overview): realiza un seguimiento de tableros, usuarios, equipos, licencias y plantillas con tendencias históricas y actualizaciones diarias.
- Moderación de IA (también disponible en la categoría Enterprise): establece niveles de filtrado para toda la organización (Estricto, Predeterminado, Mínimo) para seleccionar instrucciones que podrían dar lugar a resultados nocivos o inapropiados.
- Bloqueo de instrucciones: bloquea las instrucciones que contengan datos sensibles o código fuente en el momento de su envío; muestra un mensaje de política en lugar de enviar a un LLM.
- Enterprise Guard e integración con Microsoft Purview DSPM para IA: reenvía instrucciones y respuestas a Purview para una supervisión centralizada, auditoría y gobernanza.

## Controles de admin granulares de Miro AI para el complemento Enterprise Guard

Los controles administrativos de Miro IA permiten a los admins de empresa de Enterprise decidir qué capacidades de IA están disponibles en su organización y gestionar quién puede utilizarlas. Los admins también pueden ver los modelos que impulsan cada función de IA. Con el complemento Enterprise Guard, los controles de Miro IA se extienden al nivel de funciones dentro de cada categoría de funcionalidades, lo que ayuda a priorizar las funciones según las necesidades de la organización y los requisitos de seguridad. Además de la categoría completa de funcionalidades de Miro IA, los admins también pueden habilitar, restringir o eliminar funciones específicas de Miro IA. Por ejemplo, dentro de la categoría Imágenes, puedes habilitar "Crear imágenes con IA" y deshabilitar "Eliminar fondo". Utiliza estos controles para implementar la IA de manera segura y cumplir con los requisitos de seguridad mientras fomentas la adopción de las capacidades de IA. Para más información, consulta la [documentación sobre los controles administrativos granulares de Miro IA](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Propósito y alcance**

**¿Qué es el control granular para Miro AI?**

Con el complemento Enterprise Guard, los admins de empresa pueden habilitar, restringir o eliminar el acceso a funciones individuales de IA dentro de cada categoría de funcionalidades. Esto te permite elegir exactamente qué funciones pueden usar los equipos.

**¿Por qué usar controles granulares?**

Para equilibrar la adopción con la seguridad. Por ejemplo, dentro de Imágenes puedes permitir Crear imágenes mientras desactivas Eliminar fondo.

**Acceso y requisitos previos**

**¿Quién puede configurar los controles granulares y en qué planes?**

Los admins de la compañía en planes Enterprise con el complemento de Enterprise Guard, en el navegador.

**¿Dónde administro el acceso a nivel de función?**

Consola de administración → Miro AI → Funcionalidades. Expande una funcionalidad para ver y configurar el acceso a sus funciones individuales.

**Controles y comportamiento**

**Controles granulares: ¿cuál es la diferencia entre control a nivel de funcionalidad y control a nivel de función, y qué ocurre cuando los activo o desactivo?**

- **Nivel de funcionalidad:** Todos, Nadie o Equipos específicos se aplica a toda la categoría. Si desactivas una funcionalidad, los usuarios pierden acceso a esa funcionalidad y a todas sus funciones en los tableros. Si desactivas todas las funcionalidades, "Crear con IA" aparece deshabilitado en el tablero.
- **Nivel de función:** Con Enterprise Guard, puedes configurar Todos, Nadie o Equipos específicos por función individual. Desactivar una función elimina el acceso solo a esa función; las otras funciones de la misma funcionalidad permanecen disponibles si están habilitadas.

**¿Qué opciones de acceso existen a nivel de función?**

Para cada función, elige Todos, Ninguno, o Equipos específicos. Todos habilita la función en toda la organización y anula las restricciones a nivel de equipo. Ninguno elimina el acceso para todos los usuarios. Equipos específicos se enfoca solo en los equipos seleccionados.

**¿Qué sucede cuando desactivo una función individual?**

Los usuarios no pueden acceder a esa función en ningún tablero, pero otras funciones en la misma capacidad permanecen disponibles si están habilitadas.

**Referencia y ejemplos**

**¿Qué funciones puedo controlar individualmente?**

Consulta la referencia en el producto para la lista actual. Ejemplos bajo Crear contenido incluyen Crear notas adhesivas, Agrupar notas adhesivas, Crear y editar documentos, tablas, diagramas y operaciones de texto como reescribir, acortar, tono y traducir. Imágenes incluye Crear imágenes, Eliminar fondo y Añadir subtítulos. Resumir actividad incluye Ponerse al día y Resumen de conversaciones. Flujos, compañeros de IA, y Prototipos aparecen si están habilitados para tu organización.

**¿Puedo ver qué modelos impulsan funciones específicas?**

Sí. Los admins pueden ver los modelos asociados a cada función de IA en el área de referencia para apoyar la revisión y gobernanza.

## Bloquear el uso de Miro AI con barreras de protección inteligentes

Usa las Barreras de Protección Inteligentes para bloquear todas las interacciones impulsadas por IA en Miro cuando necesitas proteger datos sensibles o clasificados. Cuando se aplica esta barrera de protección, todas las herramientas de Miro AI se deshabilitan en los tableros afectados, mientras la colaboración sin IA sigue disponible. Para obtener más información y configuración, consulta el resumen de las Barreras de Protección Inteligentes y Define barreras de protección.

**Propósito y alcance**

**¿Qué hace "Bloquear el uso de Miro AI"?**

Deshabilita todas las funciones de Miro AI (por ejemplo, generación de texto, generación/reconocimiento de imágenes, sugerencias inteligentes) donde este guardarraíl se aplica, previniendo cualquier interacción impulsada por IA con contenido sensible o clasificado.

**¿Qué sigue disponible para los usuarios?**

Los usuarios pueden continuar con la colaboración regular, no basada en IA. El contenido generado por IA existente permanece en los tableros y puede ser visto, movido o editado manualmente, pero los usuarios no pueden usar Miro AI para modificarlo o regenerarlo.

**Acceso y requisitos previos**

**¿Quién puede configurar esta barrera de protección y dónde?**

Los admins de contenido sensible configuran las barreras de protección en *Enterprise Guard* bajo Clasificación de Datos → Barreras de Protección. (Los admins de empresa asignan el rol de admin de contenido sensible).

**¿Qué necesito antes de asignar esta barrera de protección?**

Define tus niveles de clasificación y (opcionalmente) la clasificación automática para que la barrera de protección pueda aplicarse por clasificación (por ejemplo, INTERNO, CONFIDENCIAL).

**Comportamiento e impacto**

**¿Quién se ve afectado cuando se aplica el guardrail?**

Todos, incluidos los propietarios de tableros y los copropietarios, no pueden acceder ni invocar Miro AI en los tableros afectados.

**¿Se elimina el contenido de IA existente?**

No. Impide más interacciones con IA; el contenido de IA existente sigue disponible para ver y editar manualmente.

**¿Cuándo entran en efecto los cambios?**

Después de que publiques las actualizaciones de tu guardrail, la aplicación es inmediata en los tableros afectados.

**Configuración y ajuste**

**¿Cómo activo "Bloquear el uso de Miro AI" para una clasificación?**

1. Ve a *Enterprise Guard* → Clasificación de Datos → **Guías de protección**.
2. Haz clic en el icono **Editar** para un nivel de clasificación (por ejemplo, CONFIDENCIAL).
3. Selecciona la casilla **Bloquear el uso de Miro AI** y **Hecho**.
4. Haz clic en **Siguiente** y revisa el impacto, luego **Publicar** para aplicar.

**¿Debería usar el modo Predeterminado o Estricto?**

En el modo Predeterminado, las barreras de protección no anulan la configuración de uso compartido existente. En el modo Estricto, las barreras de protección anulan el uso compartido activo y aplican los controles más estrictos. Elige en función de tus necesidades de gestión del cambio.

**Experiencia del usuario**

**¿Qué verán los usuarios en los tableros donde se bloquea la IA?**

Los puntos de entrada de Miro IA aparecen deshabilitados o no disponibles, y los usuarios no pueden invocar herramientas de IA desde el lienzo o menús en esos tableros.

**¿Pueden los usuarios solicitar excepciones en un solo tablero?**

No. La barrera de protección se aplica por política de clasificación. Cambia la clasificación del tablero (o la política para ese nivel) para modificar la aplicación.

**Interacciones con otros controles**

**¿Cómo se relaciona esto con los controles de admin granulares de Miro AI?**

Los controles granulares gestionan quién puede usar funciones específicas de IA. El guardrail es una capa de política: cuando está activa, bloquea la IA sin importar los interruptores de funciones.

**¿En qué se diferencia esto del bloqueo de instrucciones o de la Moderación de IA?**

- **Bloqueo de instrucciones** detiene instrucciones sensibles en el momento de su envío; la IA sigue disponible para instrucciones no sensibles.
- **Moderación de IA** filtra contenido dañino o inapropiado.
- **Bloqueo del uso de Miro AI** deshabilita completamente la IA en los tableros afectados.

**Resolución de problemas**

**La IA aún aparece en algunos tableros. ¿Qué debo verificar?**

- Confirma que la clasificación del tablero es una donde la barrera de protección está habilitada y que hiciste clic en **Publicar** después de editar las barreras de protección.
- Si usas la clasificación automática, verifica que la clasificación del tablero se haya actualizado en base al contenido actual.
- En los modos Estricto vs Predeterminado, asegúrate de que tus expectativas coincidan con el modo de implementación que seleccionaste.

**Necesitamos reactivar la IA para un subconjunto de trabajo.**

Ajusta la barrera de protección para la clasificación relevante o reclasifica los tableros que deben permitir la IA, y luego publica la actualización.

## Panel de estadísticas generales de administración

**Alcance y métricas**

**¿Qué cubre el panel de vista general?**

Tableros, usuarios, equipos, licencias y plantillas, con tendencias históricas donde corresponda.

**¿Cómo se define “Activo en este período” para Tableros, Usuarios y Equipos?**

- **Tableros:** Tableros únicos abiertos desde el inicio del período seleccionado. Incluye tableros que luego se movieron a la papelera.
- **Usuarios:** Usuarios únicos que abrieron un tablero al menos una vez desde el inicio del período. Incluye usuarios que ahora están desactivados.
- **Equipos:** Equipos únicos con al menos un miembro que abrió un tablero desde el inicio del período. Puede incluir equipos que luego se movieron a la papelera.

**¿Los totales excluyen los elementos en la papelera?**

Sí. Los totales para Tableros y Equipos excluyen los elementos que actualmente están en la papelera. Los recuentos históricos de "activos" pueden incluir elementos que luego fueron movidos a la papelera.

**¿Qué muestra el gráfico de Licencias?**

Totales y historial de asignación para las licencias Full, Free y de licencia gratuita limitada, reflejando cuántas licencias están actualmente en uso.

**¿Qué muestran las plantillas hoy?**

Las plantillas más populares utilizadas dentro de un tablero. Otras fuentes pueden añadirse en futuras versiones.

**Comportamiento de tiempo e historial**

**¿Cómo se muestran los valores históricos en los gráficos del Resumen?**

Los widgets históricos muestran los valores al último día de cada período. Está disponible hasta un año de historial o hasta donde existan datos.

**Actualización de datos y controles**

**¿Con qué frecuencia se actualizan los datos de Overview y dónde puedo verlo?**

Al menos una vez cada 24 horas. Un sello de “Última actualización” está disponible en el panel.

**¿Cómo cambio el rango de tiempo?**

Usa el selector de rango de tiempo en la parte superior derecha de la página de Estadísticas.

## Moderación de Miro AI

Con la moderación de Miro IA, los admins de empresa pueden ajustar los niveles de filtrado de las instrucciones que podrían contener texto potencialmente dañino o inapropiado. Puedes establecer una sensibilidad de moderación de Miro IA a nivel organizacional para filtrar contenido, incluyendo odio, contenido sexual, violencia y autolesiones. Esto te ayuda a alinear el uso de Miro IA con los requisitos, políticas y tolerancia al riesgo de tu organización. Para más información, consulta la [documentación de moderación de Miro IA](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Propósito y alcance**

**¿Qué es la Moderación IA en Miro?**

La Moderación IA permite a los admins de empresa establecer un nivel de filtrado para toda la organización (Estricto, Predeterminado o Mínimo) que examina instrucciones que podrían dar lugar a contenido dañino o inapropiado (por ejemplo, odio, contenido sexual, violencia, autolesión).

**¿Quién puede configurarlo y en qué planes?**

Los admins de empresa que tienen Enterprise con Enterprise Guard pueden configurar la opción en la configuración de la organización.

**¿Funciona si mi organización conecta su propio LLM (por ejemplo, una integración directa con un proveedor)?**

Si se conecta un LLM personalizado, el selector de moderación puede estar deshabilitado para esa integración y cualquier nivel seleccionado previamente no se aplicará a ella.

**Acceso y requisitos previos**

**¿Quién puede activarlo y qué necesito?**

Los admins de la empresa en el plan Enterprise con el complemento Enterprise Guard pueden configurar la Moderación de IA en la configuración de la organización.

**¿Cómo lo enciendo?**

Ve a Configuración → Miro AI → Moderación, elige Estricto/Predeterminado/Minimizado, y luego haz clic en **Guardar cambios**. La aplicación es inmediata para toda la organización.

**Niveles y comportamiento**

**¿Qué significan los niveles?**

- **Estricto:** Bloquea el contenido predeterminado + de bajo a moderado riesgo (por ejemplo, odio sutil/codificado, contenido sexual sugestivo, violencia no gráfica, menciones de autolesiones no explícitas).
- **Predeterminado (recomendado):** Bloquea contenido moderadamente a severamente dañino.
- **Minimal:** Bloquea solo contenido severamente dañino.

**¿Cuándo se hacen efectivas las modificaciones?**

De inmediato para toda la organización.

**¿Se rastrean los cambios?**

Sí. Las actualizaciones se registran en el registro de auditoría de tu organización.

**Configuración y ajustes**

**¿Dónde configuro o actualizo el nivel de moderación?**

Ve a Preferencias → Miro AI → Moderación, elige Estricto/Por defecto/Mínimo, y luego haz clic en **Guardar cambios**.

**¿Qué nivel de inicio recomiendas?**

El nivel por defecto se adapta a la mayoría de las organizaciones; ajústalo según las opiniones del piloto y la tolerancia al riesgo.

**Interacciones con otros controles**

**¿Cómo se relacionan la Moderación de IA con las barreras de protección e instrucciones?**

- **Barreras de protección inteligentes:** Si un tablero está cubierto por la barrera de protección "Bloquear el uso de Miro AI", la IA se deshabilita independientemente del nivel de moderación.
- **Bloqueo de instrucciones:** Funciona junto con la Moderación. El bloqueo de instrucciones detiene las instrucciones sensibles en la presentación; la Moderación filtra las categorías dañinas.
- **Controles administrativos granulares:** Los interruptores de funciones gobiernan quién puede acceder a las funciones de IA cuando esta está disponible.

**Resolución de problemas y mejores prácticas**

**Estamos viendo demasiados falsos positivos.**

Considera cambiar de Estricto → Predeterminado (o Predeterminado → Mínimo) y publicar ejemplos de uso aceptable. Si los problemas persisten después de ajustar la configuración, contacta a tu gerente de Customer Success de Miro para informar esto, de modo que nuestro equipo de producto pueda revisarlo.

**Estamos viendo que se escapa contenido dañino.**

Cambia a Predeterminado o Estricto y proporciona orientación interna. Revisa nuevamente después de las actualizaciones de política/regulación. Si los problemas continúan después de estos cambios, contacta a tu gerente de Customer Success de Miro para informar esto, de modo que nuestro equipo de producto pueda revisarlo.

## Bloqueo de instrucciones

El bloqueo de instrucciones permite a los administradores de contenido sensible evitar que los usuarios envíen instrucciones de IA que incluyan información sensible, ayudando a mantener los datos confidenciales fuera de Miro AI en toda tu organización. Miro escanea el texto que un usuario ingresa en el campo de instrucciones y cualquier contenido basado en texto que agreguen desde el tablero. Si ese contenido coincide con las etiquetas de sensibilidad o patrones de código fuente seleccionados en la configuración de bloqueo de instrucciones, Miro bloquea el envío de la instrucción. Para más información, consulta la [documentación sobre bloqueo de instrucciones](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Propósito y alcance**

**¿Qué es el Bloqueo de Instrucciones?**

El Bloqueo de Instrucciones impide a los usuarios enviar instrucciones de IA que incluyan información sensible. Miro escanea el texto que un usuario teclea en el campo de instrucción y cualquier contenido basado en texto que agreguen desde el tablero; si coincide con las etiquetas de sensibilidad o patrones de código fuente seleccionados, se bloquea el envío y se muestra un mensaje de política. Por el momento, solo admitimos contenido basado en texto.

**¿En qué se diferencia el Bloqueo de Instrucciones del escaneo de tableros?**

El escaneo de tableros encuentra contenido sensible en los tableros y puede autoclasificar tableros; el Bloqueo de Instrucciones verifica lo que los usuarios intentan enviar a Miro AI en el momento del envío.

**¿Qué etiquetas de sensibilidad son compatibles?**

Usa las categorías a nivel de la organización listadas en las etiquetas e infotypes de Sensibilidad.

**¿Qué es la Escaneo de Código?**

El Escaneo de Código bloquea las instrucciones que contienen código fuente reconocible; por diseño, requiere un bloque mínimo de código (por ejemplo, 5 o más líneas) para activarse. Actívelo o desactívelo en la configuración de Bloqueo de Instrucciones.

**¿Se escanea contenido no textual (por ejemplo, imágenes)?**

No. En este momento, el Bloqueo de Instrucciones sólo admite contenido basado en texto.

**Acceso y requisitos previos**

**¿Quién puede activarlo y qué necesito?**

Los admins de Contenido Sensible en Plan Enterprise con el complemento Enterprise Guard pueden activarlo en Configuración → Enterprise Guard → Descubrimiento de datos → Configuración.

**¿Cómo lo activo?**

Abre Bloqueo de instrucciones → Activar, elige Seleccionar todo o categorías de etiquetas específicas, opcionalmente habilita Escaneo de código, luego Activar. La aplicación es inmediata para toda la organización.

**Gestión y cambios**

**¿Cómo ajusto las etiquetas o el Escaneo de Código más tarde?**

Ve a Configuración → Enterprise Guard → descubrimiento de datos → Configuración → Bloqueo de instrucciones → Gestionar,

- **Etiquetas:** Marca la casilla *Seleccionar todas* para seleccionar todas las categorías o selecciona las casillas de categorías de etiquetas específicas.
- **Escaneo de Código:** Activa el Escaneo de Código para bloquear instrucciones que incluyan código fuente (mínimo 5 líneas). Para más información, consulta Escaneo de Código.

Los cambios se aplican de inmediato.

**¿Qué sucede con las instrucciones después de cambiar la configuración?**

Los elementos recién desbloqueados pasarán. Los elementos que aún coincidan con patrones bloqueados permanecerán detenidos.

**Experiencia del usuario**

**¿Qué ve un usuario cuando se bloquea una instrucción?**

Aparece un mensaje de política donde ingresaron la instrucción, y la solicitud no se envía a ningún LLM.

**¿Se escanea contenido no textual (por ejemplo, imágenes)?**

No. Por el momento, el bloqueo de instrucciones solo admite contenido basado en texto.

**Interacciones con otros controles**

**¿Cómo funcionan las instrucciones bloqueadas con las barreras de protección y la moderación?**

- **Barreras de protección inteligentes:** Si se aplica "Deshabilitar el uso de Miro AI", la IA se deshabilita; El bloqueo de instrucciones no se activará porque no se pueden enviar instrucciones.
- **Moderación de IA:** Ambos pueden aplicarse cuando la IA está disponible—El bloqueo de instrucciones detiene datos sensibles; la moderación filtra categorías dañinas.
- **Controles de administración granulares:** El acceso a las funciones se aplica solo cuando la IA está disponible y la instrucción no está bloqueada.

##

## Enterprise Guard y Microsoft Purview DSPM para la integración de IA

Para las organizaciones que utilizan Microsoft Entra ID (anteriormente Azure AD) como su proveedor de identidad, Enterprise Guard reenvía de manera segura las instrucciones de IA y las respuestas a Microsoft Purview Data Security Posture Management (DSPM) para IA. Los equipos de seguridad y cumplimiento pueden entonces monitorear, auditar y controlar el uso de IA generativa desde una única plataforma confiable, reduciendo la carga operativa, mitigando riesgos como fugas de datos y uso indebido, y fortaleciendo la gobernanza de IA a nivel empresarial de Miro. Para obtener más información, consulta la [documentación sobre la integración de Enterprise Guard y Microsoft Purview DSPM para IA](../integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Propósito y alcance**

**¿Qué es la integración de Microsoft Purview DSPM para IA en Miro?**

Una integración que envía las instrucciones y respuestas de Miro AI a DSPM para IA de Microsoft Purview, para que los equipos de seguridad y cumplimiento puedan monitorear, auditar y gobernar la actividad de IA en un solo lugar.

**¿Quién puede utilizar esta integración?**

Planes Enterprise con Enterprise Guard, administrados por admins de empresa con acceso a integraciones de Enterprise. Tu organización de Miro debe usar Microsoft Entra ID para inicio de sesión único. Se requiere una licencia de Microsoft Purview.

**¿Cuáles son los beneficios?**

Visibilidad centralizada del uso de Miro AI en el centro de IA de Purview, auditabilidad de instrucciones y respuestas, y alineación con tus políticas de gobernanza existentes en Purview.

**¿Qué actividad de Miro AI se incluye hoy?**

Por el momento, se envían las instrucciones y respuestas basadas en texto de las funciones de Miro AI. El contenido de las imágenes no se envía.

**¿Se registran las actividades de todos los usuarios?**

Solo la actividad de los usuarios que inician sesión en Miro a través del tenant de Microsoft Entra configurado se envía a Purview.

**¿Cuánto tarda en aparecer la actividad en Purview?**

Generalmente entre 10 y 30 minutos después de la acción de IA en Miro. Puedes verlo en Microsoft Purview → DSPM para IA → Explorador de actividades, o verificar los registros de auditoría.

**¿Hay limitaciones notables?**

Por el momento, solo se puede configurar un tenant de Entra a la vez. En entornos con múltiples IdPs o tenants, solo se registran los usuarios que se autentican a través del tenant configurado. Las imágenes no están incluidas.

**Configuración y ajuste**

**¿Cómo habilito la integración?**

En Miro: Configuración de Enterprise → Integraciones de Enterprise → activa Microsoft Purview DSPM para IA → introduce tu ID de tenant de Entra → Conectar → inicia sesión con una cuenta que pueda otorgar consentimiento de administrador a nivel de tenant → acepta la aplicación de gobernanza de Miro AI → confirma Conectado en Miro.

**¿Cuáles son los requisitos previos?**

- **Miro:** Plan Enterprise con Enterprise Guard, rol de admin de empresa, ID de Entra configurado para SSO. Para habilitar esta función, contacta a tu gerente de Customer Success.
- **Microsoft:** Licencia de Microsoft Purview, el ID de tenant de Entra utilizado para SSO de Miro, y un rol de Entra que pueda otorgar consentimiento de administrador a nivel de tenant.

**¿Cómo verifico que la configuración funcione?**

Realiza una acción simple con Miro AI, espera de 10 a 30 minutos, luego revisa Microsoft Purview → DSPM para IA → Explorador de actividad para nuevas entradas de Miro.

**¿Cómo desconecto o cambio de inquilino?**

En Miro: Integraciones Enterprise → Microsoft Purview para IA → Desconectar. Para cambiar de inquilino, desconecta primero y luego reconecta usando el nuevo ID de inquilino.

**Uso y gobernanza**

**¿Dónde puedo ver los datos reenviados en Purview?**

Microsoft Purview → DSPM para IA → Explorador de actividades. También puedes revisar los detalles en los registros de auditoría.

**¿Puedo exportar o archivar registros de actividades de IA?**

Utiliza las herramientas de exportación de Microsoft Purview. Miro reenvía la actividad a tu tenant de Microsoft donde se aplican tus políticas.

**¿Puedo aplicar políticas de Purview a los datos de Miro AI?**

Sí. Una vez ingeridos, los datos siguen el modelo de gobernanza de Purview de tu organización.

**¿Qué pasa con las responsabilidades de privacidad y seguridad?**

Miro reenvía las instrucciones y respuestas a tu tenant de Microsoft. La gobernanza y los controles de acceso se gestionan en Purview dentro de tu entorno.

**Resolución de problemas y soporte**

**El paso de consentimiento falla o se repite. ¿Qué debo verificar?**

Asegúrate de que la cuenta utilizada para Connect pueda otorgar consentimiento de administrador a nivel de inquilino en Entra, o involucra a un administrador global de Microsoft.

**No veo actividad en Purview. ¿Qué hacer ahora?**

Confirma que Enterprise Guard esté habilitado y tengas acceso a integraciones Enterprise. Verifica que tu ID de inquilino coincida exactamente con tu inquilino de inicio de sesión único de Miro. Asegúrate de que un usuario autenticado a través de ese inquilino haya realizado una acción de prueba de IA. Revisa la licencia y los filtros de Purview. Espera hasta 30 minutos para la ingestión.

**Utilizamos múltiples IdP o inquilinos. ¿Se registrarán todos los usuarios?**

No. Solo se reenvían actividades de usuarios que inicien sesión mediante el único inquilino Entra configurado.

**¿Quién soporta qué?**

Contacta con el Soporte de Miro para la configuración o conectividad en Miro. Para problemas dentro de Microsoft Purview, contacta con el Soporte de Microsoft.
