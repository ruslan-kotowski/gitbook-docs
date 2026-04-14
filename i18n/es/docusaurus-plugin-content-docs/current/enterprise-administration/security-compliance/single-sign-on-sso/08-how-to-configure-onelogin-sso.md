---
title: Cómo configurar SSO para OneLogin
article_id: 360022547134
translation_id: 360022547134
locale: es
sidebar_position: 8
created_at: '2019-05-07T13:32:16Z'
updated_at: '2025-02-26T11:22:04Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible para: [Empresa](../../../plans-billing/miro-plans/04-enterprise-plan.md),
    planes [Business](../../../plans-billing/miro-plans/06-business-plan.md) Configurado
    por: admins de empresa'
---

> *Se recomienda enfáticamente configurar el SSO en una ventana en modo incógnito por separado del navegador.* De esta manera, mantienes la sesión en la ventana estándar, lo que te permite desactivar la autorización de SSO en caso de que algo esté configurado de forma incorrecta.

Si deseas configurar una instancia de prueba antes de activar el SSO en la producción, solicítala a tu Account Executive o representante de Ventas. Solo se agregará a esta instancia de prueba a quienes configuren SSO.

> **⚠️ Consulta aquí nuestro artículo principal sobre SSO** **para conocer las reglas, las funciones compatibles y la configuración opcional desde Miro.**

## Configuración de Onelogin

### Cómo añadir y configurar la aplicación

La configuración de OneLogin en Miro es sencilla, ya que OneLogin tiene una aplicación de trabajo preconfigurada de Miro en el catálogo de **aplicaciones**.

Miro_en_apps_OneLogin.jpg
Miro en el catálogo de aplicaciones de OneLogin

Haz clic en el botón **Save** (Guardar).

botón_guardar.jpg
Pestaña de configuración de aplicaciones en OneLogin

## Configuración de Miro

Después de guardar la configuración, se te dirigirá directamente a los ajustes de la aplicación. Cambia a la pestaña **SSO** para obtener tu **Login URL** (URL de inicio de sesión) y tu **x509 Certificate**.

pestaña_sso.jpg
Pestaña SSO

A continuación, verás una lista de URL. Copia la URL **SAML 2.0 Endpoint (HTTP)**:

endpoint_de_SAML.jpg

y ***pégalo*** en el campo **SAML Sign-In URL** (URL de inicio de sesión de SAML) de Miro:

URL_inicio_sesión.jpg
**Campo SAML Sign-In URL (URL de inicio de sesión de SAML) en Miro**

Regresa a la pestaña SSO de la aplicación OneLogin y haz clic en **View Details** (Ver detalles) para copiar el **x509 Certificate**.

ver_detalles.jpg
Botón View Details (Ver detalles)

copiar_certificado.jpg
**Copiar x509 Certificate**

Pega el certificado en el campo **x509 Certificate** de Miro.

certificado_en_ajustes_SSO_Miro.jpg
**Campo x509 Certificate en los ajustes de SSO de Miro**

Como paso final de los ajustes de Miro, agrega tus dominios y [verifícalos](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). También puedes configurar los ajustes opcionales.

¡Listo! Ahora tus usuarios podrán autenticarse en Miro vía SSO.

Si tienes algún problema, consulta [nuestra lista de casos comunes y cómo resolverlos.](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)

## Probar la configuración de SSO en Miro

1. Completa los pasos anteriores para configurar tus ajustes SSO.
2. Haz clic en el botón **Probar configuración SSO**.
3. Revisa los resultados:

- Si no se encuentra ningún problema, se mostrará un mensaje de confirmación de que **la prueba de configuración SSO se ha realizado correctamente**.
- Si se encuentran problemas, se mostrará un mensaje de confirmación **Prueba de configuración SSO fallida**, seguido de mensajes de error detallados para orientarte sobre lo que hay que arreglar.

![prueba-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Probar la configuración de SSO en Miro*
