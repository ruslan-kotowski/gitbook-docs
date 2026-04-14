---
title: "Soluci\xF3n de problemas de dispositivos m\xF3viles y tabletas"
article_id: 360021113559
translation_id: 360021113559
locale: es
sidebar_position: 16
created_at: '2021-04-16T08:25:42Z'
updated_at: '2025-11-25T16:04:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Si encuentras problemas cuando trabajas con Miro en una tableta o dispositivo móvil, lo primero que debes hacer es *reinstalar la aplicación y volver a cargar tu dispositivo*.  Si eso no ayuda, consulta las posibles razones a continuación.

| **Problemas en dispositivos móviles** | | |
| --- | --- | --- |
| **Problema** | **Razones posibles** | **Solución** |
| La aplicación móvil en iOS se bloquea y no funciona correctamente. | La versión de iOS es demasiado antigua. | Actualiza tu versión de iOS o utiliza otro dispositivo. Nuestra aplicación móvil para iOS es compatible con las versiones 12 o superiores. |
| Puedo iniciar sesión correctamente en la aplicación de escritorio, pero la carga queda atascada en el logotipo de Miro en un dispositivo móvil. | Los datos de autenticación están dañados (caché con problemas). | Ve a **App settings (Ajustes de la aplicación) > Storage (Almacenamiento) > Clear storage (Borrar almacenamiento)** o reinstala la aplicación de Miro en tu dispositivo. |
| Recibo el error “Ocurrió un error” cuando intento autenticar mediante SSO en la aplicación móvil. | 1. 1. La conexión de red está protegida y algo bloquea las solicitudes.  2. 2. Chrome está agregado a la lista ADFS de agentes de usuarios compatibles con WIA y direcciona de forma incorrecta al usuario./span>  3. 3. Es posible que este dispositivo específico no pueda acceder al entorno de SSO de la empresa. | 1. 1. Intenta autorizar después de conectarte a una red diferente  2. 2. Comunícate con tu administrador de sistema y pídele que elimine a Chrome de la lista.  3. Consulta con tu departamento de TI para verificar si existe alguna restricción con respecto a dispositivos específicos para el uso de SSO. |
| No puedo encontrar los archivos importados desde los tableros en el sistema de archivos del dispositivo móvil. | Cuando descargas un archivo desde un tablero en el dispositivo móvil, queda “escondido” para ti durante algún tiempo. | Espera hasta que el archivo aparezca en la carpeta que contiene los archivos descargados. |
| Cuando inicio sesión en Miro en el dispositivo móvil, veo el mensaje “No hay cuentas disponibles” y no puedo acceder a mi perfil. | Te eliminaron o [saliste](../../managing-your-profile/06-how-to-leave-a-team.md) de todos tus equipos. | Inicia sesión en Miro desde un escritorio o una tableta, y crea un equipo nuevo. O bien, pídele a otro usuario que te invite a un equipo de Miro. |
| No puedo editar tableros de Miro en el navegador o el dispositivo móvil. | Estamos al tanto de esta limitación en este momento. | Cambia a nuestra [aplicación móvil](../../../getting-started/apps-for-devices/08-mobile-app.md), tableta o escritorio. |
| No puedo exportar mi tablero con la aplicación móvil. | Estamos al tanto de esta limitación en este momento. | Intenta cambiar a otro dispositivo.  Más información sobre la exportación en Miro en [esta página](../../import-and-export/export/03-how-to-export-your-board.md). |

| **Problemas en las tabletas** | | |
| --- | --- | --- |
| **Problema** | **Razones posibles** | **Solución** |
| La barra de herramientas desaparece o se comporta de forma extraña cuando uso Miro en el iPad. | Nuestra aplicación usa WebView para renderizar las imágenes y una de las reglas relacionadas con la gestión de memoria es que el proceso de renderizado no puede usar más del 25% de la memoria RAM del dispositivo.  Después de este límite, la aplicación se limita y deja de cargarse correctamente sin mostrar mensajes de error ni bloqueos. | - Cierra todas las aplicaciones innecesarias que estén funcionando en segundo plano antes de usar Miro - Trabaja en tableros que sean *más pequeños* - Por último, usa *otro dispositivo* (por ejemplo, de escritorio) con una mejor memoria RAM. |
| Puedo iniciar sesión correctamente en la aplicación de escritorio, pero la carga se atasca en el logotipo de Miro cuando uso una tableta. | Los datos de autenticación están dañados. | Ve a **Ajustes de la aplicación > Almacenamiento > Borrar almacenamiento** o reinstala la aplicación de Miro en tu dispositivo. |
| Recibo el mensaje de error “No puedes copiar tantos objetos al mismo tiempo” cuando pego objetos en el iPad. | Excediste la cantidad de datos que se pueden poner en un búfer en el iPad. | Copia y pega menos widgets a la vez. |
| No puedo editar [los documentos de Google que están cargados en el tablero](../../../integrations-apps/google/05-google-drive.md) en mi tableta. | Estamos al tanto de esta limitación en este momento. | Una solución alternativa puede ser abrir el documento mediante la aplicación de Google Docs desde el **ícono** Source (Fuente). |
| Uso el Apple Pencil en el iPad.  Cuando toco dos veces para cambiar de lápiz a borrador, no sucede nada. | La posibilidad de alternar entre lápiz y borrador tocando dos veces es una característica nativa de la 2.° generación de Apple Pencils, no es una función desarrollada específicamente por Miro.  Solo es compatible con la aplicación para tableta. | Asegúrate de que tu Apple Pencil admita la característica y cambia a la [aplicación para tabletas](../../../getting-started/apps-for-devices/11-tablet-app.md). |
| Las siguientes dos cosas no funcionan en el iPad:   - Acercamiento cuando se realiza mediante la rueda del mouse. - Navegar por el tablero cuando se activa con el desplazamiento de dos dedos en el trackpad. | Estamos al tanto de esta limitación relacionada con las restricciones del SO en el iPad. | Lamentablemente, aún no tenemos una solución para esto. |
