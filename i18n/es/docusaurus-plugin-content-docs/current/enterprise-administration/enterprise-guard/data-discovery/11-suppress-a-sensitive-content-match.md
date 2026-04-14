---
title: Suprimir un resultado de contenido sensible
article_id: 17144258002962
translation_id: 17144258002962
locale: es
sidebar_position: 10
created_at: '2024-02-20T00:16:59Z'
updated_at: '2025-11-25T15:41:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

En el proceso de descubrimiento de datos, podrías encontrarte situaciones en las que el sistema generó resultados que, aunque técnicamente sean correctos, podrían no ser pertinentes o considerarse datos sensibles de acuerdo con diversas políticas de seguridad y las necesidades específicas de una organización. Suprimir un resultado que no represente un riesgo a la seguridad o la privacidad se hace crucial para adaptar el proceso de descubrimiento de datos a la medida de los requisitos de seguridad y privacidad de datos específicos de una organización.

También podría haber veces en las que el sistema incorrectamente marque información en tus tableros como posiblemente sensible (un falso positivo). Varios factores contribuyen para que se produzca esta situación, incluidos la proximidad de los términos relacionados o el formato de los datos sensibles. También puedes suprimir los resultados que sean falsos positivos.

Al suprimir un resultado, las actualizaciones se hacen en tiempo real. La clasificación del tablero y las barreras de protección aplicadas también se actualizan conforme a la configuración de autoclasificación y de las barreras de protección inteligentes.

:::note
Para suprimir un resultado de contenido sensible, tienes que tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, comunícate con el admin de tu empresa.
:::

Para suprimir un resultado de contenido sensible, sigue los siguientes pasos:

1. Si estás en la página **del explorador de contenido**, pasa al paso 2.
   Si no estás en la página **del explorador de contenido**:
   a. Ve a la [configuración de Miro.](https://help.miro.com/hc/articles/https://miro.com/app/settings)
   b. En el panel izquierdo, en **Seguridad y cumplimiento**, haz clic en **Explorador de contenido**.
2. En la página **Explorador de contenido/descubrimiento de datos**, haz clic en el tablero que quieras revisar.
   Aparecerá un panel de ocultación a la derecha de la pantalla.
   ![Figura 1: Panel de ocultación](images/21017529200018_slide_out_panel.png)*Figura 1: Panel de ocultación*
3. Haz clic en los puntos suspensivos que están junto al resultado de datos sensibles que quieras suprimir y luego haz clic en **Hide match** (‘ocultar resultado’). Ten en cuenta que las actualizaciones suceden en tiempo real. La clasificación del tablero y las barreras de protección aplicadas también se actualizan conforme a la configuración de autoclasificación y de las barreras de protección inteligentes.

    Al suprimir un resultado, las actualizaciones se hacen en tiempo real. La clasificación del tablero y las barreras de protección también se actualizan conforme a la configuración de autoclasificación y de las barreras de protección inteligentes.

   Repite este paso para cada resultado de datos sensibles que quieras suprimir.
4. Haz clic en el siguiente tablero en el que quieras trabajar de la lista de resultados del explorador de contenido y haz las acciones necesarias, o cierra el panel de ocultación haciendo clic en el botón **Close** (‘cerrar’) que está en la parte superior derecha del panel.
