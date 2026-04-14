---
title: "Art\xEDculo de prueba de Balckbird sobre SCIM"
article_id: 25902000474898
translation_id: 25902000474898
locale: es
sidebar_position: 3
created_at: '2025-04-08T15:00:21Z'
updated_at: '2025-05-07T11:29:05Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

¡¡¡Artículo de prueba!!!

El Sistema para la Gestión de Identidad entre Dominios (SCIM) te permite automatizar la gestión y aprovisionamiento de usuarios entre Miro y tu proveedor de identidad (IdP).

> **Disponible para:**[Plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configurado por:** Admins de empresa

## Lo que debes saber

- **El SSO basado en SAML debe estar correctamente configurado y en funcionamiento en tu plan Enterprise antes de que empieces a configurar el aprovisionamiento automatizado.**
  Consulta [la guía](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) para configurar el SSO de SAML.
- **Sincronizar grupos con equipos de Miro es opcional.**
  Opcionalmente, puedes sincronizar tus grupos de IdP con equipos en Miro. Sin embargo, para evitar problemas donde un grupo de IdP se elimina de manera involuntaria o temporal, lo que resulta en la desactivación de todos los usuarios de ese grupo en Miro y desencadena la reasignación de tableros y espacios, no sincronices grupos de IdP con equipos de Miro. Los equipos se pueden crear y gestionar utilizando [Teams API](https://developers.miro.com/reference/enterprise-create-team). Para obtener más información sobre cómo la API SCIM te permite gestionar grupos, consulta [Miro Developers](https://developers.miro.com/docs/groups).
- **Los cambios de dirección de correo electrónico en SCIM incluyen las siguientes reglas de validación:**
  - **Revisión de Usuario Gestionado:** Si el dominio actual del usuario no está reclamado por la organización que inicia la solicitud SCIM, la actualización de correo electrónico se bloquea y arroja un error 400.
  - **Verificación del Dominio de Correo Electrónico de Destino:** Si el dominio de correo objetivo es reclamado por una organización distinta a la que inicia la solicitud SCIM, la actualización del correo electrónico es bloqueada y se genera un error 400. Si el dominio de correo electrónico de destino es reclamado por la organización que inicia la solicitud SCIM, la actualización del correo es permitida sin requerir confirmación por correo electrónico. Los registros de auditoría documentan la actualización en cada organización donde el usuario es miembro.
  - **Control de Dominio e Inicio de Sesión Único (SSO):** Se permiten las actualizaciones de correo electrónico basadas en la verificación del dominio a través del Control de Dominio (IDC) o Inicio de Sesión Único (SSO). Si el dominio de correo electrónico de destino es verificado a través de CD o SSO por la organización que lo inicia, la actualización puede proceder.
    ![scim-diagram-2.png](images/26547080620818_scim-diagram-2.png)
    *Un diagrama del flujo de trabajo de validación de cambios de correo electrónico SCIM*

### Reglas según las cuales opera SCIM de Miro

- Los cambios sincronizados por SCIM se aplican principalmente a los usuarios recién asignados. Se proveerá el estado de los que ya tienen suscripción, pero no se puede sobreescribir, ya que los cambios se aplican a nivel del grupo/equipo. Por ejemplo:
  a) si un usuario es miembro de Equipo1 del lado de Miro y tu IDP envía una actualización para agregarlo a Equipo2, su estado en Equipo1 no se verá afectado.
  b) si tu IdP envía una actualización que contiene cambios en Usuario1, los otros miembros del equipo no se verán afectados. Como se mencionó en **Características admitidas** > **Grupos de envío automático y sincronización** para sobreescribir el estado del equipo y resincronizar todos los usuarios a la vez, intenta iniciar un nuevo envío automático.
- A todos los usuarios aprovisionados bajo SCIM se les asigna la *licencia predeterminada* de tu suscripción:
  a) Para suscripciones Enterprise sin el Programa de licencia flexible: una licencia completa. Si tu suscripción se queda sin licencias, los usuarios empiezan a ser provisionados con una licencia [gratuita restringida](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
  b) Para suscripciones Enterprise con [>programa de licencia flexible](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) activado: Licencia gratuita o gratuita restringida, dependiendo de la [licencia de suscripción predeterminada](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).
  *- Si necesitas que algunos de los usuarios reciban una licencia diferente a la predeterminada:*
  *como se indica arriba, todos los usuarios reciben la licencia predeterminada. Sin embargo, puedes actualizarlos a todos o a algunos de ellos de inmediato utilizando el atributo **UserType** con un valor completo. Los usuarios actualizados con el atributo subirán de categoría a la licencia completa sin tiempo improductivo del lado del usuario.*
- Todos los usuarios abastecidos vía SCIM también se ven afectados por la característica [Control de dominio](../../enterprise-administration/canvas-25-admin-features/domain-control/01-domain-control.md). Esto significa que si un usuario es miembro de un solo grupo de seguridad de tu proveedor de identidad, pero tu configuración de control de dominio define tres equipos como los designados, el usuario también será agregado a esos tres equipos.
- Para proteger el servicio, Miro limita la cantidad de llamadas de API disponibles cada 30 segundos:

  | Tipo de solicitud | Nivel de límite |
  | --- | --- |
  | GET scim/users    GET scim/users/\{userId\} | Primer límite de tasa nivel 1 |
  | POST scim/users/\{userId\}    PUT scim/users/\{userId\}    PATCH scim/users/\{userId\}    DELETE scim/users/\{userId\} | Tercer límite de tasa nivel 3 |
  | GET scim/Groups    PATCH scim/Groups/\{groupId\} | Cuarto límite de tasa nivel 4 |
  | GET scim/Groups/\{groupId\} | Tercer límite de tasa nivel 4 |

  Para obtener más información sobre los niveles límite consulta [**aquí.**](https://developers.miro.com/reference#ratelimiting)Si la cantidad de solicitudes supera el límite, Miro devolverá el mensaje estándar **429 Demasiadas solicitudes**.

## Características admitidas

Encontrarás un diagrama detallado de SCIM de Miro [**aquí**](https://developers.miro.com/docs/scim).

Miro admite las siguientes características de provisión:

- **Crear usuarios nuevos**
  Los nuevos usuarios asignados a la aplicación Miro en IdP se crearán en tu suscripción Miro Enterprise como Miembros Enterprise.</span> Los usuarios que se agreguen a un grupo de usuarios y se sincronicen a un equipo de Miro con el mismo nombre se añadirán al equipo como miembros del equipo
- **Publicar actualizaciones del perfil de usuario**
  Para los atributos y cambios admitidos consulta a continuación
- **Sincronizar y enviar grupos por push**
  Sincroniza tus grupos de IdP y sus miembros con los equipos de tu suscripción a Miro Enterprise para gestionar automáticamente la membresía de los usuarios.</span> La sincronización continua enviará actualizaciones específicas sobre los usuarios de tu grupo al equipo de Miro sincronizado, mientras que un envío automático sobreescribirá el estado del equipo tratando al grupo como la fuente de verdad (si hubo cambios manuales por parte de tus admins de compañía del lado de Miro)
- **Desacoplar los nombres de grupo/equipo**
  Miro sincroniza los Grupos y Equipos por nombre, por lo que deben tener exactamente el mismo nombre. Sin embargo, después de que se cree la sincronización inicial, podrás darle a uno de ellos o a ambos los nombres que te resulten convenientes. Puedes ver el ejemplo del desacople [aquí](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)
- **Eliminar usuarios de grupo/equipo (no la suscripción Enterprise, consulta a continuación)**
  Eliminar un usuario de un grupo lo eliminará del equipo sincronizado de Miro (durante el siguiente Envío automático de grupo).
- **Desactivar usuarios**
  Desactivar/eliminar un usuario o deshabilitar el acceso de un usuario a la aplicación en el IdP *desactivará* al usuario en tu plan Enterprise de Miro.</span> Según las circunstancias, desactivar un usuario puede reasignar su contenido a los admins de equipo más antiguos:
  - si desactivas al usuario desde el extremo del IDP pero lo mantienes asignado a la aplicación de Miro, su membresía al equipo en el lado de Miro no cambia, y su contenido no se reasigna; simplemente se mueven de un estado **Activo** a uno **Desactivado** (y en la sección de usuarios, respectivamente) y dejan de consumir una licencia.
  - Si generas la desactivación eliminando al usuario en la IDP o quitando su asignación desde la aplicación de Miro, y el usuario es miembro de algunos *equipos sincronizados*, entonces el usuario será eliminado también de *esos* equipos de Miro y su contenido en dichos equipos se reasignará a los admins de equipo más antiguos.
  - Si generas la desactivación *eliminando* al usuario en la IDP o *quitando* su asignación desde la aplicación de Miro, cuando el usuario no sea miembro de equipos *sincronizados*, la membresía de equipos del usuario no cambiará y su contenido no se reasignará.
  **Eliminar un usuario** de la suscripción Enterprise no es compatible *de forma predeterminada.</span></em>* Aun así, puedes [agregar manualmente la funcionalidad mediante API](https://developers.miro.com/docs/scim#section-delete-user-by-id) para que el usuario sea completamente eliminado de la suscripción en lugar de asignarle el estado **Desactivado**. En este escenario, el contenido se reasigna a los respectivos miembros del equipo. Es imposible establecer qué admins obtendrán la propiedad del contenido que se reasigna automáticamente. Pero esto se puede configurar cuando se desactiva manualmente [un usuario en los ajustes de Miro.](../../enterprise-administration/user-management/01-deactivated-users.md)
- **Reactivar usuarios**
  Volver a asignar a un usuario a la aplicación o reactivar el perfil de usuario en el IdP lo reactivará en tu suscripción Enterprise de Miro si había sido previamente provisto y desactivado.
- **Automatizar la asignación de grupos de facturación**
  Asignar automáticamente nuevos usuarios a [billing groups](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/01-billing-groups.md) usando SCIM. Cuando esté configurado tu Proveedor de identidad (IdP), vincula tus centros de costos a tus grupos de facturación. Esto garantiza que cada usuario actual y futuro de estos centros de costos sea clasificado automáticamente en la categoría de facturación correcta.

También puedes eliminar usuarios de tu plan Enterprise enviando una llamada de **Delete** API directa, consulta la documentación [aquí](https://developers.miro.com/docs/scim#section-delete-user-by-id). Ten en cuenta que solo las llamadas *directas* eliminarán a los usuarios. **Eliminar** eventos iniciados *por tu solución de identidad* se tratarán como una solicitud de **Desactivación**.

### Atributos admitidos

:::warning
Ten en cuenta lo siguiente:
- **Correo electrónico** / El Parámetro Primario / Identificador Único / **Nombre de usuario**) es el único valor requerido por Miro y debe tener la forma de correo electrónico.
- la actualización del correo electrónico solo es posible para usuarios ya sincronizados. En otras palabras, la primera sincronización debe ocurrir cuando su correo electrónico en IdP y Miro sea el mismo, de lo contrario, Miro no reconocerá al usuario y se creará un perfil duplicado de Miro en el nuevo correo electrónico.
- la actualización de email debe ocurrir en el perfil de IdP del usuario, no en la lista de tareas.
- A diferencia de otros atributos, actualizar el **correo electrónico** del usuario enviará una notificación: tanto la dirección de correo electrónico anterior como la nueva recibirán una carta informándole al usuario que ahora debe usar su nueva dirección de correo electrónico para iniciar sesión en Miro.
:::

| Nombre de atributo | Atributo de SCIM (reclamo) |
| --- | --- |
| Correo electrónico | Nombre de usuario.  **Debe estar presente y con el formato de email** |
| *Los atributos enumerados a continuación no son obligatorios y serán aceptados por Miro si están presentes (se ignorarán otros atributos enviados a Miro).* | |
| Nombre completo | displayName      formateado;      givenName (Nombre de pila) + " " + familyName (Apellido);      nombre de usuario |
| Tipo de usuario | userType (tipo de usuario)       valor admitido: Con acceso completo |
| Activo | activo       valor admitido: "true" (verdadero) o "false" (falso) |
| Imagen de perfil | **fotos.^[type=='photo'].value** o     **fotos.^[type==photo].value** (Okta)     **photos[type eq "photo"].value** (Entra)        Debe ser una URL de texto para la imagen.        Tipos de archivo admitidos: jpg, jpeg, bmp, png, gif        Para definir el tipo de archivo, debes haber definido la extensión en la url       (por ej. `https://host.com/avatar_user1.jpg`) o la solicitud a la url             debe regresar junto con un encabezado de contenido de archivo-           Tipo (por ej. Tipo de contenido = 'image/jpeg')        Tamaño máximo de archivo a descargar es: 31457280 bytes |
| Rol del usuario | roles.^[primary==true].value (Okta)      roles[primary eq "True"].value (Entrar)      valores admitidos:  **ADMINISTRADOR_INTERNO_DE_LA_ORGANIZACIÓN** **USUARIO_INTERNO_DE_LA_ORGANIZACIÓN** |
| Número de empleado | Número de empleado |
| Centro de costos | costCenter (Centro de costes) |
| Organización | organización |
| División | división |
| Departamento | departamento |
| Nombre del manager | manager.displayName (Nombre de visualización del manager) |
| ID del administrador | manager.value  "valor" es un campo de tipo Cadena en el estándar SCIM pero managerId  El campo interno de Miro tiene el tipo Largo. Si el atributo "valor" no es  valor numérico, ignoramos este valor |

:::warning
No se admiten cambios de contraseña y no hay planes inmediatos para comenzar a admitir este cambio.
⚠️ **Nombre de usuario**, **tipo de usuario** y **roles.valor** no se pueden actualizar para [usuarios desactivados](../../enterprise-administration/user-management/01-deactivated-users.md).
:::

Todos los atributos se mostrarán en la lista de usuarios CSV exportada que se puede descargar desde la [sección de Usuarios activos](../../enterprise-administration/user-management/12-user-management-overview-on-enterprise-plan.md).

![download_as_CSV_in_company_settings.jpg](images/26547054913170_download%20as%20CSV%20in%20company%20settings.jpg)
*La opción de descargar una lista de usuarios*

![mceclip3.png](images/26547054914834_mceclip3.png)

## Configurar SCIM

### Paso 1: Habilitar la opción SCIM en Miro

Para habilitar SCIM para tu plan Enterprise de Miro, ve a **Configuración de empresa** > **Integraciones de empresa,** habilita la función de Aprovisionamiento SCIM**.</strong>** Allí puedes obtener la URL Base y el Token API para configurar tu IdP.

![scim.png](images/26547080627474_scim.png)
*SCIM en la configuración de Miro*

### Paso 2 Configura tu proveedor de identidad

La configuración dependerá del proveedor de identidad que utilices. Miro admite Okta y Entra ID preconfigurados, sin embargo, puedes usar cualquier proveedor de identidad que elijas, siempre que admita la configuración de SCIM.

OKTA: consulta las instrucciones de configuración [aquí](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md).

Entra ID: consulta las instrucciones de configuración [aquí](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

## Generar nuevo token

1. Ve a los **ajustes de Empresa** > **Integraciones de empresa.**

2. En la **sección de aprovisionamiento SCIM**, haz clic en **Generar nuevo token**.

![scim.png](images/26547080627474_scim.png)
*SCIM en configuraciones de Miro*

2. En la ventana **Generar nuevo token SCIM**, haz clic en **Generar**.

![generate_token.png](images/26547054918418_generate_token.png)

3. Después de generar un nuevo token, debes configurarlo en tu proveedor de IdP.

## Posibles dificultades y cómo resolverlas

*1. No se proveen usuarios debido a un error en la lista de permitidos.*
![mceclip0.png](images/26547054924562_mceclip0.png)
*Un ejemplo del error del proveedor de identidad Okta*

Asegúrate de que la dirección de dominio del usuario esté agregada a tu lista de permisos [en la configuración de **Seguridad**](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

*2. Si autenticas a tus usuarios finales con una solución de identidad (IDP1), pero deseas habilitar SCIM a través de un IdP diferente (IDP2), esto es posible en dos condiciones:*

1. el IdP2 puede hacer llamadas API con el token del portador.
2. ambos proveedores de identidad están sincronizados (por lo que también existen usuarios provistos por SCIM en el IdP1 y, por lo tanto, están en condiciones de autenticarse con Miro).

Para obtener más información, por favor [comunícate con nuestro Equipo de Soporte de Miro](https://help.miro.com/hc/en-us/requests/new?referer=help-center-article).
