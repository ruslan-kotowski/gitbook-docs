---
title: Política sobre compartir datos en el plan Enterprise
article_id: 360017730133
translation_id: 360017730133
locale: es
sidebar_position: 7
created_at: '2019-02-11T10:09:02Z'
updated_at: '2025-11-25T16:00:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible para: plan Enterprise Rol requerido: admin de empresa'
---

La seguridad y la confidencialidad de los datos son preocupaciones importantes para la mayoría de las empresas. Por eso nuestro plan Enterprise ofrece herramientas obligatorias para controlar los riesgos de seguridad de la información. Estas incluyen una gestión de acceso más segura con la opción de inicio de sesión único basada en SAML y un mejor control de derechos y permisos de usuario con capacidades de administración mejoradas. Además, introducimos restricciones opcionales: compartir fuera de los dominios permitidos y compartir por medio de un enlace público.

:::note
La configuración de la política de uso compartido también influye en la configuración de los accesos disponibles cuando se insertan tableros dentro de una aplicación específica. Más información: [Gestionar la política de uso compartido del plan Enterprise para integraciones insertadas](../../managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

## Restringe el uso compartido fuera de los dominios permitidos

A nivel de empresa A nivel de equipo

Una vez que hayas establecido los dominios permitidos a nivel de la empresa, la opción de compartir tableros fuera de los dominios quedará restringida a todos los miembros y equipos de la empresa.

1. Ve a **Company** configuración > **Seguridad** >  **Compartir**.
2. Activa la opción **Restringir dominios permitidos**.
3. Agrega la lista de dominios de confianza utilizados dentro de tu plan Enterprise.

Para habilitar el uso compartido con [colaboradores invitados](../../../using-miro/sharing-boards/07-collaboration-with-guests.md) y evitar la lista de admitidos, marca la casilla **Permitir compartir con invitados fuera de estos dominios**.

Cuando **Permitir compartir con invitados fuera de estos dominios** está activado, los usuarios con dominios fuera de la lista de admitidos pueden recibir tableros compartidos con ellos, pero aún no podrán encontrar equipos en la [descubribilidad de equipos.](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)

![sharing-allowed-domains.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956412562_sharing-allowed-domains.png)
*La lista de dominios de confianza y la opción para compartir con invitados fuera de esos dominios*

Cualquier usuario que haya sido invitado a la suscripción antes de que se habilite la configuración permanecerá en tu plan y conservará los derechos de acceso al contenido compartido. Sin embargo, no será posible compartir ningún otro contenido con ellos.

Además, puedes **verificar todos los usuarios en función de la lista de admitidos** por si hay usuarios cuyo dominio no está permitido. Puedes eliminarlos en la siguiente ventana emergente:

![validate_against_the_allowlist.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017004911250_validate%20against%20the%20allowlist.jpg)*Usuarios cuyas direcciones de correo electrónico no coinciden con la lista de admitidos*

Al restringir el acceso a nivel de equipo, los usuarios que están fuera de los dominios permitidos no podrán acceder al equipo ni a los tableros que lo integran, ni ser invitados a ellos. La opción te permite habilitar la configuración para un equipo específico sin restringir las reglas de uso compartido de todos los usuarios de Enterprise. También te da la opción de permitir un dominio específico para un solo equipo, sin necesidad de permitirlo para toda la empresa.

:::note
Si los dominios de la lista de admitidos no están configurados a nivel de equipo, valdrá la configuración de la empresa. Si la lista de admitidos a nivel de equipo está configurada, esta anulará las restricciones a nivel de la empresa. Por ejemplo, si **Dominio 1** está en la lista de admitidos a nivel de Empresa y **Dominio 2** está en la lista de admitidos a nivel de Equipo, **Dominio 1** no estará permitido a nivel de Equipo a menos que se agregue a la lista de admitidos a nivel de Equipo.
:::

Para configurar los dominios permitidos para un equipo específico:

1. Ve a **Equipos** y selecciona el equipo que deseas configurar.
2. Ve a **Configuración** y desplázate hacia abajo hasta **Dominios permitidos para el equipo**.
3. Habilita la opción **Restringir dominios permitidos**.
4. Ingresa tus dominios permitidos y haz clic en **Añadir**.
   Para permitir compartir con invitados fuera de los dominios, marca la casilla **Habilitar el uso compartido con invitados fuera de los dominios permitidos**.

![sharing-team-allowed-domains.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921804702226_sharing-team-allowed-domains.png)
*La opción para restringir los dominios permitidos para un equipo en particular dentro de una suscripción Enterprise*

Una vez que hayas restringido el uso compartido fuera de los dominios permitidos, los usuarios de la empresa solo podrán compartir sus tableros con usuarios de los dominios especificados. Con la configuración habilitada, si un usuario de la empresa intenta compartir su tablero con un dominio no permitido, obtendrán el siguiente mensaje:

![can_t_share_outside_the_allowlist.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956416146_can%27t%20share%20outside%20the%20allowlist.jpg)*El tablero no se puede compartir con un usuario cuyo dominio no está en la lista de admitidos*

:::note
Si en tu empresa está permitido compartir por medio de un enlace público, los [tableros públicos](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartir-tableros-a-traves-de-un-enlace-publico) seguirán estando accesibles para *cualquiera que tenga el enlace del tablero* (y la contraseña, si está configurada).
:::

## Restringe el uso compartido a través de un enlace público

Los admins de empresa pueden restringir a todos los usuarios de la empresa o a los miembros de un equipo en particular de [compartir públicamente los tableros de la empresa](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartir-tableros-a-traves-de-un-enlace-publico). Una vez que la configuración se desactiva, la opción **Cualquier persona que tenga el enlace** desaparece del menú Compartir de los tableros de la empresa o equipo.

A nivel de empresa A nivel de equipo

Realiza lo siguiente para restringir el uso compartido público de todos los usuarios de la empresa:

1. Ve a **Company** **Configuración >** **Seguridad > Compartir**.
2. Desactiva la opción **Los tableros pueden compartirse de manera pública**.

Al hacerlo, se eliminará la opción "Cualquier persona con el enlace" del menú Compartir del tablero. Esto también significa que todos los tableros que se hayan compartido previamente con un enlace público o que se hayan insertado en sitios dejarán de estar disponibles para los usuarios públicos y sus sesiones activas en los tableros se cerrarán.

Si los admins vuelven a habilitar la capacidad de compartir tableros públicamente, los usuarios deberán reactivar el uso compartido público manualmente para cada tablero.

Si quieres permitir la edición en tableros compartidos públicamente, marca la opción **Permitir editar en tableros compartidos públicamente***.* Si *desmarcas la casilla,* se restringirá el acceso público a todos los tableros previamente compartidos para la edición pública.

:::note
El uso compartido a través de un enlace público se activa por defecto a nivel de equipo y para los equipos recién creados está establecido que "Cualquier persona puede ver y comentar". Sin embargo, si esta característica está **apagada** a nivel de empresa, los equipos no podrán compartir tableros públicamente aunque esto sí esté permitido a nivel de equipo.
:::

Cómo restringir el uso compartido de tableros de forma pública para un equipo determinado:

1. Ve a **Equipos** y selecciona el equipo que deseas configurar.
2. Ve a **Configuración** y desplázate hacia abajo hasta **Configuración para compartir**.
3. Bajo **Uso compartido del tablero** > **Por enlace público**, verás tres opciones: puedes elegir si permitir el uso compartido público solo para ver y comentar, para ver, comentar y editar, o restringir el uso compartido público para el equipo.

![sharing-public-link.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978809746_sharing-public-link.png)
*La opción para configurar el uso compartido a través de un enlace público para un equipo dentro de una suscripción Enterprise*

**Vencimiento del enlace público (a nivel de empresa)**

Para que los tableros compartidos públicamente sean más seguros, habilita el vencimiento de enlaces públicos. Esto significa que, si el tablero no se ha abierto después de un plazo determinado, cualquier enlace al tablero compartido con visitantes dejará de funcionar. Esto se aplica a todos los tableros una vez que se active el vencimiento de enlaces públicos en la configuración de la empresa.

Para habilitar el vencimiento de enlaces públicos:

1. Ve a **Configuración de la empresa > Seguridad > Compartir**.
2. Desplázate hacia abajo hasta la sección **Contenido**.
3. Selecciona la casilla de verificación para **Vencer enlace de uso compartido público**.
4. Establece la cantidad de días antes de que caduquen los enlaces inactivos. Puedes elegir entre 30 y 999 días.

:::warning
Si se restablece la contraseña de un tablero, también se restablecerá la fecha de vencimiento de ese tablero.
:::

## Exigir contraseñas para los tableros públicos (a nivel de empresa).

También puedes aplicar contraseñas obligatorias para todos los tableros compartidos públicamente a través de enlaces.

1. Ve a **Configuración de la empresa > Seguridad > Compartir**.
2. Desplázate hasta la sección **Contenido**.
3. Marca la casilla de verificación **Solicitar contraseñas para tableros compartidos públicamente**.

Una vez que esta función esté marcada, se aplicará inmediatamente a los tableros previamente accesibles mediante enlace público y a partir de ese momento no se podrá acceder públicamente a ningún tablero sin una contraseña.

- *Para tableros previamente accesibles por* [*enlace público*](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartir-tableros-a-traves-de-un-enlace-publico) *sin contraseñas:*
  Si se podía acceder previamente a los tableros mediante enlaces públicos sin contraseñas, se revocarán las sesiones abiertas y se pedirá a los visitantes que ingresen una contraseña cuando intenten acceder a un enlace previamente accesible.
- *Para todos los tableros:*
  Para que un tablero sea accesible públicamente mediante un enlace, el propietario del tablero o el [admin de contenido](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) debe establecer una contraseña. Si se elimina una contraseña, la opción **Cualquier persona con el enlace** en el menú Compartir del tablero se convertirá a **Sin acceso**. Los miembros del equipo con derechos de edición pueden compartir un tablero a través de un enlace público si la contraseña ya se ha establecido; de lo contrario, deben comunicarse con el propietario del tablero para establecer una contraseña.
- Cuando se establezca la opción "*El enlace vence cuando el tablero ha estado inactivo durante 'x' días*", aparecerá un icono de reloj en el cuadro de diálogo Share, con un mensaje que indica que el acceso público desaparecerá después de la cantidad de días especificada.
  ![1-2.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978811282_1-2.png)
*Opción de uso compartido público en el plan Enterprise con contraseñas obligatorias*

También puedes exigir que las contraseñas sean complejas y especificar qué requisitos deben cumplir. Estos pueden incluir:

- Longitud mínima de la contraseña (de 6 a 14 caracteres; el valor predeterminado es 8).
- Letras mayúsculas y minúsculas.
- Números.
- Caracteres especiales.

![complex-board-password.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956422418_complex-board-password.png)
*Configuración para contraseñas complejas de tableros*

## Restringir el uso compartido con todos los equipos y con toda la empresa (a nivel de equipo).

:::note
El uso compartido que abarca el equipo y toda la empresa se activa por defecto si el admin de empresa no ha personalizado la configuración.
:::

Los admins de empresa del plan Enterprise también pueden habilitar o deshabilitar el uso compartido en toda la empresa o en todo el equipo.

1. Ve a **Teams** y selecciona el equipo que deseas configurar.
2. Ve a **Configuración** y desplázate hasta **Configuración para compartir**.
3. En **Uso compartido del tablero,** elige si se permite o no compartir con un equipo. Para la configuración a nivel de empresa, elige si la empresa puede ver y comentar tableros compartidos, ver/comentar/editar, o si no se permite compartir.![sharing-board-sharing.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921804722706_sharing-board-sharing.png)*Configuración de uso compartido de tableros en el plan Enterprise*

Habilitar el uso compartido de tableros con un equipo permite a sus miembros compartir fácilmente los tableros y los proyectos con todo el equipo.

Deshabilitar esta opción lo eliminará del menú Compartir de los tableros y los proyectos del equipo. Los tableros y los proyectos que se hayan compartido anteriormente ya no estarán disponibles para los usuarios del equipo, a menos que se compartan por otro medio.

Si el admin vuelve a habilitar la capacidad de compartir con el equipo, los tableros y los proyectos ya compartidos no se compartirán de forma automática con el equipo y los usuarios deberán volver a compartirlos manualmente.

![1-3.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978812178_1-3.png)
*La opción de compartir un tablero con el equipo puede ocultarse en el menú Compartir*

Los usuarios de los planes Enterprise con [Privacidad de equipo](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) deshabilitada también pueden [compartir sus tableros con toda la empresa para ver, comentar o editar con un solo clic](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md). Puedes bloquear esta opción para un equipo en particular seleccionando **No permitida** en el parámetro **Con toda la empresa**. O puedes permitir el uso compartido solo para ver y comentar; o bien para ver, comentar y editar.

Ten en cuenta que, si la [Privacidad de equipo](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) está habilitada en tu empresa, la opción de compartir tableros con toda la empresa no estará disponible incluso si lo está a nivel de equipo.

![1-4.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956423442_1-4.png)
*La opción de compartir un tablero con toda la empresa puede estar oculta en el menú Compartir*

## Restringir la capacidad de mover tableros a otros equipos (a nivel de equipo).

:::note
La posibilidad de mover tableros a otros equipos estará activada por defecto si el admin de empresa no ha personalizado la configuración.
:::

Cuando un admin de empresa no le permite a un equipo mover los tableros, sus miembros no podrán mover los tableros a otros equipos ni fuera del mismo equipo. La configuración se realiza para cada equipo en **Configuración de equipo > Permisos**.

:::note
Los usuarios que no son admins no pueden mover tableros a un equipo si tienen la [opción de crear tableros restringida](../../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md) en el equipo de destino.
:::

![sharing-moving-boards.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956424082_sharing-moving-boards.png)
*Opción de restringir la inclusión y el retiro de tableros del equipo*

## Restricción del uso compartido de plantillas personalizadas en toda la empresa

> **Disponible para:** plan Enterprise
> **Quién puede hacerlo:** admins de empresa

Los admins de empresa pueden permitir o restringir el uso compartido de plantillas personalizadas a nivel de empresa. Cuando se restringe el uso compartido, los miembros del equipo no podrán compartir una plantilla personalizada con la empresa sin la aprobación del admin.

1. Ve a **Configuración de la empresa** > **Seguridad** > **Configuración**.
2. Desplázate hasta **Roles y permisos**.
3. Activa la opción **Restringir el uso compartido de plantillas de la empresa**.

![sharing-restrict-templates.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978813202_sharing-restrict-templates.png)
*La opción de restringir el uso compartido de plantillas de la empresa*

## Preguntas frecuentes

¿Los miembros reciben notificaciones cuando los admins de empresa cambian la configuración de uso compartido mencionada anteriormente a nivel de equipo o de empresa?

No. En esos casos no se envían notificaciones. Las reglas se aplican inmediatamente.

¿Tenemos un panel donde podamos rastrear todos los tableros que se comparten con un enlace público?

Actualmente, no hay un panel para eso.

Desactivé la opción de restringir los dominios permitidos, pero todavía no podemos compartir tableros con usuarios fuera de los dominios permitidos. ¿Cómo puedo arreglar esto?

Es posible que la configuración aún esté activada a nivel de empresa o equipo. Por favor, comprueba si la restricción está desactivada en la Configuración de la empresa o en la Configuración de equipo.
