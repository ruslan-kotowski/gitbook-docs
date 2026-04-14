---
title: Importar etiquetas de sensibilidad de Microsoft Purview
article_id: 22161930709010
translation_id: 22161930709010
locale: es
sidebar_position: 7
created_at: '2024-10-23T15:05:49Z'
updated_at: '2025-12-01T16:32:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Para las organizaciones que utilizan Microsoft Purview, mantener una seguridad de datos y clasificación consistentes en múltiples plataformas es esencial. La integración de Miro con Microsoft Purview permite a los administradores importar etiquetas de sensibilidad directamente desde Microsoft Purview a Miro, simplificando la gestión de esquemas de clasificación en ambas plataformas.

Al aprovechar esta integración, las organizaciones pueden asegurarse de que el contenido dentro de Miro esté clasificado de manera consistente con el marco establecido de Microsoft Purview. Esto no solo reduce la carga operativa de recrear o actualizar manualmente las etiquetas de clasificación, sino que también refuerza la seguridad de los datos. Al alinear las capacidades de protección de datos de Miro con Microsoft Purview, los admins pueden gestionar con confianza la información sensible en todo su ecosistema digital.

## Importar etiquetas de sensibilidad de Microsoft Purview a Miro

Si tu organización no tiene una configuración de clasificación de datos en Miro, puedes fácilmente configurar la Clasificación de Datos en Miro importando etiquetas de sensibilidad existentes directamente desde Microsoft Purview.

Si ya tienes una configuración de clasificación de datos existente, puedes importar etiquetas de sensibilidad de Microsoft Purview y transferir las etiquetas de clasificación existentes en Miro.

## Configura la Clasificación de Datos importando etiquetas de sensibilidad desde Microsoft Purview

### Requisitos previos

- Asegúrate de tener los roles o privilegios necesarios para trabajar con etiquetas de sensibilidad en Microsoft Purview.
- Debes conocer los detalles de los niveles de clasificación del tablero que deseas configurar según tus requisitos de seguridad y gobernanza.
- Debes tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.

:::note
Notas:
- Según la documentación de Microsoft, las actualizaciones de etiquetas de sensibilidad en Microsoft Purview pueden tardar hasta 24 horas en replicarse en todas las aplicaciones y servicios. Por favor, permite suficiente tiempo para que se realicen los cambios y luego importa las etiquetas de sensibilidad. Si las actualizaciones que hiciste en MS Purview no se replican después de 24 horas, contacta al equipo de soporte de Microsoft Purview.
- Puedes importar hasta 50 etiquetas de sensibilidad de Microsoft Purview a Miro.
- Si ya tienes una configuración de clasificación de datos existente, puedes importar etiquetas de sensibilidad desde Microsoft Purview y transferir las etiquetas de clasificación existentes en Miro. Para más información, consulta [Importar etiquetas de sensibilidad desde Microsoft Purview a una configuración de clasificación de datos existente en Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Para importar etiquetas de sensibilidad desde Microsoft Purview y configurar la clasificación de datos en Miro, realiza los siguientes pasos:

1. Ve a tus [configuraciones de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, bajo **Enterprise Guard,** haz clic en **clasificación de datos**.
3. En la página de **Clasificación**, al final de la pantalla, haz clic en **Comenzar**.
4. En el cuadro de **Importar desde Microsoft Purview,** haz clic en **Iniciar sesión**.
5. En la página de **Inicio de sesión de Microsoft** que aparece en una nueva pestaña, ingresa tus credenciales de Microsoft e inicia sesión. Una vez que hayas iniciado sesión en tu cuenta de Microsoft, la pestaña se cierra automáticamente.
6. En la página de **Clasificación**, en el cuadro de **Importar desde Microsoft Purview**, haz clic en **Importar**.
   La página **Importar clasificación de Microsoft Purview** aparece.
7. Selecciona la casilla de las etiquetas de sensibilidad de Microsoft Purview que deseas usar como niveles de clasificación en Miro, y luego haz clic en **Siguiente**.

   > ✏️ Según la documentación de Microsoft, las actualizaciones de las etiquetas de sensibilidad en Microsoft Purview pueden tardar hasta 24 horas en replicarse en todas las aplicaciones y servicios. Por favor, permite que se complete este tiempo antes de importar las etiquetas de sensibilidad. Si las actualizaciones realizadas en MS Purview no se replican después de 24 horas, comunícate con el equipo de Soporte de Microsoft Purview.
8. En la página **Definir niveles de clasificación**, puedes editar los niveles de clasificación para asignar el nivel de clasificación por defecto o agregar un enlace a las directrices. La tabla siguiente enumera cada campo y su descripción.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | **Enlace a las directrices** | URL que proporciona más información sobre políticas o instrucciones aplicables para este nivel de clasificación. Podría ser una página que ofrezca a los usuarios de tu organización más detalles sobre los niveles de clasificación de tu tablero y cómo trabajar con ellos. Debes proporcionar la URL en el siguiente formato: `http://www.example.com`  Cuando el usuario hace clic en el icono **Más información** (icono de signo de interrogación) al lado de la insignia de clasificación del tablero, esta URL se carga en una nueva pestaña del navegador. |
   | **Usar como nivel predeterminado para nuevos tableros** | Selecciona esta casilla para establecer este nivel de clasificación como la clasificación predeterminada para todos los nuevos tableros. |
   | **Vista previa** | Muestra una vista previa de la insignia de clasificación del tablero con su descripción y el ícono de más información. La vista previa muestra exactamente cómo aparece la insignia de clasificación para los usuarios en un tablero. |
9. Para guardar la configuración del nivel de clasificación, haz clic en **Hecho**.
10. Haz clic en **Siguiente**. Tu configuración se guarda, pero solo surtirá efecto después de hacer clic en **Publicar** en la página de [**Revisar el impacto**](https://help.miro.com/hc/articles/16494764223378).

    Puedes continuar con alguno de los siguientes pasos:

    - [Definir auto-clasificación](09-define-auto-classification.md). Esto es opcional. Si deseas definir la auto-clasificación más adelante, haz clic en **Siguiente**.
    - [Definir barreras de protección](05-define-guardrails.md). Esto es opcional. Si deseas definir las barreras de protección más adelante, haz clic en **Siguiente**.
    - [Revisar impacto](https://help.miro.com/hc/articles/16494764223378). Este es el último paso del flujo de trabajo y es obligatorio.

## Importar las etiquetas de sensibilidad de Microsoft Purview en la configuración de Clasificación de Datos existente en Miro

### **Requisitos previos**

- Asegúrate de tener los roles o privilegios necesarios para trabajar con etiquetas de sensibilidad en Microsoft Purview.
- Debes conocer los detalles de los niveles de clasificación de tableros que deseas configurar según tus requisitos de seguridad y gobernanza.
- Debes tener el [rol de admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.

:::note
Notas:
- Según la documentación de Microsoft, las actualizaciones de las etiquetas de sensibilidad en Microsoft Purview pueden tardar hasta 24 horas en replicarse en todas las aplicaciones y servicios. Por favor, permite el tiempo suficiente para que se realicen los cambios y luego importa las etiquetas de sensibilidad. Si las actualizaciones realizadas en MS Purview no se replican después de 24 horas, por favor contacta al equipo de soporte de Microsoft Purview.
- Puedes importar hasta 50 etiquetas de sensibilidad desde Microsoft Purview a Miro.
- No puedes transferir niveles de clasificación que se utilizan en políticas de retención. Debes asegurarte de que los niveles de clasificación no se usen en ninguna política de retención antes de continuar. Para más información, consulta [Editar política de retención](../content-lifecycle-management/11-edit-retention-policy.md).
:::

Para importar etiquetas de sensibilidad desde Microsoft Purview y transferir/mapear a etiquetas de clasificación existentes en Miro, sigue los siguientes pasos:

1. Ve a tu [configuración de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, bajo **Enterprise Guard**, haz clic en **clasificación de datos**.
3. En la página de **clasificación**, en la parte superior de la pantalla, haz clic en **importar**.
4. Si ya iniciaste sesión en Microsoft, omite este paso y procede al siguiente.
   Si no has iniciado sesión en Microsoft, haz clic en **Iniciar sesión**. En la página de **Inicio de sesión de Microsoft** que aparece en una nueva pestaña, introduce tus credenciales de Microsoft e inicia sesión. Una vez que hayas iniciado sesión en tu cuenta de Microsoft, la pestaña se cerrará automáticamente.
5. En el cuadro de **Importar desde Microsoft Purview**, haz clic en **Importar** junto a Importar etiquetas de sensibilidad a Miro. Aparece la página de **Importar clasificación de Microsoft Purview**.
6. En la página de **Importar Niveles**, selecciona la casilla de verificación de las etiquetas de sensibilidad de Microsoft Purview que quieres usar como niveles de clasificación en Miro, y luego haz clic en **Siguiente**. Aparece la página de **Transferir niveles existentes**.

   > ✏️ Según la documentación de Microsoft, las actualizaciones de las etiquetas de sensibilidad en Microsoft Purview pueden tardar hasta 24 horas en replicarse en todas las aplicaciones y servicios. Por favor, permite suficiente tiempo para que los cambios tengan efecto y luego importa las etiquetas de sensibilidad. Si las actualizaciones que realizaste en MS Purview no se replican después de 24 horas, por favor contacta al equipo de asistencia de Microsoft Purview.
7. Para garantizar que el contenido se clasifique correctamente, debes transferir los niveles de clasificación existentes de Miro a los nuevos niveles importados desde Microsoft Purview. Los niveles listados a la izquierda son los niveles de clasificación existentes en Miro y los que aparecen en la lista desplegable a la derecha son las etiquetas de sensibilidad importadas de Microsoft Purview. Una vez que termines, haz clic en **Siguiente**.
8. En la página **Definir niveles de clasificación**, puedes editar los niveles de clasificación para asignar el nivel de clasificación por defecto o agregar un enlace a las directrices. La tabla siguiente enumera cada campo y su descripción.

   |  |  |
   | --- | --- |
   | **Campo** | **Descripción** |
   | **Enlace a los lineamientos** | URL que proporciona más información sobre políticas o instrucciones aplicables a este nivel de clasificación. Podría ser una página que ofrezca más información a los usuarios de tu organización sobre los niveles de clasificación de tu tablero y cómo trabajar con ellos. Debes proporcionar la URL en el siguiente formato: `http://www.example.com`  Cuando el usuario hace clic en el icono **Obtén más información** (icono de signo de interrogación) junto a la insignia de clasificación del tablero, esta URL se carga en una nueva pestaña del navegador. |
   | **Usar como nivel predeterminado para nuevos tableros** | Selecciona esta casilla para establecer este nivel de clasificación como el nivel de clasificación predeterminado para todos los nuevos tableros. |
   | **Vista previa** | Muestra una vista previa de la insignia de clasificación del tablero con su descripción y el icono de aprender más. La vista previa muestra exactamente cómo aparece la insignia de clasificación para los usuarios en un tablero. |

   Para guardar la configuración del nivel de clasificación, haz clic en **Hecho**.
9. Haz clic en **Siguiente**. Tu configuración se guardará, pero solo se hará efectiva después de que hagas clic en **Publicar** en la página [**Revisión de impacto**](https://help.miro.com/hc/articles/16494764223378).

   Puedes proceder con uno de los siguientes pasos:

   - [Definir clasificación automática](09-define-auto-classification.md). Esto es opcional. Si quieres definir la clasificación automática más tarde, haz clic en **Siguiente**.
   - [Definir barreras de protección](05-define-guardrails.md). Esto es opcional. Si deseas definir las barreras de protección más tarde, haz clic en **Siguiente**.
   - [Revisar el impacto](https://help.miro.com/hc/articles/16494764223378). Este es el último paso del flujo de trabajo y es obligatorio.

## Desconectar de Microsoft Purview

Cuando estás conectado a Purview, no puedes agregar ni editar nombres de clasificación, actualizar niveles de clasificación, etc. Si deseas realizar estas acciones, debes desconectar de Microsoft Purview. No puedes importar actualizaciones de Microsoft Purview a Miro una vez que te desconectes de Purview.

Para desconectar de Microsoft Purview, sigue los siguientes pasos:

1. Ve a tu [configuración de Miro](https://miro.com/app/settings).
2. En el panel izquierdo, bajo **Enterprise Guard**, haz clic en **clasificación de datos**.
3. En la página de **clasificación**, en la parte superior de la pantalla, haz clic en el botón de **Última Importación**, y luego haz clic en **Desconectar de Purview**.
