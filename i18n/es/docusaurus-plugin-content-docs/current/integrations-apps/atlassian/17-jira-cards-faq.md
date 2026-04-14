---
title: Preguntas frecuentes sobre las tarjetas de Jira
article_id: 360013463739
translation_id: 8247569704594
locale: es
sidebar_position: 17
created_at: '2022-10-24T14:58:39Z'
updated_at: '2025-10-14T19:23:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Este artículo responde a las preguntas más populares sobre cómo se crea la integración de tarjetas de Jira.

**Seguridad**

**¿Cómo funciona la autenticación Jira-Miro?**

Consulta los artículos del Centro de Ayuda para

- **Servidor de Jira en las instalaciones**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Terceros) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Centro de Datos de Jira en las instalaciones**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Terceros) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Cloud**
  Selecciona desde la página de configuración de las tarjetas de Jira.
  - [OAuth 2.0](https://help.miro.com/hc/articles/8588617184402) (3LO)

**¿Los datos están protegidos en tránsito entre Jira y Miro?**

Usamos el protocolo de seguridad TLS. Cifra mensajes HTTP antes de la transmisión y los desencripta a su llegada. También soportamos TLS mutuo para [plan Enterprise](https://help.miro.com/hc/articles/360017730433).

**¿Proveen soporte para TLS mutuo?**

Sí, [más información](https://help.miro.com/hc/articles/4410562720658).

**¿Conservará Miro alguno de los datos de Jira del cliente?**

Sí, Miro conserva los datos de la tarjeta que se añaden al tablero.

**¿Cuánto tiempo dura el período de retención y cómo se aseguran los datos?**

Para OAuth 1.0. (Servidor de Jira o centro de datos), los datos se actualizan si los webhooks están configurados durante el proceso de configuración del complemento de tarjetas de Jira. El período de retención es ilimitado. Solo se aplican los protocolos de seguridad generales de Miro.

**¿Podemos restringir la información que se recupera de Miro?**

No encontramos ninguna mención en [la documentación de Atlassian](https://developer.atlassian.com/server/jira/platform/webhooks/) sobre cómo limitar la información a solo algunos campos.

**¿Podemos tener un diagrama que muestre el flujo de datos entre Jira y Miro?**

La información detallada se puede encontrar en [este artículo de Jira para desarrolladores](https://developer.atlassian.com/server/jira/platform/oauth/). Implementamos nuestra integración de acuerdo con la documentación de Atlassian.

**¿Cómo se maneja el token?**

Oauth 1.0: solo se usa el token de acceso. El token de acceso perdura [por 5 años a menos que](https://developer.atlassian.com/server/jira/platform/oauth) se revoque (no hay opción de personalizar, ya que esta política está definida en Atlassian. Puedes revocar el token desde Jira usando la interfaz de usuario web). Recuerda que cada nuevo token impide que la integración funcione y requiere [volver a conectar](https://help.miro.com/hc/articles/360019501754#Step_2_-_Connection) la integración.

OAuth 2.0: el token de acceso dura 1 hora. El token de actualización dura 90 días (si pasas 90 días sin usar la integración, tendrás que volver a autenticarte).

**¿Se usa un único token de acceso para todos los accesos a Jira del cliente?**

Todo usuario de Miro que tenga la intención de importar, crear o editar tarjetas de Jira debe conectar sus credenciales de Jira individuales. Todas las acciones anteriores solo se pueden realizar en nombre de credenciales de Jira individuales.

**¿Cómo se aseguran los tokens de solicitud, los tokens de acceso, las claves privadas y otros secretos/credenciales de OAuth?**

Durante la integración, solo se usan tokens de acceso. Se almacenan de forma segura dentro de la base de datos y se utilizan solo desde el servidor.

Para OAuth 1.0. (Servidor de Jira y centro de datos) el authToken solo se usa para el webhook. No es el token de autenticación real que utiliza OAuth. Las solicitudes se envían a través de una conexión cifrada. La clave secreta se genera automáticamente y se asocia según el equipo.

**¿Qué endpoints usa tu integración?**

```
POST /rest/api/2/issue - crear nueva incidencia
```

```
PUT /rest/api/2/issue/id - actualizar incidencia
```

```
GET /rest/api/2/user/picker?query=xx
```

```
GET /rest/api/2/myself
```

```
GET /rest/api/2/filter/favourite
```

```
GET /rest/api/2/issue/picker
```

```
GET /rest/api/2/serverInfo
```

```
GET /rest/api/2/issue/$key
```

```
GET /rest/api/2/issue/createmeta
```

```
GET /rest/api/2/issue/$key/editmeta
```

```
GET /rest/api/2/priority
```

```
GET /rest/api/2/issuetype
```

```
GET /rest/api/2/mypermissions
```

Para OAuth 1.0. (Servidor de Jira y centro de datos) además, usamos:

```
POST /rest/webhooks/1.0/webhook
```

**¿Funcionan las tarjetas con Jira Datacenter?**

Sí. Tenemos la aprobación de Atlassian y muchos de nuestros clientes ya usan tarjetas de Jira con Datacenter de manera exitosa. El procedimiento de instalación es el mismo.

**¿Qué IP usan actualmente para comunicarse con el sistema de Jira?**

La lista de nuestras direcciones IP estáticas se puede encontrar [aquí](https://help.miro.com/hc/articles/360017572694).

Ten en cuenta que estas son las direcciones utilizadas únicamente para comunicarse con el sistema de Jira. Las IP de la aplicación de Miro son dinámicas y, para asegurar que todas las funcionalidades de los tableros de Miro (incluidas algunas de las relacionadas con las tarjetas de Jira) se ejecuten con éxito, pedimos que [agregues nuestros dominios a la lista de admitidos](https://help.miro.com/hc/articles/360017572694).

**¿Podemos integrar Jira con Miro, pero bloquear las incidencias de Jira con nivel de seguridad configurado como "Privado"?**

No, esa opción no está disponible. Los niveles de seguridad en Jira no se correlacionan con Miro.

**General**

**¿Podemos conectar Miro a Jira si usamos un servidor de Jira?**

Dado que Miro es una herramienta online, solo puedes conectar a Jira cuando tu instancia está abierta al internet público.

**¿Podemos conectar múltiples instancias de Jira al mismo tiempo?**

Sí. Sin embargo, ten en cuenta que conectar una instancia de Jira se trata de establecer el enlace inicial, mientras que una conexión activa se refiere a la instancia vinculada que se está utilizando actualmente. Una conexión activa define de dónde se importan las tarjetas de Jira cuando abres la aplicación de tarjetas de Jira, y para qué instancia los usuarios están autorizados. Para un usuario determinado, solo puede haber una (1) conexión activa a la vez. Con OAuth 2.0, un usuario puede editar cualquier tarjeta de Jira asociada con cualquier instancia vinculada para la cual ya esté autenticado. Para cualquier otro protocolo de autenticación, un equipo entero comparte una instancia activa, y solo puede importar e interactuar con tarjetas de esa instancia. Puedes definir múltiples configuraciones a nivel de organización y cambiar entre conexiones activas a nivel de equipo.

**¿Qué es el proceso de migración de servidor a nube?**

Dado que la URL base de Jira cambiará inevitablemente durante la migración a la nube, la integración se interrumpirá sin cambios por nuestra parte. Por favor [contacta a la asistencia de Miro](https://help.miro.com/hc/articles/360020185799) para obtener ayuda.

**¿Creará Miro un webhook por equipo, por proyecto o por instancia de Miro?**

Si habilitas Webhook Automático en tus configuraciones de Miro, entonces la creación de webhooks ocurre de manera automática. Si utilizas autorización a nivel de equipo con Jira, entonces Miro crea webhooks por equipo. Si usas autorización a nivel de organización, entonces Miro crea webhooks por organización.

**¿El plugin de Tarjetas Jira es compatible con proyectos Next-Gen?**

Sí, es compatible.

Ten en cuenta que actualmente no hay enlace/campo Epic cuando se crea una Tarjeta Jira para un proyecto de Next-Gen desde Miro.

**¿Son compatibles los campos Jira personalizados?**

Sí, ofrecemos casi todos los campos personalizados de tipos *básicos*. Si tienes un campo de tipo de datos *complejo*, es posible que no sea compatible y cause algún comportamiento inesperado al actualizar o crear tarjetas de Jira en el tablero.

**¿Qué pasa con las tarjetas de Jira existentes si cambiamos a otra instancia de Jira?**

Actualmente, cuando mueves incidencias de Jira de un proyecto a otro en Jira, dejan de actualizarse en Miro.

Como solución, te recomendamos copiar la URL de la incidencia de Jira (Ctrl/Cmd+C) y pegarla en un tablero de Miro (Ctrl/Cmd+V). Así, una tarjeta de Jira mostrará nuevos valores y se actualizará automáticamente.

**Si un tablero se mueve a otro equipo de Miro, ¿qué pasa con las tarjetas de Jira de ese tablero?**

Las tarjetas de Jira permanecerán en el tablero, pero nadie podrá modificarlas (incluso si la misma instancia de Jira está configurada para el equipo objetivo).

Al hacer clic en una tarjeta, verás un mensaje: *"La tarjeta de Jira se importó desde otra cuenta"*. Si quieres que las tarjetas sean editables, impórtalas de nuevo al tablero.

**¿La integración de las tarjetas de Jira tiene algún costo adicional?**

Las tarjetas de Jira están disponibles en todos los planes de pago y Education sin costo adicional (Starter, Business, Education y Enterprise).

**¿Puede un usuario acceder a todas las tarjetas de Jira en el tablero?**

Los permisos para la integración de las tarjetas de Jira aseguran que los usuarios solo pueden crear y editar tarjetas en los proyectos de Jira a los que tengan acceso.

Como todos los widgets en un tablero de Miro son visibles para todos los que tienen acceso al tablero, si alguien no tiene credenciales de Jira o no tiene las credenciales correctas, podrán ver la tarjeta de Jira colapsada en un tablero de Miro (con título y algunos otros campos) pero no podrán expandir la tarjeta para revisarla completamente o modificarla.

**¿Ha descontinuado Atlassian el soporte para Jira Server?**

Sí, Atlassian ha descontinuado el soporte para Jira Server a partir de febrero de 2024.

**¿Soporta Miro Planificador/tarjetas de Jira los campos personalizados de Jira: Tipos de incidencia personalizados y Dependencias personalizadas?**

Sí, ambos son compatibles. Si los campos de **Tipos de incidencia personalizados** y **Dependencias personalizadas** están configurados en Jira, *y* el Miro Planificador está autenticado para esa instancia de Jira, entonces estos campos personalizados están disponibles en el planificador.

**¿Soporta Miro OAuth 2.0 para el Jira Data Center?**

Sí. Consulta [Conectar con Jira Data Center usando OAuth 2.0.](https://help.miro.com/hc/articles/25753304280466)

**Tarjetas de Jira en tablas y cronogramas**

**¿Cómo puedo importar incidencias de Jira a tablas y cronograma?**

Puedes arrastrar y soltar una o varias tarjetas de Jira directamente a una tabla o cronograma. Actualmente, esta es la única forma de hacerlo.

**¿Todos los campos en la tabla están vinculados con Jira?**

No, solo cinco campos en la tabla se sincronizan con Jira en el lanzamiento inicial:

Tres campos de sistema de Jira:

- Título
- Descripción
- Fecha de finalización (aparece como Fecha de vencimiento en Jira)

Dos campos personalizados de Jira:

- Fecha de inicio
- Estimación

**¿Qué campos en la tabla no se sincronizan con Jira?**

Los campos Asignado (Assignee) y Estado (Status) no se sincronizan con Jira y están deshabilitados en las tablas y el cronograma. Estos campos y su contenido existen, pero no son visibles ni editables en las tablas y el cronograma.

Aún puedes editar estos campos directamente en las tarjetas de Jira usando el panel lateral. Simplemente, arrastra la fila desde la tabla o el cronograma al lienzo para que tu tarjeta de Jira vuelva a aparecer.

Todos los demás campos, aparte de los cinco listados arriba (Título, Descripción, Fecha de fin, Fecha de inicio y Estimación), se almacenan solo en Miro y no se sincronizan con Jira.

**¿Por qué no puedo editar un campo en tabla o cronograma de los cinco campos de Jira admitidos arriba?**

El campo puede no estar presente en la pantalla de edición en Jira.

Un método fácil para saber si el campo está presente en la pantalla de edición o no:

En Miro, abre el panel lateral de la tarjeta de Jira. Verifica si el campo está presente en el panel lateral. Si el campo no está presente, debes añadir el campo a la pantalla de edición en Jira.

Existen algunos casos raros en los que los campos son editables en Jira, pero no están presentes en la pantalla de edición en Jira. En este caso, estos campos no pueden ser editados en Miro.

¿Es el campo que no puedes editar **Fecha de inicio** o **Estimación**? Si es así:

El campo puede no estar presente en Jira o faltar en la pantalla de edición (consulta el punto anterior)

Puede haber un problema de mapeo para Fecha de inicio o Estimación ya que son campos personalizados de Jira.

Mapeamos estos campos de acuerdo con esta lógica:

- **Fecha de inicio**: Verificamos los campos con los nombres: Start Date, StartDate, Target Start
- **Estimación**: Verificamos los campos con los nombres: Story Points, Story point estimate, Story Point, StoryPoints, StoryPoint
- Si el campo de Fecha de inicio o Estimación no lleva alguno de los nombres anteriores, esto podría explicar por qué la edición no funciona.

**¿Por qué no funciona la edición de la Fecha de Inicio o del Estimado en la Tabla o Cronograma de Miro o actualiza el campo incorrecto en Jira?**

Actualmente, dependemos de la creación automática de mapas para los campos de Fecha de Inicio y Estimado en Jira. Dado que estos son personalizados en Jira, puede ocurrir que varios campos en tu configuración de Jira coincidan con los criterios mencionados anteriormente.

Seleccionamos la primera coincidencia de acuerdo con el orden de nombres de campos mencionado anteriormente:

Por ejemplo, si un ticket de Jira tiene tanto campos de Puntos de Historia como de estimado de puntos de historia, coincidimos el primero según la lista anterior, que son los Puntos de Historia. Por lo tanto, cualquier cambio en el campo Estimado en la tabla actualizará el campo Puntos de Historia en Jira, no el estimado de puntos de historia.

De momento, no existe tal opción. Si experimentas este problema, envía comentarios a tu equipo de soporte para que podamos entender mejor tus necesidades mientras desarrollamos capacidades más avanzadas de mapeo de campos.

**¿Por qué no puedo importar tarjetas de Jira de 2 instancias diferentes en una tabla o cronograma?**

Actualmente solo admitimos una instancia de Jira por tabla/cronograma. Una vez que se importa una tarjeta de Jira en una tabla/cronograma, esta se vincula a esa instancia específica de Jira.

Incluso si se eliminan todos los registros de Jira, el enlace a la instancia original de Jira permanece. Para importar tarjetas de una instancia diferente de Jira, necesitas crear una nueva tabla/cronograma.

**¿Por qué no puedo ver o editar los campos de Estado y Responsable de mis registros de Jira en una tabla o cronograma?**

Actualmente los campos de Estado y Responsable de Jira no son compatibles en tablas y cronograma. Hemos decidido deshabilitar estos campos en tablas y cronograma para manejar expectativas, evitar confusiones y potencial pérdida de datos. Los campos de Estado y Responsable de Jira y su contenido existen, pero no aparecen en tablas o cronograma.

Aún puedes editar estos campos directamente en las tarjetas de Jira usando el panel lateral. Simplemente arrastra la fila de la tabla o cronograma al lienzo para que tu tarjeta de Jira reaparezca.

**Más información:**

- [Tarjetas de Jira](https://help.miro.com/hc/articles/360017572434)
- [Cómo configurar y desinstalar Tarjetas de Jira](https://help.miro.com/hc/articles/360019501754)
- [Cómo configurar webhook para Tarjetas de Jira](https://help.miro.com/hc/articles/360017731113)
- [Posibles problemas con Tarjetas de Jira y el complemento de Jira](https://help.miro.com/hc/articles/360017572654)
