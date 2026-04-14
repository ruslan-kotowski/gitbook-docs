---
title: Mover datos entre regiones – Exportación e importación manuales
article_id: 24778387087122
translation_id: 24778387087122
locale: es
sidebar_position: 6
created_at: '2025-02-20T09:07:00Z'
updated_at: '2025-11-25T15:49:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Quién puede hacerlo: propietarios de tableros, copropietarios de tableros,
    admins de contenido, admins de empresa Qué planes: Enterprise Qué plataformas:
    navegador, escritorio'
---

Este artículo describe el método de exportación e importación manual para mover datos entre regiones. Para obtener más información sobre las opciones para mover datos entre regiones, incluida la migración automatizada, consulta [Mover datos entre regiones](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Prepararse para una exportación e importación manual a una nueva región

Como admin de empresa, las siguientes prácticas recomendadas te ayudarán a prepararte para un traslado manual a una nueva región:

- Para iniciar una nueva organización en la región de destino, comunícate con tu contacto específico de Miro.
- Para asegurarte de poder gestionar a todos los usuarios de tu dominio, verifica todos los dominios de tu propiedad con la verificación de DNS.
- Activa la política de control de dominio **Bloquear suscripciones propias**, que garantiza que los usuarios no creen por accidente suscripciones gratuitas de Miro en la región anterior.
- Consolida los equipos u organizaciones en una sola organización con una única suscripción.
- Audita qué integraciones usará y necesitará tu organización en la nueva región y, a continuación, planifica un cronograma para reconfigurar cada integración en la nueva región.
- Audita toda la configuración que tu organización usa actualmente y, a continuación, planifica un cronograma para reconfigurar cada parámetro que necesitarás en la nueva región.

## Exportar e importar datos manualmente en una nueva región

Miro aprovisiona una nueva organización Enterprise en la región de destino. Los usuarios deben exportar sus tableros como copias de seguridad desde la región de origen y, a continuación, importarlas en la región de destino.

**Más información:** Consulta [Cómo guardar una copia de seguridad de un tablero](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md).

Solo los usuarios con los siguientes permisos pueden exportar e importar contenido manualmente:

- Propietario del tablero
- Copropietarios del tablero
- Admin de empresa
- Admin de contenido

:::note
Se perderá el uso compartido de los tableros. Los usuarios deberán restaurar sus permisos de uso compartido después de cargar la copia de seguridad en la región de destino.
:::

Para comenzar la importación manual de contenido, los usuarios pueden iniciar sesión en su nueva URL regional, que es una de las siguientes:

- (Australia) [au.miro.com](https://au.miro.com/)
- (Estados Unidos) [us.miro.com](https://us.miro.com/)

:::note
Como usuario, antes de iniciar sesión por primera vez, verifica si tu organización usa el inicio de sesión único (SSO). En caso afirmativo, espera a que tu admin de empresa reconfigure el SSO en la nueva región.
:::

## Qué hacer después de una exportación e importación manual

Después de una migración de datos entre regiones, asegúrate de hacer lo siguiente:

- Reconfigura el SSO de inmediato, si corresponde, para los nuevos subdominios regionales. Por ejemplo, au.miro.com.
  > ✏️ Los usuarios no podrán iniciar sesión en la nueva región hasta que se reconfigure el SSO en el IdP.
- Reconfigura SCIM para los nuevos subdominios regionales. Por ejemplo, au.miro.com.
- Verifica que esté activado **Bloquear suscripciones propias** en la configuración del control de dominio.
- Valida todos los demás parámetros de la organización, del control de dominio y de los equipos.
- Vuelve a instalar y configurar cada aplicación e integración de Enterprise, como SIEM, SAM, eDiscovery, Smarsh y Okta.
- Invita a los usuarios a la organización en la nueva región.

## Preguntas frecuentes sobre la exportación e importación manuales de datos en una nueva región

**¿Cómo funciona un traslado manual a una nueva región?**

Los admins vuelven a configurar la organización y todos sus equipos, los parámetros de los equipos y los usuarios. Los usuarios finales descargan manualmente las copias de seguridad de los tableros de la organización antigua y las cargan en la nueva organización.

**¿Quién cumple los requisitos y quién no?**

Los clientes Enterprise pueden mover sus datos a otra región. Para obtener más información, comunícate con tu persona de contacto de Miro.

**¿Qué datos se incluyen en un traslado manual?**

Solo los tableros movidos por los usuarios. Para obtener más información, consulta Exportar e importar datos manualmente en una nueva región.

**¿Hay un costo adicional?**

No. Miro puede aprovisionar una organización nueva en Australia o en los Estados Unidos mediante el contrato Enterprise estándar.

**¿Cuánto tiempo tarda un traslado manual?**

La duración de un traslado manual depende de cuánto tiempo necesiten los usuarios para exportar sus tableros guardados como copias de seguridad e importar el contenido de las copias en la región de destino.

**¿Cómo garantiza Miro que los datos de mi organización se eliminarán de la región de origen?**

Notifica al soporte de Miro una vez que completes la exportación e importación manuales en la nueva región, incluida la reconfiguración, y que todos los usuarios hayan importado sus copias de seguridad en la región de destino. El soporte de Miro eliminará tu organización y todos los datos de la región de origen.
