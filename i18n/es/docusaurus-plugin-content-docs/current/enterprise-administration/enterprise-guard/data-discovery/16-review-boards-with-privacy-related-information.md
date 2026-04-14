---
title: "Revisar tableros con informaci\xF3n relacionada con la privacidad"
article_id: 15431051181458
translation_id: 15431051181458
locale: es
sidebar_position: 15
created_at: '2023-11-29T16:31:14Z'
updated_at: '2025-11-25T15:39:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

El panel de descubrimiento de datos permite a los [admins de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) revisar las incidencias de datos relacionados con la privacidad detectados por el descubrimiento de datos y validar los resultados.

:::note
Para revisar tableros con datos relacionados con la privacidad, debes tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.
:::

Para revisar un tablero con datos relacionados con la privacidad, realiza los siguientes pasos:

1. Ve a tus [ajustes de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, en **Enterprise Guard**, haz clic en **Descubrimiento de datos**.
3. En la página de **Data discovery** **Overview**, desplázate hasta la sección debajo de las métricas y luego haz clic en el conteo de tableros para la categoría de tableros que deseas revisar.
   Aparece una nueva página con la lista de tableros y su información.
4. Haz clic en el tablero que quieras revisar.
   En la parte derecha de la pantalla aparece un panel lateral.
5. El panel desplegable te permite realizar las siguientes acciones:
   **Mostrar u ocultar** **información relacionada** **con la privacidad:** Por defecto. la información relacionada con la privacidad está ocultada. Si quieres ver información relacionada con la privacidad, haz clic en el **interruptor de Mostrar información sensible** para activarlo.
   Cuando la información relacionada con la privacidad es visible, puedes ocultar la información relacionada con la privacidad haciendo clic en el interruptor **Mostrar información sensible** para apagarlo.

   - **Filtrar** **información relacionada con la privacidad** **según la categoría de datos:** Para ver información relacionada con la privacidad que pertenece a una etiqueta específica, haz clic en la pestaña **Información relacionada con la privacidad**, y luego haz clic en la etiqueta de sensibilidad adecuada debajo de la pestaña.

   **- Suprimir coincidencias falsamente positivas:** Durante el proceso de descubrimiento de datos relacionados con la privacidad, podrías encontrarte con situaciones donde el sistema genera coincidencias que, aunque técnicamente precisas, pueden no ser relevantes o consideradas como datos sensibles según diversas políticas de seguridad y necesidades específicas de una organización. Suprimir una coincidencia que no representa un riesgo de seguridad o privacidad se vuelve crucial para adaptar el proceso de descubrimiento de datos a los requisitos específicos de seguridad y privacidad de una organización.

   Puede haber ocasiones en que el sistema marque incorrectamente los datos de tus tableros como probablemente sensibles (un falso positivo). Varios factores contribuyen a estos eventos, incluyendo la proximidad de términos relacionados o el formato de datos relacionados con la privacidad. También puedes suprimir los falsos positivos.

   Cuando suprimis una coincidencia, las actualizaciones suceden en tiempo real. La clasificación del tablero y las barreras de protección aplicadas también se actualizan según la configuración de Clasificación automática y Barreras de protección inteligentes.

   Para suprimir una coincidencia de falso positivo, haz clic en el icono de puntos suspensivos al lado de la coincidencia de datos relacionados con la privacidad que deseas suprimir y luego selecciona **Ocultar coincidencia**. Ten en cuenta que las actualizaciones ocurren en tiempo real. La clasificación del tablero y las barreras de protección aplicadas también se actualizan según la configuración de Clasificación automática y Barreras inteligentes.
6. Haz clic en el siguiente tablero con el que quieras trabajar en la lista de resultados del Explorador de contenido y realiza las acciones necesarias, o cierra el panel deslizable haciendo clic en el botón **Cerrar** en la parte superior derecha del panel.
