---
title: 'Historial de tablero: versiones'
article_id: 360021668819
translation_id: 360021668819
locale: es
sidebar_position: 12
created_at: '2021-05-17T11:56:55Z'
updated_at: '2026-01-06T19:02:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: activity-list
availability:
  notes: 'Quién puede hacerlo: Propietarios de tableros, copropietarios, editores
    de tableros que son miembros del equipo donde se encuentra el tablero si están
    autorizados a copiar el contenido del tablero
    Cuáles planes: Starter, Business, Enterprise, Education Cuáles plataformas: Navegador,
    escritorio, aplicación para tabletas'
---

Todas las versiones de tus tableros de Miro se guardan automáticamente en el historial de tu tablero. Puedes revisar y recuperar los cambios en cualquier momento.

### Funciones principales

- Se realiza una copia de seguridad a los tableros cada hora si se hizo algún cambio y al final de cada sesión de colaboración.
- Las versiones guardadas del historial del tablero se almacenan durante *90 días*
- El tablero original *no* se cambia. La versión restaurada se crea como un tablero *separado* y su título se fecha por defecto

:::warning
Ocasionalmente, problemas imprevistos de red pueden impedir que un tablero realice una copia de seguridad. Asegúrate de tener una conexión a Internet estable para realizar copias de seguridad consistentes.
:::

### Restaurar una versión anterior de un tablero

Realiza lo siguiente para restaurar una versión anterior:

1. En la barra de Tablero, selecciona los **tres puntos** verticales.
   El **menú principal** se abre.
2. Selecciona **Tablero**>**Historial**.
   El panel de **Historial** se abre. La pestaña de **Actividad** está abierta por defecto.
3. Selecciona **Versiones**.
4. Selecciona una versión.
   El modal de **Restaurar como un tablero separado** se abre.
5. (Opcional) Sigue las instrucciones en pantalla.
6. Selecciona **Restaurar**.

### Limitar o deshabilitar la restauración de versiones anteriores del tablero

- La función está disponible para [propietarios de tableros](../sharing-boards/01-board-access-rights.md), copropietarios, y se puede habilitar para [editores](../sharing-boards/01-board-access-rights.md) que sean miembros del equipo donde está ubicado el tablero
- La función depende de la [configuración del contenido del tablero](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md): la opción está disponible para los miembros del equipo solo si el propietario del tablero permite a los miembros del equipo copiar el contenido del tablero. Esto se puede configurar en el tablero **Compartir** > **Ajustes de uso compartido** > **Permisos**
- [Permisos de admin de contenido](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md) en el [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md): cuando está habilitado, permite a los admins de empresa acceder a las **Versiones** del tablero incluso cuando están deshabilitadas por la configuración de contenido mediante [reasignación de la propiedad del tablero a sí mismos](../sharing-boards/01-board-access-rights.md)

Si no tienes permiso para usar la opción, verás el mensaje correspondiente en la pestaña **Versiones**. Comunícate con el propietario del tablero para habilitar la función.

## Preguntas frecuentes

**Recientemente he [mejorado mi plan](../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md). ¿Puedo restaurar una versión de tablero que se creó cuando mi equipo estaba en el plan Free?**

Sí, después de mejorar tu plan puedes restaurar versiones creadas cuando estabas en un plan Free.

**No tengo versiones en el historial del tablero. ¿Por qué?**

Ten en cuenta que la función no es compatible con [equipos Free](../../plans-billing/miro-plans/09-free-plan.md). Además, asegúrate de que tu rol en el tablero te permita restaurar versiones (deberías ser el [propietario del tablero](../sharing-boards/01-board-access-rights.md), [copropietario](../sharing-boards/06-co-owners-of-boards-and-spaces.md) o [editor](../sharing-boards/01-board-access-rights.md) y ser miembro del equipo en el cual está ubicado el tablero). Además, el propietario/copropietario del tablero debería permitir a los miembros del equipo copiar el contenido del tablero.
Si eliminaste un objeto, también puedes restaurarlo: consulta [esta guía](../working-on-the-board/18-restoring-board-content.md).
