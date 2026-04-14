---
title: Autenticación de dos factores (2FA)
article_id: 27356474050834
translation_id: 27356474050834
locale: es
sidebar_position: 1
created_at: '2025-06-12T12:01:03Z'
updated_at: '2025-06-24T08:19:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: 'Quién puede hacerlo: admins de equipo, admins de empresa ¿Cuáles planes:
    Starter, Business, Education, Enterprise ¿Cuáles plataformas: Navegador, escritorio,
    móvil'
---

La autenticación de dos factores (2FA) añade una capa adicional de seguridad a las cuentas en línea al requerir que los usuarios proporcionen dos métodos de verificación únicos antes de acceder a sus cuentas.

Los admins de Miro pueden habilitar la 2FA para sus equipos y restablecer la 2FA para los miembros del equipo. Los usuarios tienen la opción de confiar en un dispositivo durante 30 días.

:::note
Este artículo explica 2FA para los planes Starter, Business y Education. Para obtener información sobre 2FA para Enterprise, consulta [Autenticación de dos factores (2FA) (guía del admin).](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)
:::

## Habilitar la autenticación de dos factores (2FA)

Para los planes Starter y Education, asegúrate de tener el rol de admin de equipo.

Para un plan Business, asegúrate de tener el rol de admin de empresa.

Sigue estos pasos:

1. Desde tu panel de Miro, haz clic en tu avatar en la esquina superior derecha y selecciona **Admin Console**.
2. Ve a **Seguridad** > **Permisos**.
   (Education) Ve a **Permisos**.
   Ve a **Seguridad** > **Autenticación** de Business.
3. Bajo **Autenticación de dos factores (2FA)**, activa el interruptor **Requerir la autenticación de dos factores al iniciar sesión** en la posición de encendido.

## Configuración de la autenticación de dos factores (2FA) para usuarios

Para los equipos que tienen 2FA habilitada, los usuarios deben autenticarse usando una aplicación de autenticación, además de su correo electrónico y contraseña.

Para aprender cómo configurar 2FA como usuario, consulta [Autenticación de dos factores (2FA) – guía del usuario](02-two-factor-authentication-2fa-–-user-guide.md).

## Dispositivos de confianza

Un usuario que inicia sesión en Miro con 2FA puede optar por confiar en su dispositivo.

Al usar el dispositivo de confianza para iniciar sesión, al usuario solo se le pedirá autenticarse con su primer factor, omitiendo el segundo factor, porque el dispositivo es de confianza.

![](../../../../../../docs/administration/security-compliance/images/27358547112978_image.png)

*El dispositivo de confianza para 2FA está habilitado de forma predeterminada.*

En el inicio de sesión, **Confiar en este dispositivo durante 30 días** está seleccionado por defecto, lo cual el usuario puede deseleccionar opcionalmente.

:::note
El periodo de confianza del dispositivo solo se puede modificar en un plan Enterprise. Para obtener más información, consulta [Autenticación de dos factores (2FA) (guía del admin)](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).
:::

Para quitar la confianza a un dispositivo que se confió accidentalmente, un usuario puede cerrar sesión en todos los lugares. Ve a **perfil**, en **Configuración de perfil**, haz clic en **Cerrar sesión en todas partes**.

## Restablecer la autenticación de dos factores (2FA)

Si un usuario pierde el acceso a su segundo factor, entonces puede solicitar que su admin restablezca su 2FA.

Para restablecer 2FA para usuarios en planes Starter y Education, asegúrate de tener el rol de admin de equipo.

Para restablecer el 2FA para los usuarios en un plan Business, asegúrate de tener el rol de admin de empresa.

Sigue estos pasos:

1. Desde tu panel de Miro, haz clic en tu avatar en la esquina superior derecha y selecciona **Admin Console**.
2. Ve a **Usuarios** > **Todos los usuarios**.
3. Ubica al usuario, luego selecciona los tres puntos (**...**) al final de la fila.
4. Haz clic en **Restablecer la autenticación de dos factores**.
   El usuario recibe las instrucciones de restablecimiento por correo electrónico.
