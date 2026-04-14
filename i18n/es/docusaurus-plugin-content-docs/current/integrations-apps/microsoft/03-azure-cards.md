---
title: Tarjetas de Azure
article_id: 360033799934
translation_id: 360033799934
locale: es
sidebar_position: 4
created_at: '2019-08-13T10:01:30Z'
updated_at: '2025-11-25T16:05:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: azure-cards
availability:
  notes: 'Personas: Todos los usuarios Planes: Business y Enterprise Plataformas:
    Navegador, escritorio, móvil'
---

Las tarjetas Azure te permiten importar elementos de trabajo de los tableros de Azure (parte de los servicios Azure DevOps, anteriormente VSTS - solución en la nube) a tus tableros de Miro. Pueden convertirse en una parte esencial de tus retrospectivas remotas, estimaciones de tamaño de historias, priorización de trabajos pendientes, creación de mapas de historias y otras actividades de equipo. También puedes usarlos en los marcos de Miro Kanban y creación de mapas de historias de usuario.

Las tarjetas Azure mejoran tu experiencia en Miro al integrarse directamente con los tableros de Azure, permitiendo una gestión de flujo de trabajo sin interrupciones para diversas actividades del equipo.

## Características clave

La integración de las tarjetas de Azure ofrece varias funcionalidades clave:

- Importa tarjetas Azure usando el selector de elementos de trabajo de Azure Boards de la aplicación. Esto incluye varias opciones de clasificación
- Busca elementos de trabajo de Azure Boards en el selector de la aplicación
- La vista de tarjetas automatizada de fácil lectura cambia mientras acercas y alejas el zoom.

:::note
Asegura que tus tarjetas de Azure siempre estén actualizadas con el sondeo de tarjetas, lo que garantiza que los usuarios siempre reciban actualizaciones de tarjetas incluso si [los webhooks](../atlassian/14-how-to-set-up-webhooks-for-jira-data-center.md) fallan.
:::

## Configura la integración de tarjetas de Azure

Es necesario configurar en dos niveles:

1. La aplicación debe añadirse a nivel organizacional para todos los equipos, o añadirse a nivel de equipo para equipos específicos.
2. Después de que se añada la aplicación, la integración debe estar conectada y autorizada a nivel personal para importar Tarjetas Azure.

Este proceso requiere permisos administrativos específicos tanto en Miro como en Azure DevOps.

:::note
Para configurar exitosamente las tarjetas Azure con Miro, **el administrador de Azure y el administrador de Miro deben ser la misma cuenta**.

Ten en cuenta que agregar Tarjetas de Azure requiere permisos de Miro Team o Company Admin **y** permisos de grupo de Project Collection Admin en Azure Boards, pero estos permisos se pueden deshabilitar después de completar la conexión. Sin embargo, el admin no se puede eliminar y debe conservar el acceso al proyecto de Azure.
:::

### Agregar tarjetas de Azure para tu organización o equipo

Los admins de empresa de Miro pueden agregar Azure Cards para todos los equipos, mientras que los admins de equipo pueden hacerlo para los equipos específicos que gestionan. Este paso hace que la aplicación de Tarjetas Azure esté disponible para la conexión.

> Para conectar las tarjetas Azure a nivel del equipo, debes ser admin de equipo.

1. Navega a **Configuración de perfil** (haz clic en el ícono de hamburguesa del menú principal y elige **Configuración de perfil**, o desde el panel, haz clic en tu avatar en la esquina superior derecha y elige **Configuración**).
2. Haz clic en **Aplicaciones** y luego navega a la pestaña **Añadir aplicaciones** en el lado derecho.
3. Ingresa "Tarjetas Azure" y selecciónala de la lista desplegable. Haz clic en **Añadir**.
4. En el siguiente cuadro de diálogo, elige **Todos los equipos** o **En equipos específicos** (elige tu equipo si es necesario), luego haz clic en **Siguiente paso**.
5. En la pantalla "Review and add Azure Cards", haz clic en **Añadir**. La aplicación se agregará para tu empresa o equipo.
6. Ve a la pestaña **Manage apps**, busca Azure Cards y haz clic en **Approve**. La aplicación ahora será aprobada a nivel de empresa o equipo.
7. Luego, conecta tu organización de Azure a Miro. Desde el panel de aplicaciones, ve a **Manage Apps.**
8. Busca "Azure Cards" en tu lista de aplicaciones y haz clic en **Configuración.**
9. En el panel de configuración de las tarjetas Azure, agrega tu URL **de instancia Azure** y haz clic en **Connect**. Proporciona tus credenciales de inicio de sesión de Microsoft Azure.
10. En el cuadro de diálogo de autorización, haz clic en **Aceptar** para completar la conexión de Azure a Miro.

### Aplicar configuraciones personalizadas de tarjetas de Azure para equipos específicos

Si necesitas configuraciones diferentes para equipos específicos en lugar de la configuración global a nivel de empresa, los Admins de Equipo pueden configurar esto en el área de **Aplicaciones e Integraciones** del Equipo.

1. Desde la página de configuración de perfil, haz clic en **Equipos**.
2. Haz clic en el equipo al que te gustaría aplicar la configuración personalizada.
3. En el panel de Teams, haz clic en **Aplicaciones e integraciones**.
4. Encuentra **las Tarjetas Azure** y haz clic en ellas.
5. En el panel de configuración de la aplicación, elige **Aplicar configuración personalizada** desde el menú desplegable de la derecha y luego conecta la cuenta de Azure en la que quieres tener ajustes personalizados.
6. Autoriza a Miro en Azure DevOps con tu cuenta de Microsoft: haz clic en **Conectar** junto a "cuenta de Microsoft" e inicia sesión en tu cuenta de Microsoft, permitiéndole a Miro usarla.
7. Ingresa la **URL de tu organización Azure** (que se puede copiar de Azure DevOps) y haz clic en **Conectar.** Miro aceptará la URL personalizada de tu instancia o la dirección general `https://dev.azure.com/` que termina con el nombre de tu instancia.
   ![Animación que muestra cómo aplicar configuraciones personalizadas de Azure Cards para un equipo específico.](../../../../../../docs/integrations-apps/microsoft/images/21017013136658_azure_cards_custom_team_settings.gif)
   *Agregar configuración personalizada de tarjetas Azure a equipos específicos*

### Conecta tu cuenta personal de Azure para usar las tarjetas de Azure

Después de que un admin de Miro instale y apruebe la aplicación, cada miembro del equipo que desee usar Tarjetas Azure debe autorizar personalmente la conexión a su cuenta de Azure. Esto personaliza el selector de tarjetas y permite importar todos los elementos de trabajo de Azure a los que el usuario puede acceder.

Puedes encontrar el icono de tarjetas Azure en la barra de herramientas de creación. Si el icono no está, es posible que necesites buscarlo:

1. En la barra de creación, selecciona **Herramientas, medios e integraciones** (**+**).
   El panel de **Herramientas, medios e integraciones** se abre.
2. En la pestaña **Herramientas**, busca y selecciona Tarjetas Azure.

Para conectar tu cuenta:

1. Haz clic en el icono de Tarjetas Azure en la barra de herramientas. Una ventana emergente te pedirá que **autorices**.
2. Haz clic en el botón **Autorizar** y haz clic en **Continuar**. Irás a Team settings (Configuración del equipo) > Apps & Integrations (Aplicaciones e integraciones).
3. Usa el panel de configuración de la aplicación para conectar tu cuenta de Microsoft a Miro y especificar la instancia de Azure que te gustaría usar. Esta URL se puede copiar de Azure DevOps; Miro acepta ya sea la URL personalizada de tu instancia o la dirección general `https://dev.azure.com/` que termina con el nombre de tu instancia.
   ![Especificando la URL de la Organización de Azure en la configuración de la aplicación Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017013107730_org%20URL.jpg)

:::note
Ten presente que solo los admins de equipo pueden establecer la configuración inicial a nivel de equipo o empresa. Si no ves el botón **Conectar** para la URL de la Organización de Azure durante la configuración de administrador, asegúrate de tener [derechos de Admin de equipo para el equipo](../../administration/user-management/06-how-to-manage-admin-roles.md).
:::

## Importar elementos de trabajo de Azure a un tablero de Miro

Una vez que la aplicación de Azure Cards esté configurada y hayas conectado tu cuenta personal, puedes importar elementos de trabajo de Azure a cualquier tablero de Miro asociado con el equipo conectado. Hay dos maneras principales de hacer esto:

- Copia la URL del elemento de trabajo de Azure y pégala directamente en el tablero de Miro. El ítem se transformará automáticamente en una Tarjeta Azure.
- Usar el selector de tarjetas Azure: Haz clic en el icono de **Tarjetas Azure** en la barra de herramientas para abrir el selector.

  ![Azure Cards picker interface in Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017013109010_Azure%20cards%20picker.jpg)*Selector de Tarjetas Azure*

  El selector admite la búsqueda en todos los campos, lo que te permite encontrar una tarjeta por su título, tipo, estado, etc. También puedes usar una potente [búsqueda por palabras clave](https://docs.microsoft.com/azure/devops/project/search/get-started-search?view=azure-devops#start-your-search-with-a-keyword) con la tecnología de Microsoft.

  ![Animation showing search functionality within the Azure Cards picker.](../../../../../../docs/integrations-apps/microsoft/images/21017013114002_Azure%20Cards%20picker.gif)*Buscar Tarjetas Azure en el selector*

  Puedes filtrar tarjetas por proyecto, asignado, tipo, área y estado, lo que desbloquea el filtrado avanzado de los elementos de trabajo de Azure directamente dentro de Miro.

  ![Filtering options within the Azure Cards picker.](../../../../../../docs/integrations-apps/microsoft/images/21017013116306_filter.jpg)*Filtrar las tarjetas Azure en el selector*

  Para navegar al elemento de trabajo original de Azure, selecciona una tarjeta en el tablero y haz clic en el botón **fuente** en su menú contextual.

  ![Source button on an Azure Card linking to the item in Azure DevOps.](../../../../../../docs/integrations-apps/microsoft/images/21017042632338_card%20spurce.jpg)*El botón origen de la tarjeta*

  Las Tarjetas Azure se pueden utilizar como widgets independientes o como componentes de marcos interactivos de [Kanban](../../using-miro/advanced-tools/02-columns-formerly-kanban.md) y [Mapas de historias de usuarios](../../using-miro/advanced-tools/07-user-story-mapping.md). Puedes agregar Tarjetas Azure a estos marcos arrastrándolas.

  ![Animation showing Azure Cards being used within a Miro Kanban board.](../../../../../../docs/integrations-apps/microsoft/images/21017042632850_Azure%20cards%20and%20kanban.gif)*Trabajar con Tarjetas Azure en Kanban*

## Crear y editar Tarjetas Azure directamente en Miro

La integración bidireccional entre Miro y Azure DevOps permite a los equipos crear nuevos elementos de trabajo de Azure y editar los existentes directamente desde un tablero de Miro. También puedes convertir las tarjetas de Miro y notas adhesivas existentes en Tarjetas Azure.

### Crear una tarjeta nueva de Azure

Para crear un nuevo elemento de trabajo de Azure desde Miro:

1. Selecciona **Tarjetas Azure** desde la barra de herramientas de creación y elige **Crear elemento de trabajo** en la parte superior derecha del selector.
2. Completa los campos de la tarjeta, elige un proyecto, un tipo de artículo, un responsable y haz clic en **Crear**. El nuevo elemento se creará en tu directorio de Azure DevOps así como en tu tablero de Miro.

![Animation showing the process of creating a new Azure Card from Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017042635282_create%20an%20Azure%20Card.gif)*Crear una Tarjeta Azure en Miro*

### Convierte las tarjetas de Miro o las notas adhesivas en tarjetas de Azure

Para convertir una tarjeta de Miro o una nota adhesiva existente en una tarjeta Azure:

1. Selecciona la nota adhesiva o la tarjeta en el tablero.
2. Haz clic en la opción de convertir (generalmente un icono de Azure DevOps o "Convertir en elemento de trabajo de Azure") en el menú contextual del objeto.
3. Establece los parámetros de la tarjeta (como proyecto, tipo de elemento) en el diálogo y haz clic en **Convertir**. El texto de la nota adhesiva/tarjeta se convertirá en el título de la tarjeta.

> **💡** Ahorra tiempo convirtiendo masivamente notas adhesivas o tarjetas de Miro en tarjetas de Azure. Haz clic y arrastra para seleccionar todos los objetos que deseas convertir, y en el menú contextual, selecciona **Convertir a elementos de trabajo de Azure**.

![Converting a Miro sticky note into an Azure Card.](../../../../../../docs/integrations-apps/microsoft/images/21017013125650_convert%20a%20sticky%20into%20an%20Azure%20Card.jpg)*Convertir una nota adhesiva en una Tarjeta Azure*

### Editar una Tarjeta de Azure

La opción de editar Tarjetas Azure en Miro elimina las molestias de cambiar de una herramienta a otra. Para editar una tarjeta:

1. Haz clic en la tarjeta Azure en tu tablero de Miro.
2. Haz clic en el **ícono de bolígrafo (editar)** en el menú contextual de la tarjeta. Se abrirá una ventana emergente que te permitirá editar los campos del elemento.
3. Haz clic en **Actualizar** para guardar los cambios. Los cambios también se reflejarán en Azure DevOps.

![Editing an Azure Card's details directly within Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017042639890_edit%20an%20Azure%20card.jpg)*La opción de editar una tarjeta Azure en Miro*

### Cambiar el color de una tarjeta de Azure

Para personalizar la apariencia de tus Tarjetas Azure en el tablero:

Para cambiar el color de relleno de una tarjeta, haz clic en la tarjeta o las tarjetas y elige **color de relleno** en el menú contextual. Si duplicas la tarjeta o tarjetas, todas las copias posteriores tendrán el mismo color de relleno.

## Desinstalar la integración de Tarjetas Azure

Si ya no necesitas la integración de Azure Cards, puedes desinstalarla. Para desinstalar a nivel del equipo se requiere permisos de admin de equipo.

1. Ve a **Configuración de equipo > Aplicaciones e integraciones > Tarjetas Azure**.
2. Desplázate hacia abajo y haz clic en **Desinstalar para el equipo.**
3. Para desinstalar las tarjetas de Azure solo para tu cuenta personal, haz clic en **Desinstalar para mí.**

![Options to uninstall Azure Cards for the team or for an individual user.](../../../../../../docs/integrations-apps/microsoft/images/21017042628370_uninstall%20Azure%20cards.jpg)*Desinstalar la aplicación para todo el equipo o para ti solamente*

## Campos compatibles de la tarjeta Azure

Los siguientes campos son compatibles para Tarjetas Azure en Miro:

- Título
- Proyecto
- Tipo
- Estado
- Descripción (la edición no es compatible)
- Padre WI
- Asignado
- Prioridad
- Puntos de historia
- Área
- Iteración
- Criterios de aceptación

Los campos personalizados no son compatibles.

## Resolución de problemas de Azure Cards

Si encuentras problemas con la integración de Azure Cards, consulta los problemas comunes y sus soluciones a continuación.

La URL no es válida

La URL que usaste no es correcta. Comprueba la ortografía y el formato. Por ejemplo, la dirección de la organización de Azure debe terminar con una barra diagonal.

No se puede acceder a la URL de la organización Azure

La URL ingresada no existe. Ingresa la URL existente o verifica la ortografía. También, verifica lo siguiente:

- Asegúrate de que tu organización pueda aceptar la autorización de terceros: en **Ajustes de la Organización > Políticas (Seguridad)** **>** asegúrate de que "Acceso a aplicaciones de terceros a través de OAuth" esté habilitado.
- Tu organización de Azure está en una red privada/el firewall de tu empresa bloquea conexiones de red externas. Haz los cambios necesarios en tu firewall y la configuración de VPN, agregando nuestros dominios a tu lista de permitidos: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com, realtimeboard.com*, *.realtimeboard.com, *static.miro-apps.com. Si usas un proxy, configura uno inverso que nos permita acceder. Asegúrate de llenar el **campo de URL de Azure DevOps** en la configuración con la dirección a la que podemos acceder (la dirección puede ser diferente de la dirección real de tu Azure DevOps restringido). También podrías querer prolongar el valor de tiempo de espera en tu servidor proxy.
- Todas las solicitudes de integración pasan por un equilibrador de carga de Amazon, por lo que no es posible proporcionar información de red específica desde Miro.

No se pudo crear una suscripción al hook de servicio

El usuario de Azure que inició sesión actualmente no tiene los permisos necesarios. El usuario de Azure en cuyo nombre se conectará la instancia de Azure a Miro debe tener acceso a estos métodos de API REST:

- [*Crear suscripción al hook de servicio*](https://docs.microsoft.com/rest/api/azure/devops/hooks/subscriptions/create?view=azure-devops-rest-6.0) ("*vso.serviceendpoint_manage* [alcance](https://docs.microsoft.com/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes) requerido)
- [*Recibir metadatos sobre proyectos (esta información se utiliza para especificar correctamente los elementos de trabajo en los eventos de suscripción)*](https://docs.microsoft.com/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0)
- *También es necesario que los siguientes métodos sean accesibles para todos los usuarios que usan la integración:*
  - [*Obtener elementos*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/get%20work%20item?view=azure-devops-rest-6.0)
  - [*Lista de elementos*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/list?view=azure-devops-rest-6.0)
  - [*Obtener tipos de elementos*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/get?view=azure-devops-rest-6.0)
  - [*Listar tipos de elementos*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/list?view=azure-devops-rest-6.0)

El usuario **username@microsoft.com** no tiene acceso a ningún proyecto en la URL de la organización de Azure especificada.

No puedes acceder a ningún proyecto en la organización de Azure que se esté usando. Para importar tarjetas, deberías tener acceso a ellas del lado de Azure Boards. Comunícate con el propietario de la organización de Azure y pídele que te invite a esta organización de Azure. [Este artículo](https://docs.microsoft.com/azure/devops/organizations/security/look-up-organization-owner?view=azure-devops) puede ayudarte a averiguar el nombre del propietario de la organización.

No se pudo crear una suscripción al hook de servicio: el usuario **username@microsoft.com** no es propietario de una organización. Pide al propietario de tu organización que configure este paso.

Debes ser tanto el propietario de la organización Azure como el admin de empresa de Miro para configurar las tarjetas Azure dentro de Miro.

La autorización caducó. Vuelve a conectar la integración en la configuración de tu equipo.

La autorización de Azure caducó. Vuelve a conectar la integración a nivel personal, como se describe en la sección "Conecta tu cuenta personal de Azure para usar Tarjetas Azure" más arriba.

La tarjeta con la que estás trabajando muestra un comportamiento inesperado.

Esto puede suceder si la tarjeta no está sincronizada con la organización de Azure. Por ejemplo, si copiaste la tarjeta de otro tablero o estás trabajando en un tablero que se movió entre equipos. Para resolver la situación, vuelve a agregar el elemento de Azure al tablero.

El número de artículos de trabajo devueltos supera el límite de tamaño de 200. Cambia la consulta para que genere menos artículos.

Si recibes este mensaje de error, significa que has seleccionado demasiadas tareas para agregar al tablero como tarjetas. Limita el número de tareas usando la barra de búsqueda. En este momento, cuando abres el selector, no se aplican filtros y se muestran todas las tareas de los últimos tres meses. Cada vez que el selector intente mostrar más de 200 tareas, recibirás este mensaje de error.

No me aparece el **botón de conexión** cuando intento conectar mi organización de Azure con Miro en la configuración de Miro.

Asegúrate de tener derechos de admin de equipo. Ve a la pestaña **Usuarios activos** en la configuración de tu equipo y [asciéndete a Admin de Equipo](../../administration/user-management/06-how-to-manage-admin-roles.md) si es necesario. Esto se aplica a la configuración inicial de la conexión de la Organización Azure por un administrador.

:::note
Si tienes otros problemas, comunícate con [Soporte de Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
:::

## Preguntas frecuentes de Azure Cards

Aquí están las respuestas a algunas preguntas comunes sobre la integración de Azure Cards.

¿Qué IP deberían estar permitidas en la lista para las Tarjetas Azure?

Para que la integración de Azure Cards funcione correctamente, especialmente en entornos de red restringidos, es posible que necesites permitir las siguientes direcciones IP:

- 18.203.61.162
- 54.220.74.201
- 54.216.81.236
- 54.73.153.141
- 52.215.228.26
- 52.16.47.17
- 54.217.180.21

¿Qué sucede con las tarjetas Azure existentes cuando desconectas y desinstalas la aplicación de tarjetas Azure?

Las tarjetas se mantienen intactas en los tableros de Miro sin pérdida de datos; sin embargo, dejan de sincronizarse con Azure y el botón de origen desaparece.
