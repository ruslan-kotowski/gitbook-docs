---
title: "Editar una retenci\xF3n legal"
article_id: 27968005251090
translation_id: 27968005251090
locale: es
sidebar_position: 8
created_at: '2025-07-09T17:31:49Z'
updated_at: '2025-11-25T15:52:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Editar una retención legal permite a los admins de eDiscovery ajustar y refinar los esfuerzos de conservación legal en curso a medida que evolucionan los requisitos del caso. Ya sea que se identifiquen nuevos custodios, que más tableros de Miro se vuelvan relevantes, o que los tableros o usuarios existentes ya no estén en el alcance, editar una retención legal asegura que los datos correctos se mantengan preservados y defendibles a lo largo del proceso legal.

Los admins pueden actualizar el nombre o la descripción del "legal hold" y agregar o eliminar usuarios y tableros según sea necesario. Esta flexibilidad soporta flujos de trabajo legales dinámicos y garantiza que la conservación se mantenga precisa, actualizada y alineada con el alcance del asunto legal, manteniendo el cumplimiento mientras se evita la retención innecesaria de datos.

Cuando se edita una retención legal:

- Los tableros recién añadidos a la retención comenzarán a tener sus versiones preservadas a partir de ese momento.
- Los tableros o usuarios eliminados de la retención dejarán de ser preservados, y sus versiones ya no se conservarán como parte de esa retención legal.
- Los tableros que permanecen bajo retención seguirán teniendo todas las versiones preservadas, incluidas las eliminaciones que ocurran después de aplicar la retención.

Este enfoque garantiza que las organizaciones puedan responder a las demandas legales con precisión y responsabilidad a medida que un caso evoluciona.

Para editar una retención legal, realiza los siguientes pasos:

:::note
Debes tener el rol de [Admin de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) para realizar esta tarea. Para solicitar el rol de admin de eDiscovery, ponte en contacto con el admin de empresa.
:::

1. Ve a tu configuración de Miro.
2. En el panel izquierdo, bajo **Enterprise Guard**, haz clic en **eDiscovery**.
3. En la página de **eDiscovery**, haz clic en la pestaña de **Casos**.
4. Haz clic en la investigación dentro de la cual quieras editar una retención legal.
   La lista de retenciones legales dentro del caso aparece.
5. Haz clic en los tres puntos en la fila de la retención legal que deseas editar y luego haz clic en **Editar retención legal**.
6. En la página **Editar retención legal**, introduce o selecciona la información adecuada para cada campo. La tabla siguiente enumera cada campo y su descripción.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | Nombre de la retención legal  **(requerido)** | Nombre de la retención legal.  Longitud máxima: 60 caracteres. |
   | Criterios  **(requerido)** | Tipo de contenido incluido para esta retención legal. Esta versión solo admite todo el contenido. |
   | **Usuarios que son propietarios, copropietarios, accedieron, modificaron o crearon contenido**  **(requerido)** | Agrega los usuarios que quieres poner en retención legal. Haz clic en el campo para buscar por nombre o correo electrónico. Puedes tener hasta 200 usuarios por retención legal, incluidos los usuarios añadidos en las actualizaciones de retención legal.  **Notas:**  Cuando un usuario bajo retención legal abre, modifica o interactúa con un tablero de cualquier manera (renombrándolo o añadiendo contenido), ese tablero es marcado y preservado. Por ejemplo, si se cambia el nombre del tablero o se actualiza el contenido, se colocará automáticamente en retención legal. Además, la propiedad y creación de tableros se encuentran en espera.  - Cuando se edita una retención legal, se aplica a los tableros que los custodios crearon, poseían o coposeían en el momento de la retención. Además, cualquier tablero al que los custodios accedan y modifiquen después de que la retención esté en vigor también se incluye. El acceso histórico y los detalles de actualización del tablero no están disponibles en esta versión.  Los tableros recién agregados a la retención comenzarán a tener sus versiones preservadas desde el momento en que guardes las actualizaciones de la retención legal en el paso 9.  Los tableros o usuarios que se eliminen de la retención legal dejarán de ser preservados, y sus versiones ya no se mantendrán como parte de esa retención legal.  Los tableros que permanecen bajo retención seguirán conservando todas las versiones, incluidas las eliminaciones que ocurran después de que se aplicó la retención. |
7. Haz clic en **Siguiente**. La página de **revisar impacto** aparece.
8. Revisa el impacto de la creación de esta retención legal, como:
   - El número de tableros que permanecen en retención, que se liberarán de la retención y que se añadirán a la retención.
   - Los usuarios que eran propietarios, copropietarios, accedieron, modificaron o crearon los tableros.
   - Los criterios para la retención.
   - La lista de tableros que permanecen bajo retención.

   **Notas:**
   Los tableros bajo retención aún se pueden acceder y editar, pero se preservarán todas las versiones. Si el contenido se elimina, seguirá estando disponible en el ámbito de la retención. La cantidad de contenidos bajo retención podría aumentar en función de las acciones futuras de los usuarios.

   Cuando un usuario bajo retención legal abre, modifica o interactúa con un tablero de cualquier forma (renombrando o añadiendo contenido), ese tablero se marca y conserva. Por ejemplo, si se cambia el nombre del tablero o se actualiza el contenido, se colocará automáticamente en retención legal. Además, se suspenden la propiedad y la creación de tableros.

   - Cuando se crea una retención legal, se aplica a los tableros que los custodios crearon, poseen o coposeen en el momento de la retención. Además, cualquier tablero que los custodios accedan y modifiquen después de que se haya aplicado la retención también se incluirá. El acceso histórico al tablero y los detalles de actualización no están disponibles en esta versión.
9. Después de revisar el impacto de la retención legal que estás creando, haz clic en **Guardar retención legal**.
   La página del caso aparece mostrando la retención legal actualizada, como el nombre de la retención legal, el tipo de contenido afectado por la retención legal, la cantidad de usuarios en esta retención legal, la fecha de creación de la retención legal, el estado de la retención legal y la cantidad de tableros que están en retención legal.
