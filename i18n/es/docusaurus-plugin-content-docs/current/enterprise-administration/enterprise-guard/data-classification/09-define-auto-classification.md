---
title: "Definir la clasificaci\xF3n autom\xE1tica"
article_id: 16494707596050
translation_id: 16494707596050
locale: es
sidebar_position: 9
created_at: '2024-01-19T19:01:08Z'
updated_at: '2025-11-25T15:40:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Para ayudarte a proteger tu contenido sensible, Enterprise Guard incluye la función de autoclasificación: un proceso automatizado de clasificación de datos, que clasifica los tableros de Miro en función del nivel de su contenido sensible. La clasificación automática representa un avance significativo en la forma de gestionar y proteger tus datos sensibles. Automatizar el proceso de clasificación ayuda a tu organización a mantener un mayor nivel de seguridad de los datos, cumplir los requisitos normativos y proporcionar una mejor experiencia a los admins de seguridad. La transición de la clasificación manual a la automática es un paso estratégico hacia un marco de seguridad de datos más preciso, seguro y eficaz.

Para más información sobre la [autoclasificación](03-auto-classification-overview-and-scenarios.md) y ejemplos de escenarios, consulta [Visión general de la autoclasificación](03-auto-classification-overview-and-scenarios.md).

## Definir la clasificación automática

Este es el segundo paso del flujo de configuración de la autoclasificación y las barreras de protección. En este paso del flujo, configurarás la etiqueta de sensibilidad de autoclasificación aplicable a cada nivel de clasificación. La clasificación de tableros se aplica automáticamente a todos los tableros nuevos y existentes que coincidan con los criterios definidos. Esto se hace después de que revises el impacto y decidas publicar actualizaciones.

## Requisitos previos

- [Debes habilitar el descubrimiento de datos](../data-discovery/13-activate-privacy-related-data-discovery.md).
- Debes completar el primer paso del flujo de autoclasificación y barreras de protección, [1: Definir los niveles de clasificación](07-define-classification-levels.md)
- Debes conocer las etiquetas de sensibilidad que quieres asignar a cada nivel de clasificación en función de tus requisitos de seguridad y gobernanza.
- Debes tener el [rol admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.

## Asigna etiquetas de sensibilidad para la autoclasificación

Para asignar etiquetas de sensibilidad a un nivel de clasificación, realiza los siguientes pasos:

1. En la página **Definir autoclasificación**, haz clic en el icono **Editar** del nivel de clasificación al que quieras asignar las etiquetas de sensibilidad. Por ejemplo, si quieres asignar las etiquetas de sensibilidad de la clasificación automática para el nivel de clasificación **CONFIDENCIAL**, haz clic en el icono Editar de la fila del nivel de clasificación **CONFIDENCIAL**.
2. Marca la casilla de cada etiqueta de sensibilidad que quieras asignar a este nivel de clasificación. Por ejemplo, si quieres clasificar automáticamente todos los tableros que contengan datos sensibles relacionados con el GDPR, selecciona la casilla de verificación **Reglamento General de Protección de Datos GDPR**. Puedes asignar una o varias etiquetas de sensibilidad por etiqueta de clasificación.
3. Haz clic en Done (listo).
   La clasificación de tableros se aplica automáticamente a todos los tableros nuevos y existentes que coincidan con los criterios definidos. Esto se hace después de que revises el impacto y decidas publicar actualizaciones.
4. Cuando hayas terminado de asignar etiquetas de sensibilidad para los distintos niveles de clasificación, pasa a [Completar la configuración de la clasificación automática](09-define-auto-classification.md).

## Configuración completa de autoclasificación

Cuando hayas terminado de asignar etiquetas de sensibilidad para la autoclasificación, haz clic en **Siguiente**. Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) de la página Revisar impacto.

A continuación, puedes seguir cualquiera de los siguientes pasos:

- Definir las barreras de protección Esto es opcional. Si quieres definir las barreras de protección en un momento posterior, haz clic en **Siguiente**.
- Revisar el impacto Este es el último paso del flujo de trabajo y es obligatorio.
