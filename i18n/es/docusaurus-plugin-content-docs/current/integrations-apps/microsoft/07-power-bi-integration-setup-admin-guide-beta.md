---
title: Configuración de la integración de Power BI (guía para admins) (versión beta)
article_id: 18945328862994
translation_id: 18945328862994
locale: es
sidebar_position: 8
created_at: '2024-05-15T12:57:57Z'
updated_at: '2025-11-25T15:42:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
availability:
  notes: 'Disponible para: planes Free, Starter, Business, Education y Enterprise
    Disponible en: navegador, aplicación de escritorio Rol necesario: admin de empresa'
---

Para las organizaciones que buscan integrar Microsoft Power BI con Miro, esta guía ofrece instrucciones paso a paso sobre cómo configurar la integración, habilitarla para los equipos y abordar las consideraciones de seguridad.

Funciones principales:

- Insertar informes y paneles de Power BI en tableros de Miro
- Especificar gráficos para importar a tableros de Miro
- Solicitar contenido actualizado de Power BI directamente de tableros de Miro

:::tip
Por el momento, la integración de Power BI está en versión beta privada.
:::

### Implementación técnica

Miro se integra con Power BI a través de la [API REST](https://learn.microsoft.com/rest/api/power-bi/) junto con las [API de cliente de análisis integrado de Power BI](https://learn.microsoft.com/javascript/api/overview/powerbi/). Los usuarios pueden vincular fácilmente sus informes o paneles de Power BI a tableros de Miro autorizando el acceso de Power BI. Para la autenticación, utilizamos [OAuth2.0](https://learn.microsoft.com/entra/identity-platform/v2-protocols).

### Requisitos de la integración

Asegúrate de que tu suscripción incluya lo siguiente:

- Power BI en la nube
- Suscripciones compatibles:
  - SKU de Power BI Premium por capacidad
  - SKU de reserva de capacidad de Fabric

## Configurar la integración de Power BI

1. Inicia sesión en Microsoft Entra como admin.
2. Navega hasta **Aplicaciones empresariales** > **Consentimiento y permisos** > **Configuración de consentimiento del administrador**.
3. En **Configuración de consentimiento del administrador**, selecciona **Sí** para **Los usuarios pueden solicitar el consentimiento del administrador para las aplicaciones en las que no puedan proporcionar un consentimiento**.
4. En **Quién puede revisar las solicitudes de consentimiento del administrador**, selecciona los usuarios, roles y grupos necesarios a quienes se les permitirá revisar las solicitudes de consentimiento del admin.
5. De esa forma, los usuarios podrán solicitar la aprobación. Para ver la pantalla de solicitud de aprobación, un usuario que no sea admin debe pegar un enlace de Power BI en un tablero de Miro del equipo de Miro habilitado para las pruebas de integración de Miro y Power BI.
6. Los admins seleccionados en el paso 4 pueden navegar hasta la pantalla de solicitudes de consentimiento del admin y aprobar la solicitud pendiente.
7. Una vez aprobada, se permite que cualquier usuario autorice la integración de Miro y Power BI por su propia cuenta.
8. Para comprobar si la integración funciona, pega un enlace a un panel o a un informe de Power BI en un tablero de Miro que pertenezca a un equipo para el que hayas habilitado la integración.
9. Haz clic en **Conectar** para confirmar la autorización en la página web de Power BI.
10. Se abrirá un diálogo que te indicará que selecciones los gráficos que quieras insertar. Selecciona un gráfico y haz clic en **Agregar gráfico**.
11. Los gráficos se agregarán como imágenes a tu tablero de Miro.

## Cómo desactivar la integración de Power BI

Para revocar el permiso, los admins pueden eliminar la aplicación de Miro de las aplicaciones empresariales en Microsoft Entra.

1. Inicia sesión en Microsoft Entra.
2. Haz clic en **Aplicaciones empresariales** > **Consentimiento y permisos**.
3. En la lista de aplicaciones, busca y selecciona la opción **Todas las aplicaciones**.
4. Busca la aplicación **Contenthub Microsoft Power BI Integration** (Integración de Microsoft Power BI del Centro de contenido) en la lista.
5. Haz clic en la aplicación para acceder a sus propiedades.
6. Dentro de las propiedades de la aplicación, haz clic en **Eliminar**.

## Limitaciones de la integración

- No se admite la inserción en tableros públicos.
- No se admite la inserción de enlaces de conjuntos de datos.
- No se admite la inserción de enlaces desde el menú Compartir.

## Retención de datos

Los datos insertados de Power BI cumplen con la política de retención de datos estándar de Miro que se aplica a todos los datos de los clientes. Lee nuestro [Apéndice de procesamiento de datos de Miro](https://miro.com/legal/documents/Miro-Data-Processing-Addendum.pdf).

Diferentes tipos de datos de enlaces de Power BI pegados se obtienen como imagen y se almacenan en Miro:

- Imágenes de mosaicos de los paneles de Power BI
- Imágenes de objetos visuales de los informes de Power BI
- Títulos de los paneles, informes, objetos visuales y mosaicos de Power BI
- Nombres de páginas de los informes de Power BI
- Nombres y valores de filtros de los informes de Power BI

## Preguntas frecuentes

¿Por qué la integración de Power BI está en versión beta?

La fase beta tiene como objetivo recopilar comentarios para mejorar la estabilidad y la experiencia del usuario. La seguridad es siempre prioritaria.
