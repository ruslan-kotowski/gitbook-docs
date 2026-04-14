---
title: "Grupos de facturaci\xF3n"
article_id: 6574185673874
translation_id: 6574185673874
locale: es
sidebar_position: 1
created_at: '2022-07-12T12:53:45Z'
updated_at: '2026-02-19T10:50:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: billing-groups
---

Los grupos de facturación permiten que los admins de empresa puedan mapear usuarios para presupuestos internos. Dado que cada usuario puede ser asignado a solo un grupo, los admins pueden rastrear fácilmente el número de licencias utilizadas por cada centro de costo. Los admins también pueden establecer una cuota flexible para las licencias disponibles para cada grupo de facturación. Esto simplifica procesos como ajustes de licencias, renovaciones y asignaciones de costos para los equipos.

> **Disponible para:** Plan Enterprise
> **Quién puede hacerlo:** Admins de empresa

## Configuración de grupo de facturación

La configuración de tu grupo de facturación muestra una visión general completa del uso de licencias. Por ejemplo, detalles de todos los grupos de facturación existentes, incluyendo el conteo de usuarios, la cantidad de cada tipo de licencias, y si está asignada, la [cuota flexible](02-billing-groups-soft-quotas.md) de licencias asignadas por grupo. Usa el campo de búsqueda para encontrar rápidamente un grupo de facturación.

### Dónde encontrar tus grupos de facturación

Para encontrar tu configuración de grupo de facturación, ve a **Company** **settings** > **Subscription** > **Billing groups.**

:::note
Los usuarios que no están asignados a un grupo de facturación son colocados automáticamente en el grupo de facturación predeterminado de la empresa. Puedes ver la cantidad de usuarios activos asignados en el banner de la parte superior de la configuración de tu grupo de facturación.
:::

## Cómo crear un grupo de facturación

1. Ve a **Configuración** **de la empresa** > **Suscripción** > **Grupos de facturación**.
2. Haz clic **en Crear un grupo de facturación**.
3. Añade el nombre del grupo de facturación.
4. (Opcional) Para establecer una cuota flexible en las licencias asignadas a este grupo de facturación, selecciona **Añadir cuota para licencias Estándar** o **Añadir cuota para licencias Avanzadas**, e ingresa un número.
   Para aprender más sobre las cuotas flexibles, consulta las preguntas frecuentes al final de este artículo.
5. Para añadir nuevos usuarios al grupo de facturación, puedes cargar un archivo CSV con la lista de direcciones de correo electrónico de los usuarios, o asignar usuarios más tarde.
6. (Opcional) Asigna un contacto para el grupo de facturación. Se podrá contactar al contacto para obtener información sobre el uso de licencias.
7. Haz clic en **Crear grupo de facturación**.

## Cómo editar un grupo de facturación

Puedes editar el nombre de un grupo de facturación, establecer o actualizar una cuota flexible, cambiar el contacto del grupo de facturación y añadir usuarios al grupo de facturación.

:::note
Al agregar usuarios a un nuevo grupo de facturación, se transfieren automáticamente de su grupo anterior.
:::

1. Ve a **Configuración de la compañía** > **Suscripción** > **Grupos de facturación**.
2. Haz clic en los tres puntos junto a un grupo de facturación y elige **Editar**.
3. Edita cualquiera de las propiedades del grupo de facturación. Para agregar usuarios al grupo de facturación, carga un archivo CSV con la lista de correos electrónicos de los usuarios, o asigna usuarios más tarde.
4. Haz clic en **Guardar**.

## Cómo eliminar un grupo de facturación

1. Ve a **Configuración de la empresa** > **Suscripción** > **Grupos de facturación**.
2. Haz clic en los tres puntos junto a un grupo de facturación y elige **Eliminar**.
3. Confirma la eliminación.
4. Todos los usuarios que estuvieron en este grupo de facturación serán asignados nuevamente a la cuenta principal y ya no formarán parte de ningún grupo de facturación.

## Cómo asignar un usuario a un grupo de facturación

Un usuario puede ser miembro de un solo grupo de facturación dentro de la organización.

1. Ve a **la configuración de la empresa** > **Usuarios activos**.
2. Haz clic en los tres puntos que se encuentran junto al usuario.
3. Elige **Cambiar grupo de facturación**.
4. Selecciona un grupo de facturación y haz clic en **Asignar usuario**. El usuario se agregará al nuevo grupo de facturación.

## Cómo asignar usuarios de forma masiva a un grupo de facturación

Asigna varios usuarios en simultáneo a un grupo de facturación.

1. Ve a **configuración de la empresa** > **Usuarios activos**.
2. Selecciona usuarios manualmente o aplica filtros y selecciona hasta 50 usuarios al mismo tiempo.
3. Haz clic en **Acciones en masa** y selecciona **Asignar grupo de facturación**.
4. Elige un grupo y haz clic en **Asignar usuarios**. Si algunos usuarios ya son miembros de otros grupos de facturación, podrás anular la selección o cambiar la asignación de su grupo de facturación.

## Cómo verificar qué usuarios están en un grupo de facturación

Comprueba quién está en un grupo de facturación para gestionar el acceso de usuarios y la facturación de manera más eficaz.

1. Ve a **Configuración de la empresa** > **Suscripción** > **Grupos de facturación**.
2. Haz clic en un grupo de facturación específico para ver los usuarios asignados a él.

## Cómo eliminar un usuario de un grupo de facturación

Si un usuario no está asignado a un grupo de facturación específico o es eliminado de uno, automáticamente pasa a formar parte del grupo de facturación estándar de la cuenta de la empresa.

1. Ve a **configuración de la empresa** > **Usuarios activos**.
2. Haz clic en los tres puntos que se encuentran junto al usuario.
3. Elige **Cambiar grupo de facturación**.
4. Selecciona **Grupo de facturación de cuenta predeterminado**. El usuario se eliminará del grupo de facturación y permanecerá en el grupo de facturación general de la empresa.

## Cómo asignar usuarios a un grupo de facturación mediante un archivo CSV

Asigna varios usuarios a un grupo de facturación cargando un archivo CSV con correos electrónicos de los usuarios. Si un usuario ya forma parte de otro grupo de facturación, pasa al grupo de facturación recién asignado.

:::note
Asegúrate de que tu archivo CSV tenga solo una columna con el encabezado "correo electrónico". Esta columna debe incluir la lista de correos electrónicos que se agregarán al grupo de facturación. Comprueba que el CSV use comas para separar los valores. La información en columnas adicionales no se procesará. Miro no guarda los archivos CSV.
:::

1. Ve a **Configuración de la empresa** > **Suscripción** > **Grupos de facturación**.
2. Haz clic en los tres puntos junto a un grupo de facturación y elige **Editar**.
3. Carga un archivo CSV con la lista de direcciones de correo electrónico de los usuarios.
4. Haz clic en **Guardar**.

## Cómo asignar usuarios a un grupo de facturación mediante SCIM

Configura [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) para asignar automáticamente a los usuarios a un grupo de facturación según un centro de costos.

#### Paso 1: Configura tu Proveedor de Identidad (IdP)

Asegúrate de que tu IdP esté configurado para agregar el centro de costos a Miro. Consulta las guías para:

- [Configurar la provisión automatizada con OKTA](../../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md)
- [Configurar la provisión automatizada con Azure AD](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)

#### Paso 2: Asigna centros de costos a tu grupo de facturación

Añade uno o más centros de costo a un grupo de facturación. Todos los usuarios presentes y futuros de estos centros de costo se unirán automáticamente al grupo de facturación.

**Cómo añadir un centro de costo**

1. Abre la página de **Editar grupo de facturación**.
2. Introduce tu centro de costo en el campo **Insertar centro de costo**.
3. Presiona **Intro** en tu teclado.
4. Añade cualquier centro de costo adicional según sea necesario.
5. Haz clic en **Guardar**.

:::note
*Miro no verifica la información del centro de costos que ingresas. Asegúrate de ingresar información precisa para los nombres de los centros de costos. Este campo no distingue entre mayúsculas y minúsculas.*
:::

### Etiqueta de Administrado por SCIM

Los usuarios con un centro de costo asignado y vinculado a un grupo de facturación están etiquetados como **Administrado por SCIM**. Verás esta etiqueta junto al nombre del usuario.

Estos usuarios no pueden ser añadidos manualmente a grupos de facturación y solo pueden ser asignados a un centro de costo a través de una actualización SCIM.

### Lineamientos para el centro de costo y grupos de facturación

- Un grupo de facturación puede contener varios centros de costo, pero un único centro de costo puede estar vinculado a solo un grupo de facturación.
- Para reasignar un centro de costo, primero necesitas eliminar el centro de costo de su grupo de facturación actual.
- Los usuarios que están asignados a un grupo de facturación en función de su centro de costo no pueden ser asignados manualmente a otro grupo de facturación.
- Eliminar un centro de costo de tu grupo de facturación también eliminará a todos los usuarios provisionados por SCIM de ese grupo de facturación.
- Los usuarios no provisionados por SCIM pueden ser asignados manualmente a cualquier grupo de facturación.

### Cómo eliminar un centro de costo de un grupo de facturación

1. Abre la página de **Editar grupo de facturación**.
2. Haz clic en la **X** junto al centro de costos que deseas eliminar.
3. Haz clic en **Guardar**.

## Cómo exportar datos del grupo de facturación

Los admins de empresa pueden exportar un archivo CSV con la lista de usuarios en Configuración de la **empresa** > **Usuarios activos**. Luego puedes usar el atributo de grupos de facturación en la hoja de cálculo CSV exportada para filtrar presupuestos.

## Preguntas frecuentes

¿Qué sucede cuando mis usuarios cambian de centro de costo en el proveedor de identidad (IdP)?

Después de una actualización SCIM:

- si este nuevo centro de costo está asignado a un grupo de facturación, el usuario será trasladado automáticamente a este nuevo grupo de facturación.
- si este nuevo centro de costo no está asignado a un grupo de facturación o el centro de costo fue removido del usuario en IdP, el usuario será trasladado automáticamente al grupo de facturación predeterminado de la empresa.

¿Qué pasa con los usuarios que fueron asignados manualmente a un grupo de facturación después de implementar SCIM para grupos de facturación?

Son reasignados automáticamente a un nuevo grupo de facturación según su centro de costo, mientras que aquellos sin un centro de costo correspondiente o alguno permanecen en su grupo de facturación actual.

¿Por qué ya no puedo asignar manualmente a un usuario a los grupos de facturación?

Los usuarios asignados a un grupo de facturación a través de su centro de costo SCIM no pueden ser movidos manualmente a otro grupo.

¿Qué sucede si mi IdP deja de sincronizar el atributo del centro de costos con Miro?

Los nuevos usuarios no se asignarán automáticamente a un grupo de facturación sin centros de costos sincronizados, pero pueden ser asignados manualmente hasta que se reanude la sincronización.

¿Qué es una cuota flexible de grupo de facturación?

Una cuota flexible te permite opcionalmente establecer un límite en las licencias Avanzadas, Estándar o Completas (heredadas) disponibles para un grupo de facturación.

Cuando creas o editas un grupo de facturación, puedes habilitar **Añadir cuota para licencias Estándar** o **Añadir cuota para licencias Avanzadas** e ingresar un número.

La cuota flexible aparece, como el número que estableciste y una barra de progreso que indica el consumo, en la parte superior de la vista general del grupo de facturación.

Para obtener más información sobre las cuotas flexibles, consulta [Cuotas flexibles para grupos de facturación](02-billing-groups-soft-quotas.md).
