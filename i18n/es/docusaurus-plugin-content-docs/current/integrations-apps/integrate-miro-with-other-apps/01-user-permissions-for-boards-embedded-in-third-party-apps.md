---
title: Permisos de usuario para tableros insertados en apps de terceros
article_id: 4411883577618
translation_id: 4411883577618
locale: es
sidebar_position: 1
created_at: '2021-12-08T10:13:42Z'
updated_at: '2025-11-25T16:07:55Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Personas: Propietarios de tableros, copropietarios de tableros Planes: Todos
    los planes Plataformas: Navegador, aplicación de escritorio'
---

Miro ofrece varias integraciones que te permiten colaborar fácilmente con tableros en entornos de terceros, como [Microsoft Teams](../microsoft), [Confluence](../atlassian/01-miro-for-confluence.md), Notion y Google Meet. Puedes descubrir otras aplicaciones compatibles en el [Marketplace de Miro](https://miro.com/marketplace/category/embed-miro/). Al insertar tableros, puedes establecer diferentes niveles de acceso de usuario y gestionar estos permisos desde Miro.

## Comprender el acceso de inserción

Cuando compartes un tablero en una app externa, puedes proporcionar acceso para ver, comentar o editar específicamente a usuarios dentro de esa app para una única colaboración, independientemente de su acceso a Miro. Estos usuarios no necesitarán tener un perfil de Miro para acceder al tablero dentro de la aplicación. Esto te permite establecer ciertos derechos de acceso al tablero para los usuarios de la aplicación que no estén registrados en Miro sin necesidad de hacer que el tablero esté disponible públicamente.

Para una seguridad máxima, desaconsejamos utilizar este método fuera de colaboraciones puntuales (como un taller) y recomendamos que tu organización asigne el acceso a Miro de forma adecuada a quienes lo requieran.

![embed_Miro_in_Zoom.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020254296722_embed%20Miro%20in%20Zoom.gif) *Configuración de derechos de acceso de una inserción de tablero*

El tablero se vuelve accesible solo dentro de la aplicación en la que se insertó. El nivel de acceso que configuraste para un tablero insertado en la aplicación no afecta la configuración de uso compartido del tablero fuera de la aplicación. Por ejemplo, si un [tablero privado](../../using-miro/sharing-boards/15-make-a-miro-board-private.md) se inserta en un canal de Microsoft Teams con acceso de "Cualquiera puede ver", los usuarios en ese canal de Microsoft Teams pueden ver el tablero sin iniciar sesión en Miro. Si los mismos usuarios intentan acceder al tablero fuera del canal de Microsoft Teams siguiendo el enlace del tablero, no tendrán acceso.

Sin embargo, la configuración de uso compartido en Miro tiene prioridad sobre el nivel de acceso establecido en la aplicación externa. Por ejemplo, si un tablero se [comparte públicamente en el lado de Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), estará disponible para cualquier persona en Microsoft Teams, incluso si insertaste el tablero como Privado.

## Administrar y revocar el acceso de inserción

Puedes rastrear, administrar y revocar fácilmente el acceso a tableros insertados en aplicaciones externas compatibles.

Para administrar y revocar el acceso a tableros insertados:

1. Haz clic en el botón **Compartir** para abrir la configuración de uso compartido de un tablero de Miro.
2. Selecciona **Configuración de uso compartido**.
3. Abre la pestaña **Inserciones**.
4. Verás las aplicaciones externas donde se inserta el tablero, incluyendo el nombre de la integración, cuándo y por quién se insertó, y la configuración de acceso al tablero dentro de la aplicación.
5. Para revocar el acceso al tablero dentro de una aplicación, haz clic en **Revocar acceso** junto a la aplicación. Ten en cuenta que esta acción es irreversible.

ol

![remove_an_access_link.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020265344914_remove%20an%20access%20link.gif)
*Cómo eliminar un enlace de acceso*

Después de revocar el acceso insertado, el acceso al tablero estará limitado en la aplicación. Ten en cuenta que es posible que el tablero aún esté accesible dentro de la aplicación si se comparte en Miro. Por ejemplo:

- Si cualquiera pudiera **editar** el tablero dentro de la aplicación y el mismo tablero se [compartiera públicamente](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) para **ver** desde el lado de Miro, entonces cualquiera podría **ver** el tablero dentro de la aplicación.
- Si el tablero es privado y solo se comparte [con otros usuarios mediante correo electrónico](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), se requerirá **inicio de sesión** para acceder al tablero insertado dentro de la aplicación.

## Reglas y limitaciones de inserción

Ten en cuenta las siguientes reglas y limitaciones al insertar tableros:

- No puedes insertar un tablero si está [inactivo](../../using-miro/tools/troubleshooting/15-the-board-is-locked.md) o si solo tienes acceso para ver el tablero.
- Los tableros guardados en [equipos gratuitos](../../plans-billing/miro-plans/09-free-plan.md) no se pueden insertar con acceso a comentarios.
- Para los usuarios del [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), tu configuración de acceso respetará los controles de acceso de toda la organización, lo que podría implicar que algunas opciones para compartir estén restringidas. Más información: [Gestionar la política de uso compartido del plan Enterprise para integraciones insertadas](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- En el caso de algunos enlaces antiguos, solo verás el nivel de acceso y la aplicación, pero no quién creó el tablero ni cuándo se insertó.
- Si quieres limitar la capacidad de insertar tableros de Miro dentro de aplicaciones externas para tu organización Enterprise, consulta [Gestión de la política de uso compartido del plan Enterprise para integraciones insertadas](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- La gestión de enlaces de acceso a tableros insertados aún no es compatible con dispositivos móviles o tabletas.

Obtén más información sobre [el acceso a tableros insertados para usuarios con licencias gratuitas limitadas](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
