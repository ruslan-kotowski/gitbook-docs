---
title: Equipos de desarrolladores de Enterprise
article_id: 4766759572114
translation_id: 4766759572114
locale: es
sidebar_position: 4
created_at: '2022-03-22T14:13:15Z'
updated_at: '2025-04-29T13:25:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: developer-teams
---

Conoce la opción para configurar equipos de desarrolladores en las suscripciones de Enterprise. Es una manera fácil y segura de crear aplicaciones personalizadas para tu plan Enterprise.

> **Disponible para: [Plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configurado por: admins de empresa
> Los usuarios de otros planes de Miro pueden crear equipos de Programadores desde [esta página](https://developers.miro.com/docs/rest-api-build-your-first-hello-world-app#step-1-create-a-developer-team-in-miro)****

### Cómo crear un equipo de desarrolladores

Para crear un equipo de desarrolladores, abre los ajustes **Empresa** > **Equipos** y haz clic en **Crear equipo nuevo** en la esquina superior derecha.

En la siguiente ventana emergente, ingresa el nombre del equipo y [elige el nivel de permisos de equipo: puedes establecer los ajustes predeterminados de permisos o seleccionar un equipo para copiar los permisos (conoce más sobre](../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)los permisos y los ajustes predeterminados).  Marca la casilla **Equipo de desarrolladores**, confirma tu autorización y haz clic en **Crear equipo**.

![crear-equipo-dev.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803173266_create-dev-team.png)
Cómo crear un equipo de desarrolladores

### Permisos del equipo de desarrolladores en Enterprise

Puedes crear aplicaciones de forma segura en el equipo de desarrolladores de Enterprise, que te proporciona todas las características de seguridad de Enterprise mientras tienes una subscripción a este plan.

El equipo de desarrolladores de Enterprise tiene tableros ilimitados y no hay un límite de miembros.

Los tableros creados en el equipo tendrán una marca de agua para diferenciarlos de otros equipos de la organización.

El equipo tiene todos los ajustes estándar para configurar los permisos de los usuarios en el plan Enterprise: puedes permitir/prohibir que los miembros del equipo inviten a usuarios nuevos, compartir tableros con el equipo o empresa mediante enlace público, mover tableros, restringir los dominios permitidos, etc. Para obtener más información, consulta [este artículo](../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md).

### Cómo crear e instalar aplicaciones

> **Configurado por: admins de equipo
> Si quieres invitar a desarrolladores a crear una app en el equipo, asegúrate de [conceder permisos de admin de equipo](../../administration/user-management/06-how-to-manage-admin-roles.md)**

[Para crear una aplicación nueva en Miro Enterprise mediante el equipo de desarrolladores de Enterprise, ve a los](../../using-miro/managing-your-profile/01-profile-settings.md) ****Ajustes del perfil** > Tus aplicaciones****, acepta los términos y condiciones, y haz clic en** Crear una nueva aplicación.

![perfil-crear-nueva-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780634770_profile-create-new-app.png)
Tus aplicaciones en los ajustes de perfil

:::tip
También puedes ir a la página haciendo clic en **Crear una app** en la esquina superior derecha del panel del equipo de desarrolladores.
:::

![dev-team-build-an-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780641298_dev-team-build-an-app.png)
La opción para crear aplicaciones nuevas y personalizadas

**Ingresa el nombre de la aplicación, selecciona el equipo de desarrolladores y haz clic en** Create app (crear aplicación).

create_a_new_app.jpg
Cómo crear una aplicación nueva para el equipo de desarrolladores de Enterprise

**En la página de la aplicación, desplázate hacia abajo y selecciona el alcance del acceso que deseas otorgar a la aplicación y, luego, haz clic en** Install app and get OAuth token (instalar aplicación y obtener el token de OAuth).

permisos_app.jpg
Permisos de la aplicación

Cuando instales la aplicación, selecciona un equipo (diferente del equipo de desarrolladores) de la organización de Enterprise y haz clic en **Install & authorize (instalar y autorizar)**. En el siguiente paso se mostrará el token de acceso.

instalar_la_app.jpg
Instalar la aplicación

### Cómo eliminar un equipo de desarrolladores

Puedes eliminar el equipo de desarrolladores como lo harías con cualquier otro equipo de tu organización de Enterprise, pero primero debes eliminar todas las aplicaciones que se hayan creado en ese equipo. Una vez eliminadas las apps, ve a [**Equipos**](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md)haz clic en el nombre del equipo, selecciona la pestaña **Perfil** y, a continuación, **Eliminar equipo**.

:::warning
Ten en cuenta que, una vez que elimines el equipo de desarrolladores de Enterprise, todos los tokens asociados con él dejarán de ser válidos.
:::

![borrar-equipo-desarrollador.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803181586_delete-dev-team.png)*Eliminar el equipo de desarrolladores de empresas*
