---
title: Amazon Q (Beta)
article_id: 31347586131346
translation_id: 31347586131346
locale: es
sidebar_position: 3
created_at: '2025-11-25T13:35:45Z'
updated_at: '2025-12-29T15:25:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: '¿Quién puede hacerlo?: Propietarios de tableros, copropietarios de tableros,
    editores de tableros, miembros del equipo, admins de equipo, admins de usuarios,
    admins de contenido, (Configuración) admins de empresa; admin de Amazon Q ¿Cuáles
    planes?: Business, Enterprise ¿Cuáles plataformas?: Navegador, Escritorio'
---

La integración de Amazon Q permite a los equipos recuperar conocimientos de la empresa en la plataforma Miro AI a través de compañeros de IA y flujos. La inteligencia empresarial se entrega y visualiza directamente dentro de Miro.

:::note
Solo puedes usar la integración de Amazon Q con la plataforma Miro AI. [Regístrate aquí](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb) para obtener acceso.  Se te notificará cuando la plataforma Miro AI esté habilitada para tu organización.
:::

El conocimiento empresarial a menudo está disperso en numerosas herramientas como Slack, Confluence, Salesforce, Google Drive y repositorios internos, lo que obliga a gerentes de producto, líderes de ingeniería y equipos de tecnología a invertir tiempo valioso buscando detalles cruciales y alineando perspectivas.

Las siguientes funcionalidades de Miro y Miro AI respaldan la integración con Amazon Q:

- [**Flujos**](../../using-miro/miro-ai/04-flows-overview.md)
  Visualiza flujos de trabajo que transforman información dispersa en entregables claros, ayudando a los equipos a automatizar y estandarizar cómo convierten las ideas en acción.
- [**Asistentes**](../../using-miro/miro-ai/06-sidekicks-overview.md)
  Trabaja en conjunto con agentes de IA que razonan sobre el contenido del tablero y datos empresariales para generar nuevos artefactos, brindar ideas instantáneas y acelerar el proceso creativo, la documentación y el diseño.

## Configurar la integración de Amazon Q

Asegúrate de haber [registrado aquí](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb), y de haber recibido la confirmación de Miro de que la plataforma Miro AI está habilitada para tu organización, luego completa los siguientes dos procedimientos.

Para configurar la integración de Amazon Q con Miro, debes añadir a Miro como un data accessor en Amazon Q Business, y luego conectar el índice de Amazon Q al Admin Console en Miro.

### Añadir a Miro como data accessor en Amazon Q Business

1. En la consola de Amazon Q Business, en el panel de navegación, haz clic en **Aplicaciones**.
2. Haz clic en la aplicación donde deseas añadir un acceso de datos.
3. En el panel de navegación, haz clic en **Accesos de datos**.
4. Haz clic en **Añadir acceso de datos**.
5. Bajo **Accesos de datos**, para **Miro**, haz clic en el icono más (**+**).
6. Para **ID externo**, agrega el ID de tu organización en Miro.
   Para obtener tu ID de organización en Miro, ve a Admin Console. Copia el ID de organización desde la barra de URL del navegador.
   ![](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/31367058137746_image.png)
   *Encuentra el ID de tu organización en el Admin Console. Puedes copiar el ID desde la barra de URL del navegador.*
7. Haz clic en **Agregar acceso de datos**.
8. Toma nota de los siguientes detalles. Necesitas cada valor para completar la configuración en la Consola de Administración de Miro:
   - ID de la aplicación
   - ARN de la aplicación IdC
   - ID de Recuperador
   - Región de la aplicación
   - Región de la aplicación IdC

### Conectar un índice de Amazon Q a la Consola de Administración en Miro

1. En Miro, ve a **Consola de Administración** > **Aplicaciones e integraciones** > **Aplicaciones** > **Agregar aplicaciones**.
2. Busca y localiza Amazon Q.

   > ✏️ Si no puedes encontrar Amazon Q por nombre, busca usando el siguiente ID de cliente: `1601842442647206821`.
3. En el perfil de la aplicación, selecciona si deseas agregar la aplicación para **Todos los equipos** o **Equipos específicos**.
4. Revisa la página de permisos.

   > ✏️ La aplicación Amazon Q es desarrollada y mantenida por Miro y no requiere permisos específicos.
5. Haz clic en **Agregar**.
6. Ve a **Apps** > **Gestionar Apps**.
7. Busca y localiza Amazon Q.
8. Haz clic en **Configuración**.
9. Añade los detalles del acceso a los datos de Amazon Q. Mira el paso final en Añadir Miro como un accesor de datos en Amazon Q Business.
10. Haz clic en **Guardar**.
    Tu configuración está aplicada.
