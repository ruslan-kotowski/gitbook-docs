---
title: "Posibles problemas con la aplicaci\xF3n de Miro para Confluence"
article_id: 360021388500
translation_id: 8637531357970
locale: es
sidebar_position: 21
created_at: '2022-11-18T11:21:39Z'
updated_at: '2025-02-26T11:23:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
---

Usa los consejos para resolución de problemas a continuación si tienes dificultades al usar el [plugin de Confluence](https://help.miro.com/hc/articles/360020712594).

|  |  |  |
| --- | --- | --- |
| **Mensaje/incidencia** | **Posibles causas** | **Pasos para resolver el problema** |
| Tienes un selector de Miro en negro/en blanco cuando inicias sesión en Miro/insertar tableros de Miro en las páginas de Confluence. | Ajustes incorrectos del navegador | Ve a los ajustes de tu navegador y comprueba lo siguiente:   - La casilla de verificación **Prevent cross-site tracking** (Impedir seguimiento entre sitios) está deshabilitada. - La casilla de verificación **Block all cookies** (Bloquear todas las cookies) está deshabilitada:   mceclip0.png   - **Pop-up windows** (Ventanas emergentes) en los sitios web de Miro y de Atlassian está permitido:   mceclip1.png |
| Solo tienes permiso de visualización para este tablero y no puedes compartirlo o insertarlo.  **altmceclip0.png** | No eres editor/propietario del tablero. | Asegúrate de:   - Ser editor o propietario del tablero. - Tener autorización en el navegador en Miro con las credenciales correctas. - Insertar un tablero en Confluence en el mismo navegador |
| Después de insertar un tablero de Miro verás el mensaje: "Miro necesita acceder a tus archivos cookie" | Tu navegador no permite guardar cookies de terceros. | Para habilitar la inserción, tienes que habilitar las cookies en tu navegador. Esto sucede mayormente en Mozilla y Safari. |
| En el tablero insertado se muestra el mensaje de error “Your session has expired” (Tu sesión expiró). |
| Cuando intentas insertar un tablero, recibes el siguiente mensaje: "No eres miembro de ningún equipo. Please log in to the full version of the product and create your team or let someone invite you to the existing one.” (No eres miembro de ningún equipo. Inicia sesión en la versión completa del producto y crea tu equipo o deja que alguien te invite al existente).  mceclip0.png | No eres miembro de ningún equipo con el perfil de Miro autorizado en el navegador. | Ve a [Miro](https://miro.com/app/dashboard/) y crea un equipo. Si sabes que deberías ser miembro de algún equipo en Miro, abre Miro en otra pestaña de navegador y asegúrate de tener autorización con el **correo electrónico correcto**. |
