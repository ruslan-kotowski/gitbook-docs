---
title: "Revisar tableros con informaci\xF3n sensible de la empresa y personalizada\
  \ (Beta)"
article_id: 24090123693586
translation_id: 24090123693586
locale: es
sidebar_position: 13
created_at: '2025-01-21T15:10:56Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

El explorador de contenido permite a los [admins de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) revisar las ocurrencias de coincidencias de datos sensibles de la empresa o personalizados.

:::note
- Para revisar tableros con coincidencias de datos sensibles de la empresa o personalizados, debes tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.
- Las coincidencias de datos sensibles de la empresa están etiquetadas como CUSTOMER, TECH o STRATEGY y los resultados se listan en la parte superior de la lista de resultados.

- Las coincidencias de datos sensibles personalizados de la empresa se etiquetan con las etiquetas personalizadas adecuadas aplicables.
:::

Para revisar un tablero con coincidencias de datos sensibles de la empresa o datos sensibles personalizados de la empresa, realiza los siguientes pasos:

1. Si estás en la página del **explorador de contenido**, pasa al paso 2.
   Si no estás en la página del **explorador de contenido**:
   a. Ve a tu [configuración de Miro](https://miro.com/app/settings).
   b. En el panel izquierdo, bajo **Enterprise Guard**, haz clic en **explorador de contenido**.
   c. Haz clic en **descubrimiento de datos**.
2. En la página **Explorador de contenido/Descubrimiento de datos**, haz clic en el tablero que quieres revisar.
   Aparece un panel lateral a la derecha de la pantalla.
3. El panel lateral te permite realizar las siguientes acciones:

   - Para coincidencias de datos sensibles de la empresa personalizados únicamente: Mostrar u ocultar **información sensible de la empresa**
   De forma predeterminada, la información sensible de la empresa personalizada está oculta. Si deseas ver la información centrada en datos personalizados de la empresa, habilita el interruptor **Mostrar información sensible**.
   Cuando la información sensible personalizada es visible, puedes ocultarla al deshabilitar el interruptor **Mostrar información sensible**.datos sensibles de la empresa son visibles, puedes ocultar los datos al hacer clic en el interruptor **Mostrar información confidencial** para desactivarlo.

   > ✏️ - Los datos sensibles de la empresa se etiquetan como CLIENTE, TECNOLOGÍA, o ESTRATEGIA y los resultados se listan en la parte superior de la lista de resultados.
   > - Los datos sensibles personalizados de la empresa se etiquetan con las etiquetas personalizadas correspondientes.

   - Para tanto los datos sensibles de la empresa como los datos personalizados sensibles de la empresa: **Filtra la información según la categoría de datos sensibles de la empresa**
   Para ver datos sensibles de la empresa que pertenecen a una categoría específica, haz clic en la pestaña **Información sensible de la empresa** y luego haz clic en el botón de filtro adecuado debajo de la pestaña.

   -Solo para coincidencias de datos sensibles de la empresa: **Suprimir las falsas coincidencias**
   En el proceso de descubrimiento de datos sensibles de la empresa, podrías encontrarte con situaciones donde el sistema genera coincidencias que, aunque técnicamente precisas, pueden no ser relevantes o consideradas como datos sensibles basados en varias políticas de seguridad y las necesidades específicas de una organización. Suprimir una coincidencia que no representa un riesgo de seguridad o empresarial se vuelve crucial para adaptar el proceso de descubrimiento de datos a los requisitos específicos de seguridad de datos y de negocio de una organización.

   También puede haber momentos en que el sistema marque incorrectamente datos en tus tableros como probablemente sensibles (un falso positivo). Varios factores contribuyen a estas ocurrencias, incluyendo la proximidad de términos relacionados o el formato de datos relacionados con el negocio. También puedes suprimir coincidencias de falsos positivos.

   Cuando suprimes una coincidencia, las actualizaciones ocurren en tiempo real. La clasificación del tablero y las barreras de protección aplicadas también se actualizan según la configuración de Auto-clasificación y Barreras de Protección Inteligentes.

   Para suprimir una coincidencia de falso positivo, haz clic en el ícono de tres puntos junto a la coincidencia de datos sensible de la empresa que deseas suprimir, y luego selecciona **Ocultar coincidencia**. Ten en cuenta que las actualizaciones se realizan en tiempo real. La clasificación del tablero y las barreras de protección aplicadas también se actualizan según la configuración de Clasificación automática y Barreras Inteligentes.
4. Haz clic en el siguiente tablero con el que deseas trabajar en la lista de resultados del explorador de contenido y realiza las acciones necesarias, o cierra el panel desplegable haciendo clic en el botón **Cerrar** en la parte superior derecha del panel.
