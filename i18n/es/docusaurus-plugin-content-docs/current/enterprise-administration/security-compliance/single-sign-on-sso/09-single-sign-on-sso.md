---
title: "Inicio de sesi\xF3n \xFAnico (SSO)"
article_id: 360017571414
translation_id: 360017571414
locale: es
sidebar_position: 9
created_at: '2019-02-11T10:08:59Z'
updated_at: '2026-01-07T13:25:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Con el inicio de sesión único (SSO) basado en SAML, los usuarios pueden acceder a Miro a través de un proveedor de identidad (IdP) de su elección.

> **Disponible para:** planes Business y Enterprise
> **Rol requerido:** admin de empresa

## Cómo funciona el SSO basado en SAML

1. Cuando un usuario de Miro intenta iniciar sesión en Miro utilizando SSO, Miro envía una solicitud SAML (Lenguaje Marcado para Confirmaciones de Seguridad) al proveedor de identificación (IdP)
2. El proveedor de identificación valida las credenciales del usuario y envía una respuesta a Miro para confirmar la identificación del miembro
3. Miro reconoce la respuesta y otorga acceso, lo que permite al miembro iniciar sesión en su cuenta de Miro

## ¿Qué sucede cuando se habilita el SSO?

**Habilitar el SSO por primera vez**

La primera vez que configures el SSO, los usuarios existentes podrán seguir trabajando en Miro sin interrupción. Sin embargo, la próxima vez que se desconecten, caduque su sesión o intenten conectarse desde un nuevo dispositivo, tendrán que iniciar sesión mediante SSO.

Las otras opciones de inicio de sesión quedarán deshabilitadas para los usuarios, incluyendo la opción estándar de nombre de usuario y contraseña y otras como Google, Facebook, Slack, AppleID y O365.

**Tiempo de espera de sesión inactiva**

Si habilitaste [el tiempo de espera de sesión inactiva](../../security-integrations/security-management/02-idle-session-timeout.md), la sesión de los usuarios en su perfil de Miro se cerrará automáticamente y se requerirá una nueva autorización vía SSO.

**Múltiples equipos y organizaciones**

Si los usuarios tienen varios equipos u organizaciones de Miro, puedes configurarlos para que usen el mismo proveedor de identificación (IdP) para la autenticación.

**Quién debe iniciar sesión con SSO**

El inicio de sesión con SSO será obligatorio los para usuarios activos que sean parte de tu suscripción Enterprise *y* tengan un dominio que figure en tu configuración de SSO.

- Los usuarios que accedan a Miro desde dominios no añadidos en tu configuración de SSO no están obligados a iniciar sesión con SSO, y en su lugar deben hacerlo utilizando los métodos de inicio de sesión estándar.
- Los usuarios de un dominio verificado que no formen parte de tu suscripción a Miro Enterprise solo deben iniciar sesión a través del inicio de sesión único (SSO) si está habilitado [el aprovisionamiento justo a tiempo (JIT)](../../user-management/13-user-provisioning-on-enterprise-plan.md). Estos usuarios se añadirán automáticamente a un equipo preconfigurado y deberán utilizar SSO para iniciar sesión.
- [Usuarios gestionados](../../user-management/06-managed-users-on-enterprise-plan.md)que es cualquier usuario dentro de tu(s) dominio(s) verificado(s), incluido cualquier usuario gestionado que también sea miembro de un equipo fuera de tu suscripción de Empresa. Para restringir el acceso a equipos concretos, actualiza la configuración de [control de dominios](../../canvas-25-admin-features/domain-control/01-domain-control.md).
  > ✏️ Para una suscripción de empresa, una organización puede tener dominios verificados y no verificados. En los dominios verificados, los usuarios se convierten en usuarios gestionados que deben autenticarse con SSO. Para los usuarios de dominios no verificados de la misma organización, el correo electrónico y la contraseña son necesarios para la autenticación.

**Cómo gestionar los datos del usuario**

Los datos del usuario son atribuidos automáticamente en Miro por tu proveedor de identidad al iniciar sesión con éxito. Algunos parámetros como el nombre y la contraseña no se pueden cambiar. Otros parámetros como el departamento y las fotos de perfil son opcionales.  /span>

- Los nombres de usuario en Miro se actualizan después de cada autenticación de usuario exitosa. Para obtener más información sobre cómo configurar los nombres de usuario de Miro, consulta la configuración avanzada de SSO. Si necesitas cambiar la dirección de correo electrónico de un usuario, puedes hacerlo solo a través de [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md). Si no utilizas SCIM, [ponte en contacto con el equipo de Soporte](https://help.miro.com/hc/requests/new?referer=help-center-article).

![sso-settings-2.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21027132582290_sso-settings-2.png)
*Selección de dominio en la configuración de SSO*

> **💡** Para evitar un bloqueo, crea un usuario de emergencia con un correo electrónico que tenga un dominio fuera del dominio que aparece en la configuración de SSO, como acmebreaktheglass@gmail.com. De lo contrario, puedes comunicarte con el servicio de Soporte y este puede deshabilitar el SSO para toda la organización.

## Configurar SSO

### Proveedores de identificación (IdP)

Usa cualquier proveedor de identificación de tu elección. A continuación, se muestran las plataformas de proveedores de identificación más populares:

- [OKTA](../../security-integrations/single-sign-on-sso/07-how-to-configure-okta-sso.md)
- [Entra ID](../../security-integrations/single-sign-on-sso/05-how-to-configure-entra-id-sso.md) de Microsoft
- [OneLogin](../../security-integrations/single-sign-on-sso/08-how-to-configure-onelogin-sso.md)
- [ADFS](../../security-integrations/single-sign-on-sso/02-how-to-configure-adfs-sso.md) de Microsoft
- [Auth0](../../security-integrations/single-sign-on-sso/03-how-to-сonfigure-auth0-sso.md)
- [Google SSO](../../security-integrations/single-sign-on-sso/06-how-to-configure-google-sso.md)
- [Jumpcloud SSO](https://support.jumpcloud.com/support/s/article/single-sign-on-sso-with-miro)

### Cómo configurar tu IdP

> **💡** [Si tu organización empresarial desea añadir varios proveedores de identidades](../../security-integrations/single-sign-on-sso/01-adding-multiple-identity-providers.md) (IdPs), inscríbete en nuestra [beta privada](https://coda.io/form/Miro-Multi-IdP-Private-Beta-Sign-Up_dkoTJMza_jV).

1. Ve a la sección de configuración de tu proveedor de identidad y sigue las instrucciones del proveedor para configurar el inicio de sesión único.

2. Añade los siguientes metadatos. Te recomendamos que omitas los campos opcionales y dejes los valores por defecto como están.

#### Especificaciones (metadatos)

|  |  |
| --- | --- |
| **Protocolo** | SAML 2.0 |
| **Vinculación** | Redirección HTTP del SP al IdP HTTP Post para IdP a SP |
| **La URL del servicio** (URL iniciada por SP)  También se conoce como URL de lanzamiento, URL de respuesta, URL de servicio de SSO de usuario de confianza, URL de destino, URL de inicio de sesión de SSO, punto final del proveedor de identificación, etc. | https://miro.com/sso/saml |
| **URL del servicio de consumidor de aserciones**    También se conoce como URL de devolución de llamada permitida, URL de ACS personalizada, URL de respuesta | https://miro.com/sso/saml |
| **ID de entidad**    También se conoce como identificador, identificador de usuario de confianza | https://miro.com/ |
| **Estado de retransmisión predeterminado** | Debe dejarse vacío en la configuración |
| [**Requisito de firma**](https://developers.onelogin.com/saml/examples/response) | Una respuesta SAML sin firmar con una aserción firmada  Una respuesta SAML firmada con una afirmación firmada |
| **Método de SubejctConfirmation** | "urn:oasis:names:tc:SAML:2.0:cm:bearer" |
| La respuesta SAML del proveedor de identidad debe contenerun Certificado x509 de clave pública emitido por el proveedor de identidad.  Ver ejemplos detallados de SAML. Descarga el [archivo de metadatos](https://drive.google.com/file/d/1BN58fiwC062F5MC-PsO3QN7JlCbKNCSJ/view) Miro SP(XML). | |

:::warning
No se admite el cifrado ni el cierre de sesión único.
:::

#### Credenciales de usuario

No se requieren campos adicionales que no estén incluidos a continuación. Te recomendamos que omitas los campos opcionales y dejes los valores por defecto como están.

|  |  |
| --- | --- |
| Atributos de credenciales de usuario requeridos | |
| **NameID**(es igual a la dirección de correo electrónico de un usuario)  También se conoce como SAML_Subject, clave primaria, nombre de inicio de sesión, formato de nombre de usuario de la aplicación, etc. | &lt;NameID Format="urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress"&gt; |
| **Atributos opcionales que se enviarán con la aserción**  (se actualiza con cada nueva autenticación mediante SSO, se utiliza cuando está presente/disponible) | - "DisplayName" o"http://schemas.microsoft.com/identity/claims/displayname"(utilizado como nombre preferido)  [mceclip0.png](http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname)  - "Nombre", "Apellido" o"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname"; - "Apellido", "Apellidos" o"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname"; - “ProfilePicture”: la URL codificada de la imagen. |

### Cómo habilitar el SSO en tu configuración de Miro

Plan Business y plan Enterprise

1. Ve a la configuración de tu **empresa** > **Seguridad** > **Inicio de sesión único**
2. Activa **SSO/SAML

*![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20889990489874_security-sso.png)
*security-sso.png****

1. Ve a la configuración de tu **empresa** > **Seguridad y cumplimiento** > **Autenticación** > **Inicio de sesión único**
2. Activa **SSO/SAML

*![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366644626_sso-enterprise.png)
*sso-enterprise.png****

:::note
Habilitar el SSO en tu configuración no habilita inmediatamente el SSO para los usuarios. El inicio de sesión SSO está disponible una vez [verificados](../../canvas-25-admin-features/domain-control/01-domain-control.md) tus [dominios](../../canvas-25-admin-features/domain-control/01-domain-control.md). Después, cuando configures el SSO en la siguiente sección, asegúrate de añadir tus dominios verificados.
:::

### Cómo activar el SSO en tu configuración de Miro

Tras activar la función SSO/SAML en la configuración del inicio de sesión único, rellena los siguientes campos:

1. URL de **inicio de sesión de SAML** (en la mayoría de los casos abre la página de tu proveedor de identidad donde tus usuarios finales deben ingresar sus credenciales)
2. **Certificado x.509 de clave pública** (emitido por tu proveedor de identidad)
3. Todos los dominios y subdominios permitidos o requeridos (ACME.com o ACME.dev.com) para autenticarte a través de tu servidor SAML
4. Añade tu(s) dominio(s) verificado(s). Para **Los usuarios de estos dominios iniciarán sesión mediante SSO**, haz clic en ***Selecciona un dominio***y selecciona cualquiera de tus dominios para añadirlo a la lista.

![sso-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366648082_sso-settings.png)
*Configuración de SSO de Miro*

### Cómo renovar tu certificado de SSO/SAML

Si tu certificado de clave pública x.509 caducó, el SSO seguirá funcionando, pero recomendamos enfáticamente renovarlo para seguir usando Miro de forma segura. Los certificados de clave pública x.509 garantizan la seguridad, la privacidad, la autenticidad y la integridad de la información compartida entre tu proveedor de identificación y Miro.

Estos certificados solo son válidos por un período de tiempo que se puede especificar (y verificar) con tu proveedor de identificación. Consulta con tu proveedor de identidad para verificar la fecha de caducidad.

Este proceso consta de dos pasos:

1. Renovar el certificado con tu proveedor de identificación. Consulta sus instrucciones sobre cómo hacer lo anterior.
2. Añadir el certificado renovado a tu configuración de SSO de Miro.

#### Cómo añadir certificados renovados a Miro

:::warning
Recomendamos reemplazar tu certificado x.509 durante los períodos de menos actividad en tu organización (por ejemplo, el fin de semana o después del horario comercial) para evitar interrupciones durante el inicio de sesión.
:::

1. Ve a **Configuración de** empresa > **Autenticación** > **Inicio de sesión único.**
2. Elimina el contenido dentro del campo **Certificado de clave x.509**.
3. Pega la nueva clave dentro de este campo.
4. Desplázate hacia abajo y haz clic en **Guardar**
   ![sso-gif-2.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21027132584850_sso-gif-2.gif)
*Renovación de un certificado x.509 en Miro*

## Cómo probar tu configuración SSO

Prueba tu configuración de SSO antes de habilitarla para reducir las posibilidades de que tus usuarios tengan problemas de inicio de sesión.

1. Completa los pasos anteriores para configurar tus ajustes SSO.
2. Haz clic en el botón **Probar configuración SSO**.
3. Revisa los resultados:

- Si no se encuentra ningún problema, se mostrará un mensaje de confirmación de que **la prueba de configuración SSO se ha realizado correctamente**.
- Si se encuentran problemas, se mostrará un mensaje de confirmación **Prueba de configuración SSO fallida**, seguido de mensajes de error detallados para orientarte sobre lo que hay que arreglar.

![sso-test.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366649618_sso-test.png)
*Prueba la configuración de SSO*

## Configuración de SSO avanzada opcional

La sección de configuración opcional la utilizan los usuarios avanzados que están familiarizados con la configuración de SSO.

### Aprovisionamiento justo a tiempo para usuarios nuevos

Haz que sea más fácil para los usuarios comenzar a usar Miro de inmediato, sin tener que esperar una invitación o pasar por un proceso de incorporación demasiado extenso. Y asegúrate de que los equipos gratuitos no se creen fuera de tu suscripción gestionada (requiere control de dominio). Se requiere SSO para habilitar el aprovisionamiento justo a tiempo (JIT) de usuarios nuevos. A todos los usuarios con aprovisionamiento JIT se les asigna la licencia predeterminada de tu suscripción:

|  |  |  |
| --- | --- | --- |
| **Tipo de suscripción** | **Tipo de licencia** | **Comportamiento cuando se agotan las licencias** |
| Plan Business | Licencia con acceso completo | Los usuarios no se agregan automáticamente; la función JIT deja de funcionar. |
| Plan Enterprise (sin [el programa de licencias flexibles](../../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)) | Licencia con acceso completo | Usuarios aprovisionados bajo licencia [gratuita limitada](../../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) |
| Plan Enterprise (con el programa de licenciaa flexibles activado) | Licencia gratuita o gratuita limitada | Depende de la configuración [de licencias predeterminada](../../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md) |

### Cómo habilitar el aprovisionamiento justo a tiempo

Cuando actives el aprovisionamiento justo a tiempo, se aplicará automáticamente a todos los usuarios nuevos que se registren en Miro. Sin embargo, los usuarios existentes de Miro seguirán necesitando una invitación para unirse a tu plan.

1. Ve a tu configuración SSO
2. Marca la casilla **Agregar de forma automática a todos los usuarios recién registrados de la lista de dominios en tu cuenta Enterprise**
3. **Elige un equipo predeterminado para los usuarios recién registrados** en el menú desplegable
4. Haz clic en **Guardar**

Cuando incluyas dominios específicos en tu configuración de inicio de sesión único (SSO), los usuarios que se registren con esos dominios se añadirán automáticamente a tu suscripción de Empresa. Se asignarán al equipo que hayas seleccionado en tu configuración justo a tiempo (JIT).

![Copy of user_provisioning_jit_provisioning.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528391698_Copy%20of%20user_provisioning_jit_provisioning.png)*Habilita la función de aprovisionamiento justo a tiempo en la página de integraciones de empresas*

Todos los **usuarios recientemente registrados** de los dominios que enumeres en la configuración se agregarán de forma automática en tu cobertura Enterprise a este equipo en particular cuando se registren en Miro.

:::warning
En el plan Enterprise este equipo también aparecerá en la lista de equipos que se pueden descubrir si habilitas elDescubrimiento de equipos.
:::

### Configurar el nombre de visualización como el nombre de usuario predeterminado

De forma predeterminada, Miro usará los atributos **FirstName** y **LastName** . Alternativamente, puedes solicitar el uso de **DisplayName** En este caso, Miro utilizará **DisplayName** *cuando esté presente* en la respuesta SAML del usuario.

Si **DisplayName** no está presente, pero sí **FirstName** + **LastName** , Miro utilizará **FirstName** + **LastName.** Ponte en contacto con el equipo de Soporte de Miro para que **DisplayName** sea tu nombre de usuario SSO preferido.

Si ninguno de los tres atributos está presente en tu comunicación SAML, Miro mostrará la dirección de correo electrónico del usuario como nombre de usuario.

|  |  |
| --- | --- |
| **Configuración** | **Nombre de usuario predeterminado** |
| Nombre de usuario de Miro | FirstName + LastName |
| Configuración alternativa | DisplayName (si está presente en la solicitud SAML del usuario) |
| Respaldo | FirstName + LastName (si DisplayName no está presente) |
| Nombre de usuario SSO preferido | DisplayName ([comunícate con el servicio de Soporte de Miro](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)) |
| No hay atributos presentes | La dirección de correo electrónico se muestra como Nombre de usuario |

Si ves algo diferente de lo esperado, es posible que debas autenticarte mediante SSO o que la respuesta SAML no contenga los valores necesarios para actualizar.

### Sincronizar imágenes del perfil de usuario desde el IdP

:::warning
Por lo general, se recomienda habilitar esta opción si no habilitas SCIM o si tu IdP no es compatible **con el** atributo **ProfilePicture** (por ejemplo, ProfilePicture no es compatible con Azure). En otros casos, se recomienda pasar ProfilePicture a través de SCIM con actualizaciones inmediatas.
:::

Cuando esta configuración está activada:

- La imagen de perfil establecida del lado del IdP será la imagen del perfil de Miro del usuario.
- Los usuarios no podrán actualizar ni eliminar su imagen de perfil por sí mismos.

:::warning
Al igual que con el atributo de nombre de usuario, los usuarios no podrán cambiar sus datos en Miro de inmediato, pero la *sincronización* de datos no es inmediata. Desde IdP se envía la actualización a Miro solo con la *siguiente* autenticación SSO del usuario, siempre que la configuración “Sincronizar las fotografías de perfil del usuario desde el IdP” todavía esté activa en ese momento.
:::

Si la imagen del perfil está configurada en el IDP y deseas que el atributo se pase en la comunicación SAML, Miro esperará el siguiente esquema:

```
<saml2:Attribute Name="ProfilePicture" NameFormat="urn:oasis:names:tc:SAML:2.0:attrname-format:uri">
<saml2:AttributeValue
xmlns:xs="http://www.w3.org/2001/XMLSchema"
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">https://images.app.goo.gl/cfdeBqKfDKsap1icxecsaHF
</saml2:AttributeValue>
</saml2:Attribute>
```

## SSO y residencia de datos

Si utilizas el Soporte de [Residencia de Datos](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md) de Miro y tienes una URL dedicada (workspacedomain.miro.com), debes ajustar la configuración de tu proveedor de identidad.

:::note
Para las organizaciones con residencia de datos en Australia y Estados Unidos, el inicio de sesión social no está disponible. Para más información sobre la residencia de datos, consulta [Residencia de datos en Miro](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md).
:::

Para hacerlo, deberás agregar tu [ORGANIZATION_ID] a la URL.

Puedes encontrar tu ORGANIZATION_ID del panel de Miro si haces clic en tu **Perfil** en la esquina superior derecha > **Configuración** > que se muestra en la URL de la barra de direcciones.

|  | Valor estándar | Valor bajo residencia de datos |
| --- | --- | --- |
| **URL del servicio de consumidor de aserciones**(también conocida como URL de devolución de llamada permitida, URL ACS personalizada, URL de respuesta): | https://miro.com/sso/saml | https://workspace-domain.miro.com/ sso/saml/ID_ORGANIZACIÓN |
| **Identificador de entidad** (Identificador, Identificador de confianza de la parte que confía): https://miro.com/ | https://miro.com/ | https://workspace-domain.miro.com/ ORGANIZACIÓN_ID |

## Cómo configurar la autenticación multifactor (2FA) para usuarios que no utilicen SSO

La autenticación de dos factores (2FA) proporciona una capa de seguridad adicional. Con 2FA, los usuarios deben completar un paso adicional durante el inicio de sesión para verificar su identificación. Esta medida adicional garantiza que solo las personas autorizadas puedan acceder a tu suscripción.
Obtén más información en nuestra [Guía de admins de autenticación de dos factores](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).

## Preguntas frecuentes y resolución de posibles problemas

Mis direcciones de dominio no se aceptan en la configuración SSO - Mensaje “DomainName is busy” (DomainName está ocupado).

Por razones de seguridad, respaldamos los dominios de una organización en *un grupo de la empresa (suscripción Enterprise) solamente*. Es posible que tus dominios ya estén siendo utilizados para otro plan Business o [en un plan Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md), lo que te impide habilitar SSO con los dominios deseados. Tal vez quieras comprobarlo con tus colegas de antemano.

Mi dominio no aparece en el desplegable de dominios disponibles.

Primero tienes que reclamar y verificar tus dominios en la [configuración de dominios gestionados](../../canvas-25-admin-features/domain-control/01-domain-control.md).

Necesitamos cambiar las direcciones de correo electrónico de nuestros usuarios finales/Hemos cambiado los emails de nuestros usuarios y ahora no pueden acceder a sus tableros.

Si tu empresa cambia su nombre de dominio y, por lo tanto, las direcciones de correo electrónico de los usuarios finales necesitan un cambio de las credenciales de SSO, comunícate con el equipo de Soporte [para obtener asistencia.](https://help.miro.com/hc/requests/new?referer=help-center-article)

Nos gustaría usar una puerta de enlace separada (por ejemplo, MFA, como Dag Duo) para el procedimiento SSO.

Ciertamente puedes hacerlo. Miro admitirá tu solución preferida siempre que funcione con SAML 2.0.

Habilitamos SSO, pero los datos de los perfiles de usuario (nombre e imágenes de usuario si los admite tu IdP) en Miro no se sincronizan con los que están en IdP.

El nombre de usuario y la imagen de perfil de Miro se actualizan después de cada autenticación de usuario correcta  *si* SAMLResponse contiene nuevos valores no vacíos. Para obtener más información sobre cómo configurar el nombre de usuario de Miro, consulta la configuración avanzada de SSO.

¿Cuál es el proceso para cambiar de proveedor de SSO?

Cuando cambies de proveedor de SSO, tendrás que configurar el nuevo IDP desde cero, como harías en una primera configuración.

Si uno de tus usuarios o todos ellos experimentan un error al intentar iniciar sesión en Miro, consulta esta lista de errores comunes y cómo resolverlos.
