---
title: Conector Netskope para Miro Enterprise
article_id: 4415711060498
translation_id: 4415711060498
locale: es
sidebar_position: 6
created_at: '2022-01-19T06:23:42Z'
updated_at: '2025-02-26T11:27:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

El conector personalizado de Miro para Netskope permite visualizar eventos relacionados con filtraciones de datos y administrar el siguiente tráfico dentro de Miro:

- [Descargar copia de seguridad del tablero](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)

Esta guía proporciona pasos para configurar Netskope para el plan Enterprise de Miro y describe la experiencia del usuario.

> **Disponible para: [Plan Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md)**

### Crea una nueva aplicación de Miro en Netskope

Dentro de tu instancia de Netskope ve a **Settings (ajustes) > Security Cloud Platform (plataforma de seguridad en la nube) > App Definition (definición de aplicaciones)** y haz clic en **NEW CLOUD APP (nueva aplicación en la nube)**:

nueva_aplicación_en_la_nube.jpg
![Cómo crear una aplicación de nube en Netskope](blob:https://miro.atlassian.net/8cb061a4-e184-4bd6-bb95-774cd34fc8e7#media-blob-url=true&id=78b7a8cb-792a-41da-bf16-b26ca4480059&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.08.43.png&size=181298&height=513&width=1028&alt=)

Para crear una nueva aplicación dentro de Netskope, se te pedirá que importes el siguiente archivo de JSON **miro-activities-for-netskope.json**:

```
Versión: 0.0.0.1.

"nombre_dominio": "miro.com",
"uri_path": "/api/v1/ tableros/.+/",
"http_method": CONSEGUIR
"uri_param": [{ "clave": "archivo", "valor": "verdadero" }],
"resp_code": 200.
"patrón": "",
"nombre_actividad": descargar


"nombre_dominio": "miro.com",
"uri_path": "/api/v1/tableros/.+/recursos/.+/ficheros/originales",
"http_method": CONSEGUIR
"uri_param": [],
"resp_code": 307.
"patrón": "",
"nombre_actividad": descargar
```

Ingresa el nombre de la aplicación, selecciona la opción **Custom Connector (conector personalizado)** y haz clic en **IMPORT FROM FILE (importar desde archivo) > Add To Activity List (añadir a la lista de actividades)** para cargar el archivo **miro-activities-for-netskope.json** del paso anterior**.**

cargar_el_archivo.jpg
Cómo cargar el archivo

Después de importar el archivo **miro-activities-for-netskope.json** se mostrarán las actividades grabadas. Ahora puedes hacer clic en **SAVE (guardar)** y crear la aplicación de Miro.

save_the_app.jpg
![Cómo guardar la aplicación](blob:https://miro.atlassian.net/b9da4e19-b3b1-4c25-aed3-762f458fd639#media-blob-url=true&id=f7549007-0265-42e1-b946-a3e167124f12&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.26.58.png&size=209044&height=693&width=1028&alt=)

Una vez que se haya creado la aplicación, tienes que seleccionarla y hacer clic en **APPLY CHANGES (aplicar cambios).**

apply_changes.jpg
/strong>La opción de aplicar cambios a la aplicación de Miro

![](blob:https://miro.atlassian.net/82b8ac6e-1952-44e7-a62f-cefb7dbee6ab#media-blob-url=true&id=975f42e8-de5d-4bbb-ae07-c243cce9bb2f&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.32.06.png&size=257154&height=575&width=1780&alt=)

### Crea una nueva Política para tu aplicación de Miro en Netskope

Una vez que se haya creado la aplicación, puedes proceder a crear una política. Para eso, puedes navegar hasta **Policy (política) >** **Real-time Protection (protección en tiempo real)** y hacer clic en **NEW POLICY (nueva política) > Cloud App Access (acceso a aplicaciones en la nube).**

create_a_policy.jpg
![Cómo crear una política para tu aplicación de Miro](blob:https://miro.atlassian.net/d2ae8479-8f5c-4417-8b09-2b57ee344d90#media-blob-url=true&id=e9c82ee5-cdea-4b33-8491-9613a848be81&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.39.02.png&size=107320&height=321&width=635&alt=)

Aquí, en **Destination (destino)**, necesitas proporcionar la aplicación de Miro que creaste en el paso anterior, configurar un **Policy Name (nombre de política)** y hacer clic en **SAVE (guardar).**

save_the_policy.jpg
/strong>Cómo guardar la política

![](blob:https://miro.atlassian.net/abf26593-27ad-40f4-b3e5-731a9e58d062#media-blob-url=true&id=0edd2e23-2762-4173-8f3f-9a7bb74bf217&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.45.14.png&size=200430&height=722&width=1575&alt=)altA continuación, puedes seleccionar dónde prefieres colocar la política y hacer clic en altSAVE (guardar).

mover_política.jpg
Cómo seleccionar dónde prefieres colocar la política

Finalmente, puedes aplicar los cambios haciendo clic en el botón **APPLY CHANGES (aplicar cambios)**

applying_changes.jpg
Cómo aplicar cambios

![](blob:https://miro.atlassian.net/41cdf802-aa1c-4f9a-bd22-950ea6ad755e#media-blob-url=true&id=7f85d987-6550-4271-90da-c9273a0cbc9a&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2019.29.17.png&size=157218&height=490&width=1576&alt=)

### Visualización de eventos

Una vez hecho todo lo anterior, podrás visualizar el tráfico navegando a **Skope IT**, filtrando por la aplicación Miro personalizada y haciendo clic en **See Events (ver eventos)** de la siguiente manera.

ver_eventos.jpg
La opción de ver eventos de tráfico

### Experiencia del usuario

Los usuarios para quienes deban bloquearse las actividades de Descarga deben tener el cliente de Netskope instalado en su máquina.  Cuando los usuarios intentan realizar una operación de copia de seguridad de Descarga, Netskope bloquea la acción y muestra una ventana emergente de su SO nativo con un mensaje.

alerta.jpg
Un mensaje que se muestra a usuarios que no están autorizados para descargar una copia de seguridad de un tablero de Miro
