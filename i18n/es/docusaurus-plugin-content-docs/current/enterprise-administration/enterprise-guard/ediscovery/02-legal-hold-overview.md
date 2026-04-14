---
title: "Descripci\xF3n general de la retenci\xF3n legal"
article_id: 21922434361618
translation_id: 21922434361618
locale: es
sidebar_position: 1
created_at: '2024-10-11T12:20:34Z'
updated_at: '2025-11-25T15:48:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

La función de Retención Legal está diseñada para apoyar los procesos de cumplimiento y eDiscovery al preservar tableros que están sujetos a investigación o son relevantes para casos legales en curso.

[Los administradores de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) pueden prevenir la eliminación permanente de contenido creando bloqueos legales basados en usuarios específicos y sus acciones en Miro. Esta funcionalidad es esencial para garantizar que la información relevante se mantenga y se asegure durante los procedimientos legales.

Por ejemplo, cuando un usuario que está sujeto a una retención legal interactúa con un tablero, ese tablero se coloca automáticamente en retención para evitar su eliminación permanente.

Además, todas las versiones del tablero también se conservan, asegurando que el contenido del tablero se retenga para fines legales.

![legalholdoverview.png](images/22388794093842_legalholdoverview.png)

:::note
Debes tener el rol de [Administrador de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) para realizar tareas de Retención Legal. Para solicitar el rol de Admin de eDiscovery, ponte en contacto con el Admin de Empresa.
:::

## Beneficios Clave de la Retención Legal

- **Preservación de la Información:** La retención legal garantiza que todos los datos relevantes se conserven, evitando su eliminación permanente. Esto es crucial para el cumplimiento normativo y las investigaciones legales, ya que garantiza que los datos presentados en casos legales se mantengan precisos y sin alterar.
- **Cumplimiento de los requisitos legales:** Legal Hold apoya a las organizaciones a cumplir con las obligaciones legales y reglamentarias al garantizar que la información necesaria se retenga y esté disponible cuando se necesite, ayudando a evitar sanciones o desafíos legales.
- **Mitigación de riesgos:** Al proteger datos importantes, Legal Hold reduce el riesgo de pérdida de datos que podría resultar en consecuencias legales o financieras significativas.
- **Supervisión y auditoría:** Cada vez que se crea o modifica una retención legal, se genera un registro de auditoría que proporciona visibilidad y trazabilidad completas. Todos los registros de auditoría en una organización se conservan indefinidamente cuando hay al menos una retención legal activa. Esto garantiza la responsabilidad y la transparencia en la gestión de retenciones legales.

## Cómo funciona la retención legal

- **Interacciones del Usuario o del Tablero:** Cuando un usuario en retención legal abre, modifica o interactúa de cualquier manera con un tablero (cambiando su nombre o agregando contenido), ese tablero se marca y conserva. Por ejemplo, si se cambia el nombre del tablero o se actualiza el contenido, se colocará automáticamente en retención legal. Además, la propiedad del tablero y la creación de tableros están en espera.

  Cuando se crea una retención legal, esta se aplica a los tableros que los custodios crearon, son propietarios o copropietarios en el momento de la retención. Además, cualquier tablero al que los custodios acceden y modifican después de que la retención esté en su lugar también está incluido. El acceso al tablero histórico y los detalles de actualización no están disponibles en esta versión.
- **Acciones del usuario final y eliminación del tablero:** Aunque los usuarios finales pueden eliminar tableros, estos se conservan si hay una retención legal. Permanecen inaccesibles para el usuario final, pero se retienen para fines legales y administrativos.
- **Control Administrativo:** Los admins de eDiscovery pueden crear y eliminar retenciones legales a través de la sección de eDiscovery en la configuración. Las retenciones legales pueden aplicarse a todos los tableros que un usuario haya creado, poseído, coposeído, editado o accedido. Para gestionar múltiples retenciones legales, los administradores pueden primero crear un caso bajo el cual se agruparán estas retenciones.
- **Eliminación de equipo:** Si un tablero bajo retención legal existe dentro de un equipo, ese equipo no se puede eliminar de forma permanente hasta que se libere la retención. Esto previene la pérdida involuntaria de datos, asegurando que todo el contenido relevante se conserve. En los casos en que se elimina un equipo pero contiene un tablero bajo retención legal, el equipo se marcará como preservado en la página de equipos eliminados y su eliminación permanente se desactivará hasta que se libere la retención legal.
- **Perspectiva del administrador y eDiscovery:** Aunque los usuarios finales no pueden acceder ni recuperar un tablero eliminado que está en espera, los administradores y los equipos de eDiscovery aún pueden interactuar con él. El tablero se conserva hasta que el caso legal se cierre, momento en el cual se puede levantar la retención legal y el tablero puede ser eliminado de forma permanente.
- **Funcionalidad de exportación del tablero:** Los tableros bajo retención legal aún pueden ser exportados utilizando la funcionalidad de exportación del tablero, lo que permite una fácil recopilación de datos relevantes para casos legales.
- **Mover tableros:** Los tableros bajo retención legal no pueden moverse fuera de la organización. Si un tablero está bajo retención legal, los equipos externos se filtran automáticamente de la lista de equipos a los que se puede mover el tablero.
