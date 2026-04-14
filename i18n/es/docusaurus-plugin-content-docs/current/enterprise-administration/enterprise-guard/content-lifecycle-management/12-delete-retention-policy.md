---
title: "Eliminar la pol\xEDtica de retenci\xF3n"
article_id: 19205219887762
translation_id: 19205219887762
locale: es
sidebar_position: 12
created_at: '2024-05-28T18:02:52Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

Eliminar una política de retención libera los tableros retenidos asociados a la política de retención. Estos tableros pueden eliminarse permanentemente sin restricciones.

:::note
Para eliminar políticas de retención, debes tener el [Data Governance Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de gobernanza de datos, ponte en contacto con el admin de empresa.
:::

Para eliminar una política de retención, sigue estos pasos:

1. Ve a tu [configuración de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, en **Enterprise Guard**, haz clic en **Ciclo de vida del contenido**.
3. Haz clic en la pestaña **Retención**.
4. En la página de **Políticas** de **retención**, haz clic en la política de retención que quieras eliminar.
   Aparece la página que muestra la información relacionada con la política.
5. Haz clic en **Eliminar** en la parte superior derecha de la página.
6. Revisa el impacto que tiene eliminar esta política de retención. La página de revisar impacto proporciona la siguiente información:
   - **Resumen:** configuración de la política de retención, como el nombre de la política, el periodo de retención y el alcance.
   - **Impacto de la política:** número de tableros que se liberarán de la retención y podrán eliminarse permanentemente sin restricciones. La política de retención también es aplicable a los tableros en la papelera y se incluyen en el cálculo del impacto de la revisión.
7. Para eliminar la política de retención, haz clic en **Eliminar política**.

:::note
La creación, actualización o eliminación de una política activa el proceso de políticas de retención, que puede tardar hasta 24 horas en completarse. Sin embargo, la actualización del nombre o la descripción de una política se produce inmediatamente, ya que estas acciones no activan el proceso de las políticas de retención.
:::
