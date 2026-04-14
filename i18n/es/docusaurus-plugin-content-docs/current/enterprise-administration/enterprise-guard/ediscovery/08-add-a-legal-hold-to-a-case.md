---
title: "Agregar una retenci\xF3n legal a un caso"
article_id: 22120471564946
translation_id: 22120471564946
locale: es
sidebar_position: 7
created_at: '2024-10-21T23:29:24Z'
updated_at: '2025-11-25T16:22:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Crear un bloqueo legal es un proceso crítico para los [eDiscovery Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) cuando se espera un litigio o una investigación. Los bloqueos legales aseguran que los tableros de Miro relevantes se conserven y protejan de alteraciones, eliminación o remoción. Esto es esencial para mantener el cumplimiento con los requisitos legales y regulatorios, prevenir la pérdida o modificación de datos críticos y salvaguardar pruebas clave durante la duración del asunto legal. Un bloqueo legal permite a los administradores asegurar los datos, garantizando que todos los tableros de Miro relevantes estén disponibles para revisión cuando sea necesario.

Crear una retención legal implica identificar a los usuarios relevantes y tableros de Miro asociados con un caso y aplicar la retención para evitar cualquier modificación. Los admins pueden gestionar múltiples retenciones dentro de un caso, asegurándose de que todos los datos necesarios se agrupen y conserven de manera organizada. Este proceso ayuda a mantener la integridad y la responsabilidad de los datos, asegurando que la organización esté completamente conforme y preparada para el proceso legal.

Aún se puede acceder y editar los tableros de Miro bajo retención legal, pero se preservan todas las versiones. Si el contenido se elimina, aún estará disponible bajo la retención legal. La cantidad de contenidos bajo retención podría aumentar en función de las acciones futuras de los usuarios. Después de que un tablero sea colocado en retención legal, todas las versiones del tablero se retendrán indefinidamente hasta que la retención sea levantada.

Para crear una retención legal, realiza los siguientes pasos:

:::note
Debes tener el [rol de admin de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) para realizar esta tarea. Para solicitar el rol de admin de eDiscovery, ponte en contacto con el admin de empresa.
:::

1. Ve a tu configuración de Miro.
2. En el panel izquierdo, bajo **Enterprise Guard**, haz clic en **eDiscovery**.
3. En la página de **eDiscovery**, haz clic en la pestaña **Casos**.
4. En la página de **Crear caso**, haz clic en el caso en el que deseas añadir una retención legal.
5. Haz clic en **Añadir retención legal**.
6. En la página **Añadir retención legal**, ingresa o selecciona la información apropiada para cada campo. La siguiente tabla lista cada campo y su descripción.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | Nombre de la retención legal  **(obligatorio)** | Nombre de la retención legal.  Longitud máxima: 60 caracteres. |
   | Criterios  **(obligatorio)** | Tipo de contenido incluido para esta retención legal. Esta versión solo admite todo el contenido. |
   | **Usuarios que son propietarios, copropietarios, accedieron, modificaron o crearon contenido**  **(obligatorio)** | Agrega los usuarios que deseas poner en retención legal. Haz clic en el campo para buscar por nombre o correo electrónico. Puedes añadir hasta 200 usuarios de una sola vez.    **Notas:**  - Cuando un usuario bajo retención legal abre, modifica o interactúa con un tablero de cualquier forma (renombrando o añadiendo contenido), ese tablero se marca y conserva. Por ejemplo, si se cambia el nombre del tablero o se actualiza el contenido, será automáticamente puesto en retención legal. Además, la propiedad y creación del tablero se suspenden.  - Cuando se crea una retención legal, se aplica a los tableros que los custodios crearon, poseían o coposeían en el momento de la retención. Además, cualquier tablero que los custodios acceden y modifican después de que la retención esté en su lugar también se incluye. Los detalles históricos de acceso y actualización de tableros no están disponibles en esta versión. |
7. Haz clic en **Siguiente**. Aparece la página de **Revisar impacto**.
8. Revisa el impacto de esta creación de retención legal, como el número de tableros existentes que se retendrán y los usuarios que eran propietarios, copropietarios, accedieron, modificaron o crearon los tableros.

   **Notas:**
   - Es posible acceder a los tableros bajo retención y editarlos, pero se conservarán todas las versiones. Si el contenido se elimina, seguirá estando disponible en el ámbito de la retención. La cantidad de contenidos bajo retención podría aumentar en función de las acciones futuras de los usuarios.

   - Cuando un usuario bajo retención legal abre, modifica o interactúa con un tablero de cualquier manera (cambiando el nombre o agregando contenido), ese tablero se marca y se preserva. Por ejemplo, si se cambia el nombre del tablero o se actualiza el contenido, se colocará automáticamente en retención legal. Además, la propiedad y la creación del tablero quedan en espera.

   - Cuando se crea una retención legal, se aplica a los tableros que los custodios crearon, poseían o co-poseían en el momento de la retención. Además, cualquier tablero al que los custodios accedan y modifiquen después de que la retención esté en vigor también queda incluido. En esta versión no están disponibles los detalles históricos de acceso y actualización de tableros.
9. Después de revisar el impacto de la retención legal que estás creando, haz clic en **Agregar retención legal**.
    La página del caso aparece mostrando la retención legal que contiene y la información sobre cada retención legal, como el nombre de la retención legal, el tipo de contenido afectado por la retención legal, el número de usuarios en esta retención legal, la fecha de creación de la retención legal, el estado de la retención legal y el número de tableros que están en retención legal.
