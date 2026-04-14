---
title: Configurar la gestión de movilidad empresarial (EMM) en Android
article_id: 13888848676498
translation_id: 13888848676498
locale: es
sidebar_position: 3
created_at: '2023-09-21T14:45:02Z'
updated_at: '2025-11-25T15:38:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
availability:
  notes: 'generales: sobre cómo configurar la solución EMM/MDM de tu empresa utilizando
    tres ejemplos de software específico: VMWare (Workspace ONE), Ivanti Neurons (antes
    MobileIron Cloud) e Intune (Microsoft Endpoint Manager). Si usas una solución
    diferente, te recomendamos consultar los pasos exactos en la documentación de
    tu proveedor de EMM.'
---

La EMM permite a los admins de empresa configurar y distribuir Miro a los usuarios de sus organizaciones de forma centralizada y unificada. Miro admite el aprovisionamiento de la siguiente configuración en los dispositivos de usuarios finales:

- Deshabilitar el flujo de registro.
- Limitar los proveedores de autenticación compatibles (por ejemplo, redes sociales, proveedores de correo electrónico, etc.).
- Restringir el nombre de usuario a un valor específico o a una lista de dominios de correo electrónico permitidos.
- Configuración de SSO avanzada.

## Cómo configurar

### Añade Miro al directorio de aplicaciones de tu organización

Para la mayoría, habilitar la configuración de EMM requerirá agregar Miro al catálogo de aplicaciones de tu organización. Este proceso puede diferir de un proveedor de EMM a otro. Aun así, por lo general, agregarás Miro al catálogo de aplicaciones directamente desde Google Play Store y establecerás una política de distribución basada en los grupos de dispositivos, grupos de usuarios, etc.

#### Ejemplos

**VMware Workspace ONE**

La guía de implementación general de VMware Workspace ONE se puede encontrar [aquí](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Haz clic en **Añadir,** luego **en Aplicación pública.**
2. Selecciona **Android** en el menú desplegable de la plataforma y **Buscar en App Store par**a la fuente.
3. Ingresa “**Miro**” en el **cuadro de texto Nombre** y haz clic en siguiente.
4. Selecciona la aplicación de Miro y presiona **Aprobar** si se te solicita.
5. Publica la aplicación haciendo clic en **Guardar y asignar**.
6. Configura las asignaciones y los parámetros de distribución según las preferencias de tu organización.

**Ivanti Neurons**

La guía de implementación general de Ivanti Neurons se puede encontrar [aquí](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/92/all/Managing_Google_Play_apps.htm).

- 1. Ve a **Aplicaciones >** **Catálogo de aplicaciones) y haz lic en Añadir.**
  2. Selecciona "**Google Play Store**" y tu país como origen.
  3. Buscar "**Miro**" y selecciona "**Miro: Pizarra online**" de la lista de aplicaciones disponibles.
  4. Establece la configuración y las políticas de distribución según las preferencias de tu organización.

**Intune (Microsoft Endpoint Manager)**

Puedes encontrar la guía general de implementación de Intune de MS [aquí](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-android).

1. Ve a **Aplicaciones > Todas las aplicaciones** y haz clic en **Añadir**.
2. Selecciona **App de la tienda > Tienda de aplicaciones de Android** como el **Tipo de aplicación.**
3. En la **página Información de la aplicación,**completa los detalles desde la [lista de Miro en Google Play Store.](https://play.google.com/store/apps/details?id=com.realtimeboard)
4. Establece la configuración y las políticas de distribución según las preferencias de tu organización.

Establece la configuración y las políticas de distribución según las preferencias de tu organización.

### Completar previamente la configuración de la aplicación

Miro usa [AppConfig](https://www.appconfig.org/) como la forma unificada de configurar y proteger los datos de los clientes, lo que proporciona una manera fácil de configurar las aplicaciones móviles empresariales.  Muchas soluciones de EMM admiten el formato AppConfig o lo aceptan en un “modo de compatibilidad”. Para conocer las limitaciones exactas aplicables en tu caso, consulta la documentación de tu proveedor de EMM.

#### Ejemplos

**VMWare Workspace ONE**

La guía de implementación general de VMware Workspace ONE se puede encontrar [aquí](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Ve a **Recursos > Aplicaciones**.
2. Haz clic en **Asignar** en el **Estado de la instalación** en **Miro: Pizarra online** app row.
3. Define las **categorías Nombre, Grupos de asignación** y **Método de entrega de la aplicación** de la distribución.
4. Habilita **Acceso gestionado** y**Configuración de envío.**
5. Definir la configuración de la aplicación.

**Ivanti Neurons**

La guía de implementación general de Ivanti Neurons se puede encontrar [aquí](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/92/all/Using_the_Android_enterprise_App_Configuration.htm).

1. Ve a **Aplicaciones > Catálogo de aplicaciones**.
2. Navega hasta "**Miro: Pizarra online**" ajustes.
3. Ve a **Configuraciones de la aplicación > Configuraciones gestionadas para Android**.
4. Haz clic en **Añadir** para crear **Restricciones de aplicaciones**.
5. Define los parámetros **Requerido** y Permisos **de tiempo de ejecución** .
6. Selecciona el perfil de distribución en la **sección** Distribuir esta configuración de aplicación.

**Intune (Microsoft Endpoint Manager)**

Puedes encontrar la guía general de implementación de Intune de MS [aquí](https://learn.microsoft.com/mem/intune/apps/app-configuration-policies-use-android).

1. Ve a **Aplicaciones > Políticas de configuración de aplicaciones > Añadir > Dispositivos gestionados** para crear una nueva configuración de aplicación.
2. Define el nombre de tu perfil de configuración.
3. Selecciona **Android Enterprise** como **Plataforma**.
4. Selecciona **Miro: Pizarra online** como el **app de destino** haciendo clic en **Seleccionar app**.
5. Selecciona **Usar configuración de diseñador** ( como **Configuration setings format (Formato de configuración de ajustes**).
6. Definir la configuración de la aplicación.
7. Selecciona el perfil de distribución para la configuración.

## Lista completa de configuraciones compatibles

### Limitar las opciones de “Iniciar sesión con…"/"Registrarse"

Si la opción “Registrarse" está habilitada, todas las configuraciones de “Iniciar sesión con…" afectarán el flujo de registro.

:::warning
Cualquier clave que no esté explícitamente establecida como "verdadera" (o ausente) se considera "falsa". Por lo tanto, la opción de autenticación está disponible (comportamiento predeterminado).
:::

| Clave | Tipo | Valores permitidos |
| --- | --- | --- |
| **Facebook** miro.authentication.facebookRestricted | Booleano | verdadero/falso |
| Google miro.authentication.googleRestricted | verdadero/falso |
| **Microsoft Office 365** miro.authentication.office365Restricted | verdadero/falso |
| ****Slack****  miro.authentication.slackRestricted | verdadero/falso |
| registro miro.authentication.signUpRestricted | verdadero/falso |
| **Iniciar sesión con Magic link** miro.authentication.magicLinkRestricted | verdadero/falso |
| **Espacio de trabajo para empresas** miro.authentication.enterpriseEspacioTrabajoDeshabilitado | verdadero/falso |

### Restricciones de nombre de usuario

Los clientes que quieran mejorar la seguridad manteniendo la autenticación de contraseña simple pueden usar las siguientes opciones.

| Clave | Valor | Descripción |
| --- | --- | --- |
| **Nombre de usuario predefinido** miro.politica.autentificacion.nombreusuario | **Tipo de valor:** string | El campo está bloqueado y el usuario no puede cambiarlo. |
| **Dominios en lista blanca** miro.politica.autenticacion.dominiospermitidos | **Tipo de valor:** array  **Valor:** @miro.com, @yourdomain.com  *Algunos proveedores no admiten el tipo de datos **array**.  Si ese fuera el caso, utiliza el tipo **cadena** y la matriz JSON como valor. ["@miro.com", "@tudominio.com"] | Solo se permiten los correos electrónicos correspondientes a uno de los dominios enumerados. |

### Configuración de SSO

Para mejorar la seguridad de la organización y simplificar el proceso de autenticación para los usuarios finales, los administradores de la organización pueden configurar la política de SSO usando el siguiente ejemplo.

:::warning
Asegúrate de que la política de SSO en la configuración de la aplicación corresponda con la configuración de SSO de la organización de Miro. La incompatibilidad de esas políticas podría resultar en una situación de “bloqueo” cuando los usuarios no puedan iniciar sesión. Miro no puede validar la configuración antes de aplicarla en los dispositivos de destino.
:::

|  |  |
| --- | --- |
| Clave de configuración | miro.policy.sso |
| Tipo de valor de configuración | string |
| Objeto de política | \{ "authenticationRestricted" : falso, "email": "user@domain.com", "allowedDomains": ["domain1.com", "domain2.com"], "forceSsoLogin": verdadero \} |

| Atributos de objeto de política | | | |
| --- | --- | --- | --- |
| Parámetro | Tipo | Descripción | Nota |
| authenticationRestricted | booleano | Si el botón "Iniciar sesión con SSO" está habilitado en la página principal. | **La clave se ignora cuando se proporcionan otras opciones de configuración.** |
| correo electrónico | string | Correo electrónico predefinido para el inicio de sesión con SSO. | El campo está bloqueado y no se puede cambiar. |
| allowedDomains | booleano | Mantén el SSO como el único método disponible para la autenticación. | El usuario final es dirigido inmediatamente a "Página de inicio de sesión con SSO". Las opciones que no sean **correo electrónico** y **allowedDomains** se ignoran. No hay otros métodos de autenticación disponibles. |
