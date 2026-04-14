---
title: "Definir los niveles de clasificaci\xF3n"
article_id: 16494683650322
translation_id: 16494683650322
locale: es
sidebar_position: 6
created_at: '2024-01-19T18:57:35Z'
updated_at: '2025-11-25T15:40:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Este es el primer paso del flujo de configuración de la autoclasificación y las barreras de protección. En este paso del flujo, puedes definir los niveles de clasificación, lo que implica añadir nuevos niveles de clasificación o actualizar la configuración de un nivel de clasificación, como el nombre de la clasificación, el orden de sensibilidad, el color de la insignia, el enlace a las directrices de clasificación, etc. Al definir los niveles de clasificación puedes:

- [Añadir o editar un nivel de clasificación](07-define-classification-levels.md)
- [Configura la clasificación de datos importando etiquetas de sensibilidad de Microsoft Purview](07-define-classification-levels.md)
- [Actualizar el nivel de clasificación por defecto para los nuevos tableros](07-define-classification-levels.md)
- [Actualizar el orden de sensibilidad de un nivel de clasificación](07-define-classification-levels.md)
- [Eliminar un nivel de clasificación](07-define-classification-levels.md)

## Requisitos previos

- Debes conocer los detalles de los niveles de clasificación de tableros que quieres configurar en función de tus requisitos de seguridad y gobernanza.
- Debes tener el [rol admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.

## Añadir o editar un nivel de clasificación

Puedes añadir o editar un nivel de clasificación realizando los siguientes pasos:

1. Ve a tu [configuración de Miro.](https://miro.com/app/settings)
2. En el panel izquierdo, en **Enterprise Guard,** haz clic en **Clasificación de datos**.
3. Si estás definiendo niveles de clasificación por primera vez, haz clic en **Configurar clasificación** en la parte inferior de la pantalla.
   Si quieres editar los niveles de clasificación, haz clic en **Editar niveles de clasificación** en la parte superior derecha de la pantalla.
4. En la página **Definir niveles de clasificación**:
   Para añadir un nivel de clasificación, haz clic en **Añadir nivel**.
   Para editar un nivel de clasificación, haz clic en **Editar niveles de clasificación**.
5. Añade o edita el nivel de clasificación según tus necesidades. La tabla siguiente enumera cada campo y su descripción.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | **Nivel** | Indica el orden de sensibilidad de los tableros para este nivel de clasificación.  Actualmente, el orden de sensibilidad **1** indica el nivel de clasificación **menos sensible** .  Haz clic en las flechas hacia arriba o hacia abajo para asignar el orden de sensibilidad de los tableros para este nivel de clasificación. |
   | **Nombre** | Nombre del nivel de clasificación.  Cuando los usuarios ven un tablero que pertenece a este nivel de clasificación, este nombre aparece en la insignia de clasificación del tablero junto al nombre del tablero.  La Figura 1 ilustra un ejemplo en el que el nombre de la clasificación de los tableros es **INTERNO**.  ejemplo_tablero_interno.png Figura 1: Ejemplo en el que el nombre de la clasificación de los tableros es **INTERNO** |
   | **Descripción** | Descripción de este nivel de clasificación.  Cuando los usuarios ven un tablero que pertenece a este nivel de clasificación y hacen clic en la insignia de clasificación del tablero, aparece la descripción del nivel de clasificación.  Te recomendamos que añadas una descripción significativa que oriente a tus usuarios sobre la sensibilidad de este tablero y las precauciones o acciones recomendadas.  La Figura 2 ilustra un ejemplo de la **descripción** añadida para el nivel de clasificación INTERNO.   muestra_descripcion_interna.png Figura 2: Ejemplo de **descripción** añadida para el nivel de clasificación INTERNO |
   | **Color de insignia** | Color de fondo de la insignia de clasificación de los tableros.  La figura 3 ilustra un ejemplo en el que el nivel de clasificación del tablero INTERNO tiene una insignia de color **Amarillo**.  ejemplo_tablero_interno.png Figura 3: Ejemplo en el que el nivel de clasificación del tablero INTERNO tiene una insignia de color **Amarillo** |
   | **Enlace a los lineamientos** | URL que proporciona más información sobre las políticas o instrucciones aplicables a este nivel de clasificación. Puede ser una página que proporcione más información para que los usuarios de tu organización conozcan mejor los niveles de clasificación de tus tableros y cómo trabajar con ellos. Debes proporcionar la URL en el siguiente formato: `http://www.example.com`  Cuando el usuario hace clic en el icono **Más información** (icono de interrogación) situado junto a la insignia de clasificación del tablero, esta URL se carga en una nueva pestaña del navegador. |
   | **Usar como nivel predeterminado para los tableros nuevos** | Selecciona esta casilla para establecer este nivel de clasificación como la clasificación por defecto para todos los tableros nuevos. |
   | **Vista previa** | Muestra una vista previa de la insignia de clasificación del tablero con su descripción y el icono de más información. La vista previa muestra exactamente cómo aparece la insignia de clasificación para los usuarios de un tablero. |

   Para guardar la configuración de los niveles de clasificación, haz clic en **Listo**.
6. Haz clic en **Siguiente**. Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) de la página Revisar impacto.

   A continuación, puedes seguir cualquiera de los siguientes pasos:

   - Definir la clasificación automática Esto es opcional. Si quieres definir la autoclasificación más adelante, haz clic en **Siguiente**.
   - Definir las barreras de protección Esto es opcional. Si quieres definir las barreras de protección en un momento posterior, haz clic en **Siguiente**.
   - Revisar el impacto Este es el último paso del flujo de trabajo y es obligatorio.

## Configura la clasificación de datos importando etiquetas de sensibilidad de Microsoft Purview

### Requisitos previos

- Asegúrate de que tienes los roles o privilegios necesarios para trabajar con etiquetas de sensibilidad en Microsoft Purview.
- Debes conocer los detalles de los niveles de clasificación de tableros que quieres configurar en función de tus requisitos de seguridad y gobernanza.
- Debes tener el [rol admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.

:::note
Notas :
- Según la documentación de Microsoft, las actualizaciones de las etiquetas de sensibilidad en Microsoft Purview pueden tardar hasta 24 horas en replicarse a todas las apps y servicios. Por favor, deja tiempo suficiente para que se produzcan los cambios y luego importa las etiquetas de sensibilidad. Si las actualizaciones que hiciste en MS Purview no se replican al cabo de 24 horas, ponte en contacto con el equipo de Soporte de Microsoft Purview.
- Puedes importar hasta 50 etiquetas de sensibilidad de Microsoft Purview a Miro.
- Si ya tienes una configuración de clasificación de datos, puedes importar etiquetas de sensibilidad de Microsoft Purview y transferir las etiquetas de clasificación existentes en Miro. Para más información, consulta [Importar etiquetas de sensibilidad de Microsoft Purview a la configuración de Clasificación de Datos existente en Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Para importar etiquetas de sensibilidad del ámbito de Microsoft y configurar la clasificación de datos en Miro, realiza los siguientes pasos:

1. Ve a tu [configuración de Miro.](https://miro.com/app/settings)
2. En el panel izquierdo, en **Enterprise Guard,** haz clic en **Clasificación de datos**.
3. En la página **Clasificación** , en la parte inferior de la pantalla, haz clic en **Empezar**.
4. En el cuadro **Importar desde Microsoft Purview**, haz clic en **Iniciar sesión**.
5. En la página de **inicio de sesión de Microsoft** que aparece en una nueva pestaña, introduce tus credenciales de Microsoft e inicia sesión. Una vez que hayas iniciado sesión en tu cuenta Microsoft, la pestaña se cerrará automáticamente,
6. En la página **Clasificación** , en el cuadro **Importar desde Microsoft Purview**, haz clic en **Importar**.
   Aparece la página **Importar clasificación desde Microsoft Purview**.
7. Selecciona la casilla de verificación de las etiquetas de sensibilidad de Microsoft Purview que quieras utilizar como niveles de clasificación en Miro y, a continuación, haz clic en **Siguiente**.
   > ✏️ Según la documentación de Microsoft, las actualizaciones de las etiquetas de sensibilidad en Microsoft Purview pueden tardar hasta 24 horas en replicarse a todas las apps y servicios. Por favor, deja tiempo suficiente para que se produzcan los cambios y luego importa las etiquetas de sensibilidad. Si las actualizaciones que hiciste en MS Purview no se replican al cabo de 24 horas, ponte en contacto con el equipo de Soporte de Microsoft Purview.
8. En la página **Definir niveles de clasificación**, puedes editar los niveles de clasificación para asignar el nivel de clasificación por defecto o añadir un enlace a las directrices. La tabla siguiente enumera cada campo y su descripción.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | **Enlace a los lineamientos** | URL que proporciona más información sobre las políticas o instrucciones aplicables a este nivel de clasificación. Puede ser una página que proporcione más información para que los usuarios de tu organización conozcan mejor los niveles de clasificación de tus tableros y cómo trabajar con ellos. Debes proporcionar la URL en el siguiente formato: `http://www.example.com`  Cuando el usuario hace clic en el icono **Más información** (icono de interrogación) situado junto a la insignia de clasificación del tablero, esta URL se carga en una nueva pestaña del navegador. |
   | **Usar como nivel predeterminado para los tableros nuevos** | Selecciona esta casilla para establecer este nivel de clasificación como la clasificación por defecto para todos los tableros nuevos. |
   | **Vista previa** | Muestra una vista previa de la insignia de clasificación del tablero con su descripción y el icono de más información. La vista previa muestra exactamente cómo aparece la insignia de clasificación para los usuarios de un tablero. |

   Para guardar la configuración de los niveles de clasificación, haz clic en **Listo**.
9. Haz clic en **Siguiente**. Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) de la página Revisar impacto.

   A continuación, puedes seguir cualquiera de los siguientes pasos:

   - Definir la clasificación automática Esto es opcional. Si quieres definir la autoclasificación más adelante, haz clic en **Siguiente**.
   - Definir las barreras de protección Esto es opcional. Si quieres definir las barreras de protección en un momento posterior, haz clic en **Siguiente**.
   - Revisar el impacto Este es el último paso del flujo de trabajo y es obligatorio.

## Actualizar el nivel de clasificación por defecto para los nuevos tableros

Puedes actualizar el nivel de clasificación por defecto realizando los siguientes pasos:

1. Ve a tu [configuración de Miro.](https://miro.com/app/settings)
2. En el panel izquierdo, en **Enterprise Guard,** haz clic en **Clasificación de datos**.
3. Haz clic en **Editar niveles de clasificación** en la parte superior derecha de la pantalla.
4. En la página **Definir niveles de clasificación**, haz clic en **Editar niveles de clasificación**.
5. Haz clic en el icono **Editar** (![Captura de pantalla 2024-01-22 a las 23.20.18.png](images/21017430844178_Screenshot%202024-01-22%20at%2023.20.18.png)) del nivel que quieras establecer como nivel de clasificación por defecto.
6. Selecciona la casilla **Utilizar como nivel por defecto para los nuevos tableros**.
7. Haz clic en **Done** (listo).
   Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) de la página Revisar impacto.
8. Haz clic en **Siguiente**. Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) de la página Revisar impacto.

   A continuación, puedes seguir cualquiera de los siguientes pasos:

   - Definir la clasificación automática Esto es opcional. Si quieres definir la autoclasificación más adelante, haz clic en **Siguiente**.
   - Definir las barreras de protección Esto es opcional. Si quieres definir las barreras de protección en un momento posterior, haz clic en **Siguiente**.
   - Revisar el impacto Este es el último paso del flujo de trabajo y es obligatorio.

## Actualizar el orden de sensibilidad de un nivel de clasificación

Puedes actualizar el orden de sensibilidad de un nivel de clasificación realizando los siguientes pasos:

1. Ve a tu [configuración de Miro.](https://miro.com/app/settings)
2. En el panel izquierdo, en **Enterprise Guard,** haz clic en **Clasificación de datos**.
3. Haz clic en **Editar niveles de clasificación** en la parte superior derecha de la pantalla.
4. En la página **Definir niveles de clasificación**, haz clic en **Editar niveles de clasificación**.
5. Los niveles de clasificación aparecen con su orden de sensibilidad actual. Haz clic en las flechas hacia arriba o hacia abajo de los niveles de clasificación cuyo orden de sensibilidad quieras actualizar.

   > ✏️ Actualmente, el orden de sensibilidad **1** indica el nivel de clasificación **menos sensible** .

   Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón **[Revisar impacto](https://help.miro.com/hc/articles/16494764223378)** de la página Revisar impacto.
6. Haz clic en **Siguiente**. Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) de la página Revisar impacto.

   A continuación, puedes seguir cualquiera de los siguientes pasos:

   - Definir la clasificación automática Esto es opcional. Si quieres definir la autoclasificación más adelante, haz clic en **Siguiente**.
   - Definir las barreras de protección Esto es opcional. Si quieres definir las barreras de protección en un momento posterior, haz clic en **Siguiente**.
   - Revisar el impacto Este es el último paso del flujo de trabajo y es obligatorio.

## Eliminar un nivel de clasificación

:::note
No puedes eliminar un nivel de clasificación si está asociado a una [política de retención](https://help.miro.com/hc/sections/19180529348754).
:::

Puedes eliminar un nivel de clasificación realizando los siguientes pasos:

1. Ve a tu [configuración de Miro.](https://miro.com/app/settings)
2. En el panel izquierdo, en **Enterprise Guard,** haz clic en **Clasificación de datos**.
3. Haz clic en **Editar niveles de clasificación** en la parte superior derecha de la pantalla.
4. En la página **Definir niveles de clasificación**, haz clic en **Editar niveles de clasificación**.
5. Haz clic en el icono de eliminar del nivel de clasificación que quieras eliminar.
6. Si el nivel de clasificación que quieres eliminar ya se ha aplicado a 1 o más tableros, aparece una ventana de notificación informándote del número de tableros a los que se ha aplicado el nivel de clasificación.
   Selecciona el nuevo nivel de clasificación que quieres aplicar a los tableros afectados.
7. Haz clic en **Done** (listo).
   Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) de la página Revisar impacto.
8. Haz clic en **Siguiente**. Tu configuración se guarda, pero sólo entrará en vigor cuando hagas clic en **Publicar** en el botón [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) de la página Revisar impacto.

   A continuación, puedes seguir cualquiera de los siguientes pasos:

   - Definir la clasificación automática Esto es opcional. Si quieres definir la autoclasificación más adelante, haz clic en **Siguiente**.
   - Definir las barreras de protección Esto es opcional. Si quieres definir las barreras de protección en un momento posterior, haz clic en **Siguiente**.
   - Revisar el impacto Este es el último paso del flujo de trabajo y es obligatorio.
