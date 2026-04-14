---
title: Conectar a Jira usando OAuth 1.0 (Actualizado)
article_id: 27689156602514
translation_id: 27689221618834
locale: es
sidebar_position: 12
created_at: '2025-06-27T13:20:37Z'
updated_at: '2025-11-25T15:52:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quién puede hacerlo: Administradores de empresa, administradores de equipo
    Para qué planes: Starter, Business, Enterprise, Education Para qué plataformas:
    Navegador, Escritorio'
---

Las organizaciones que no están listas para migrar a OAuth 2.0 pueden usar el siguiente procedimiento para conectar Miro a Jira usando OAuth 1.0.

Atlassian ha [obsoleto OAuth 1.0](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively), y el método proporcionado en este artículo es una solución provisional. Para evitar incidencias y alinearse con las mejores prácticas de seguridad y compatibilidad, Miro recomienda encarecidamente migrar a OAuth 2.0 lo antes posible.

:::note
El método de autenticación anterior de OAuth 1.0 [está obsoleto](https://help.miro.com/hc/articles/360019501754-Set-up-and-disable-Jira-Cards-OAuth-1-0) y será eliminado el 31 de julio de 2025.
:::

Este artículo también explica cómo utilizar una sola instancia de Jira para varios equipos de Miro, y cómo deshabilitar las tarjetas de Jira a nivel de organización y equipo.

## Requisitos previos

- Asegúrate de tener los siguientes permisos:
  - (Business, Enterprise) admin de empresa de Miro
    (Starter, Education) admin de equipo de Miro
  - Administrador del sistema de Jira

    > ✏️ Para completar el procedimiento, debes poder crear un enlace de aplicación en Jira.
- En Jira, elimina cualquier enlace de aplicación existente a Miro.

## Procedimiento

Para conectarte a Jira usando OAuth1.0, sigue estos pasos:

1. Desde tu panel de Miro, selecciona tu avatar en la parte superior derecha y haz clic en **Consola del administrador**.
2. En la barra lateral izquierda, ve a **Aplicaciones e integraciones** > **Aplicaciones** > pestaña **Gestionar aplicaciones**.
3. Asegúrate de que **Permitir solo aplicaciones de la lista a continuación** esté habilitado.
4. En la columna **Aplicación**, para **Tarjetas de Jira** selecciona **Configuración**.
5. En la pestaña **Configuración predeterminada**, selecciona **Añadir nueva conexión**.
6. Bajo **Configuración de Jira**, selecciona ya sea **Jira Cloud** o **Jira Data Center**.
7. En **Método de autenticación**, selecciona **OAuth 1.0x (Actualizado)**.
8. En **URL de Jira**, introduce la URL de tu instancia de Jira.
9. (Opcional) Para hacer de esta conexión la conexión predeterminada para todos los equipos de tu organización, marca **Establecer como predeterminada**.
10. En **Instrucciones de configuración**, verifica que tengas las siguientes propiedades:
    - URL
    - Clave del consumidor
    - Nombre del consumidor
    - Clave pública
11. En Jira, crea un enlace de la aplicación.
    1. (Cloud) Ve a **Configuración** > **Productos** > **Enlaces de Aplicación**.
       (Data Center) En la configuración de administración de Jira ve a **Productos** > **Enlaces de Aplicación**.
    2. Haz clic en **Crear enlace**.
    3. (Cloud) Para **Tipo de aplicación**, selecciona **Aplicación directa**.
       (Data Center) Para **Tipo de aplicación**, selecciona **Producto de Atlassian**.
    4. Para **URL de la aplicación**, pega la URL de las instrucciones de configuración de Miro. Ver paso 10.
    5. Haz clic en **Continuar**.
    6. Para **nombre de la aplicación**, nombra tu aplicación.

       > **⚠️** No ingreses datos en ningún otro campo. Proporcionarás datos de Miro en un paso siguiente.
    7. Marca **Crear enlace entrante**.
    8. Haz clic en **Continuar**.
    9. Copia y pega tu clave del consumidor, nombre del consumidor y clave pública desde las instrucciones de configuración de Miro. Ver paso 10.
    10. Haz clic en **Continuar**.
        Has creado tu enlace de la aplicación.
12. En Miro, haz clic en **Conectar**.
    Has conectado Miro a Jira usando OAuth 1.0.

## ¿Qué sigue?

Has configurado y conectado tu integración de Jira con Miro utilizando Jira OAuth1.0. Cuando un usuario intenta realizar una acción relacionada con Jira en Miro por primera vez, se le solicita autenticarse.

**Más información:** Consulta [Cómo usar tarjetas de Jira](https://help.miro.com/hc/articles/360017572434).

## Una instancia de Jira para varios equipos de Miro

Puedes instalar tarjetas de Jira a nivel de organización, o a nivel de equipo. Si tienes múltiples equipos, puedes especificar configuraciones a nivel de organización para evitar configuraciones repetitivas para cada equipo. El enlace de la aplicación existente se usará para todos los equipos.

:::note
No es posible conectar varias instancias de Jira a un equipo de Miro.
:::

Para las solicitudes de actualización, después de conectar tu organización o equipo a una instancia de Jira, se añade un webhook a los webhooks de Jira para esa organización o equipo de Miro.

:::tip
Asigna un nombre único a cada webhook por equipo. Ve a tu página de webhooks de Jira y edita cada webhook recién creado.
:::

Si especificas configuración a nivel de la organización, los equipos que ya tienen su propia configuración de equipo mantienen su configuración. Cualquier equipo con su propia configuración puede cambiar a la configuración de nivel organizativo en cualquier momento.

Por el contrario, cualquier equipo puede anular la configuración a nivel organizativo para conectarse a una instancia separada de Jira.

## Deshabilitar tarjetas de Jira

### A nivel de organización

Para deshabilitar las tarjetas de Jira a nivel de organización, sigue estos pasos:

1. Desde el panel de Miro, haz clic en tu avatar en la esquina superior derecha y selecciona **Consola de administración**.
2. Ve a **Aplicaciones e Integraciones** > **Gestionar aplicaciones**.
3. Ubica **Tarjetas de Jira**.
4. Para las Tarjetas de Jira, cambia el interruptor de **Permitido** a la posición desactivada.

:::warning
Si deshabilitas las Tarjetas de Jira para la organización, los miembros de todos los equipos Enterprise no podrán usar tarjetas de Jira. Para aprender más sobre la gestión de aplicaciones, consulta [gestión de aplicaciones](https://help.miro.com/hc/articles/4404659741458).
:::

### Nivel de equipo

Para deshabilitar las Tarjetas de Jira a nivel de equipo, sigue estos pasos:

1. Desde tu panel de Miro, haz clic en tu avatar en la esquina superior derecha y haz clic en **Admin Console**.
2. Ve a **Equipos**.
3. Haz clic en la fila del equipo que deseas gestionar.
   Se abrirá el panel de configuración del equipo.
4. Haz clic en la pestaña **Aplicaciones**.
5. Localiza y haz clic en **Jira Cards**.
6. Haz clic en **Eliminar para el equipo**.
