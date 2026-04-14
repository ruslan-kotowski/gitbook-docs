---
title: Cómo eliminar tu perfil
article_id: 360017571354
translation_id: 360017571354
locale: es
sidebar_position: 7
created_at: '2019-02-11T10:08:54Z'
updated_at: '2026-01-07T13:30:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  notes: 'Configurado por: propietario del perfil'
---

Eliminar tu perfil de Miro dará lugar a que tu información sea eliminada de nuestro sistema. Ten en cuenta que un perfily un equipo son dos cosas diferentes.

- Tu perfil representa tus datos conectados a tu registro y dirección de email.
- Un equipo es un espacio del que formas parte junto con otros miembros del equipo donde los miembros pueden crear contenido y almacenar sus tableros

Cada perfil puede estar asociado con diversos equipos. Si quieres eliminar un equipo, consulta cómo hacerlo [aquí](../../administration/team-management/06-delete-and-restore-teams.md).
:::warning
La eliminación de un perfil **no se puede** deshacer.
:::

:::warning
Ten presente que la eliminación de un perfil no cancela tus suscripciones activas. Para impedir que se realicen nuevas renovaciones, [cancela tu suscripción en los ajustes](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md).
:::

### Cómo eliminar tu perfil

1. Abre la [Configuración de perfil](https://miro.com/app/settings/user-profile/).

2. 2. Ve a la parte inferior de la página y elige **Eliminar mi perfil.**

Eliminar_perfil.png
Cómo eliminar tu perfil

3. 3. En este punto, te sugerimos que guardes [copias de seguridad](../import-and-export/export/05-how-to-save-board-backup.md) o [exportes](../import-and-export/export/03-how-to-export-your-board.md) tus tableros antes de eliminarlos.

![eliminación_perfil_modal.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017429125778_profile%20removal%20modal.jpg)*Mensaje de confirmación de eliminación de perfil*

4. 5. Poco después, recibirás un mensaje de correo electrónico con un enlace de confirmación. Haz clic en el enlace para finalizar. Ten presente que es necesario que hayas iniciado sesión en tu perfil de Miro en el navegador cuando hagas clic en **Eliminar perfil** para completar satisfactoriamente la eliminación.

Email_eliminación_perfil.jpg
Correo electrónico de confirmación para eliminar el perfil

### ¿Qué le sucede a tu contenido después de que se elimina el perfil?

Tan pronto como eliminas tu perfil, tus tableros se eliminan.

Si eres el único Administrador de tu equipo, el contenido se eliminará *por completo*.  Los derechos de Administrador se le otorgarán al primer miembro invitado en orden cronológico.

Si hay otros admins en el equipo del cual eres miembro, el contenido se eliminará y se reasignará a uno de los demás admins. Esto significa que el admin podrá [restaurar los tableros en el transcurso de 90 días](../managing-boards/08-how-to-restore-a-deleted-board.md) (los usuarios de pago los encontrarán en la Papelera, los usuarios de planes gratuitos podrán restaurarlos a través de un enlace).

### Preguntas frecuentes

1. *¿Puedo eliminar mi perfil si inicio sesión en Miro con [inicio de sesión único (SSO](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md))?*
   - Sí, puedes. [Sin embargo, si tu organización usa SCIM, tu perfil se recreará inmediatamente, en tanto tu correo electrónico le sea suministrado a Miro a través de SCIM.](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)
2. *¿Cómo puedo cambiar mi dirección de correo electrónico vinculada al perfil de Miro?*
   - Utiliza esta guía: Cómo cambiar tu correo electrónico
3. *No he recibido el mensaje de correo electrónico con el enlace de confirmación.*  ¿Qué hago?
   - Intenta seguir estos pasos:

- Abre tus carpetas de **Spam, Promociones,****Correo no deseado, Redes sociales** y **Actualizaciones**, y comprueba si el correo electrónico de confirmación de Miro está ahí.
- Verifica si tu bandeja de entrada está llena para asegurarte de que no hayas llegado al límite de memoria en la bandeja de entrada de tu email.  Si está llena, posiblemente tengas que borrar algunos mensajes existentes para poder recibir nuevos. Después de eliminar mensajes, solicita nuevamente la eliminación del perfil.
- También es posible que un firewall esté impidiendo que el correo electrónico llegue a tu bandeja de entrada.  Comunícate con tu administrador de sistema y pídele que permita incluir nuestros dominios y subdominios: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com y realtimeboard.com*, *.realtimeboard.com. Aquí hay un artículo con más información sobre los remitentes de correo que debes incluir en la lista de admitidos.
- Si ninguna de estas soluciones funciona, [reporta el problema al Soporte de Miro](../tools/troubleshooting/06-contacting-miro-support.md).
