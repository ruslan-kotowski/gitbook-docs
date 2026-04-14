---
title: Tarjetas de Jira
article_id: 360017572434
translation_id: 6634752953490
locale: es
sidebar_position: 5
created_at: '2022-07-15T14:22:55Z'
updated_at: '2025-11-25T15:59:40Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Planes: Starter, Business, Education, Enterprise Usuarios: Todos los usuarios
    Plataformas: Navegador, Escritorio, Móvil Jira: Jira Cloud, Jira Server (en las
    instalaciones), Jira Data Center'
---

Las tarjetas de Jira te permiten trabajar con incidencias de Jira directamente dentro de los tableros de Miro. Esta integración optimiza el flujo de trabajo de tu equipo al traer las incidencias de Jira a tu espacio de trabajo colaborativo, para retrospectivas, dimensionamiento de historias, priorización del backlog, mapeo de historias y otras actividades del equipo.

![Jira cards in user story mapping](../../../../../../docs/integrations-apps/atlassian/images/21017348097170_Jira%20cards%20in%20USM.png)

## Importar incidencias de Jira a tu tablero

Puedes importar incidencias de Jira a tu tablero de dos maneras:

1. Copia la URL de la incidencia de Jira y pégala en el tablero.
2. Haz clic en el icono de **Herramientas, Medios y Integraciones** (**+**) en la barra de herramientas de Creación, selecciona **Tarjetas de Jira**, elige una o más incidencias y haz clic en **Agregar**.

Cuando importes incidencias por primera vez, necesitarás conectar tu cuenta de Jira:

1. Haz clic en **Autorizar** en el cuadro de diálogo que aparece.
2. Inicia sesión en tu cuenta de Jira con tus credenciales.
3. Autoriza la conexión entre Miro y Jira.

Después de autorizar, verás todas las incidencias de Jira a las que tienes acceso en el selector de Tarjetas de Jira.

:::note
Los usuarios que no han autorizado su cuenta de Jira verán una vista de tarjeta simplificada sin los avatares de los asignados.
:::

## Crear nuevas incidencias de Jira

Puedes crear incidencias de Jira directamente desde Miro de dos maneras.

### Crear usando la aplicación de Jira

1. Haz clic en el icono de **Herramientas, Medios e Integraciones** (**+**) en la barra de herramientas de Creación
2. Selecciona **Tarjetas de Jira**.
3. Haz clic en **Crear incidencia**.
4. Completa los campos requeridos.
5. Haz clic en **Crear**.

### Convertir elementos existentes en incidencias de Jira

Puedes convertir notas adhesivas o tarjetas ya existentes en tu tablero a incidencias de Jira.

1. Selecciona hasta 50 notas adhesivas o tarjetas.
2. Haz clic en **Convertir a** > **Jira** en el menú contextual.
3. Configura los valores predeterminados (tipo de incidencia, prioridad, asignado, etc.).
4. Haz clic en **Convertir**.

:::warning
Nota:

- Las tarjetas de la línea USM Tasks no se pueden convertir en incidencias de Jira.
- Durante la conversión, las etiquetas y la fecha de inicio de las tarjetas de Miro no se conservarán.
- Es necesario volver a establecer la información del asignado después de la conversión.
:::

## Ver y editar incidencias de Jira

:::warning
No se admite la edición de tarjetas de Jira en la aplicación de escritorio o móvil.
:::

Puedes ver las tarjetas de Jira de dos maneras:

- Vista lateral
- Vista centrada

### Editar incidencias en Miro

1. Haz clic en el icono **Abrir en panel lateral** o **Abrir en panel central**.
2. Realiza tus cambios.
3. Haz clic en **Actualizar** para guardar.

### Cambiar el estado de la incidencia

1. Haz clic en el icono **Flujo de trabajo**.
2. Selecciona el **Estado** y **Comentario** deseados.
3. Haz clic en **Actualizar** para guardar.

### Editar en Jira

1. Selecciona una tarjeta y haz clic en el icono de **Fuente**.
2. Edita la incidencia en Jira en la nueva pestaña del navegador.
3. Los cambios se sincronizarán automáticamente con la tarjeta de Miro.

## Sincronización entre Miro y Jira

|  |  |
| --- | --- |
| **Actualización en la instancia de Jira vs. Actualización en la tarjeta de Miro** | **¿Cuándo ocurre la actualización?** |
| Actualización en Jira vía OAuth 1.0 y OAuth 2.0 | La tarjeta de Jira en Miro se actualiza inmediatamente vía [webhook](https://help.miro.com/hc/articles/360017731113). |
| Actualización en Miro | La tarjeta de Jira en Miro se actualiza inmediatamente y la incidencia de Jira correspondiente se actualiza simultáneamente. |

## Personaliza las tarjetas de Jira

### Cambiar colores de tarjeta

1. Selecciona una o más tarjetas de Jira.
2. Haz clic en **color de relleno** en el menú de contexto.
3. Elige el color que desees.

### Configurar campos personalizados

1. Haz clic en el icono **Herramientas, Medios e Integraciones** (**+**) de la barra de herramientas de creación.
2. Selecciona **Tarjetas Jira**.
3. Selecciona **Configurar tarjetas**.
4. Selecciona los campos que quieres mostrar.
5. Haz clic en **Guardar**.

:::note
Notas importantes sobre los campos:

- La configuración se aplica solo al tablero actual.
- Los campos predeterminados (Asignado, Tipo de incidencia, Prioridad, Estado) no se pueden eliminar.
- Los campos pueden no aparecer si no tienen valor o no están disponibles para el tipo de incidencia.
- Algunos tipos de campos (como los campos personalizados de color) no son compatibles.
:::

## Buscar incidencias de Jira

El selector de tarjetas de Jira muestra primero las tareas recientes y ofrece varias opciones de clasificación:

- Tipo de incidencia
- Prioridad
- Clave
- Resumen
- Persona asignada
- Estado

Usa palabras clave para encontrar incidencias específicas o usa **Jira Query Language** (JQL) para búsquedas complejas:

1. Selecciona la opción **Búsqueda avanzada** en la barra de búsqueda.
2. Ingresa tu consulta JQL.

Los resultados se actualizarán en función de tu consulta.

## Artículos relacionados

- [FAQ de tarjetas de Jira](https://help.miro.com/hc/articles/360013463739)
- [Configurar e desinstalar tarjetas de Jira](https://help.miro.com/hc/articles/360019501754)
- [Configurar webhooks para tarjetas de Jira](https://help.miro.com/hc/articles/360017731113)
- [Solucionar problemas de tarjetas de Jira](https://help.miro.com/hc/articles/360017572654)
