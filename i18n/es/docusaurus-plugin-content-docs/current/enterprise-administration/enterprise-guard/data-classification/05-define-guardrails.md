---
title: "Definir las barreras de protecci\xF3n"
article_id: 16494716849810
translation_id: 16494716849810
locale: es
sidebar_position: 4
created_at: '2024-01-19T19:01:45Z'
updated_at: '2025-11-25T15:40:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Definir barreras de protección es el tercer paso del flujo de configuración de la clasificación automática y barreras de protección. En este paso del flujo, configurarás las barreras de protección, que son las restricciones aplicables para cada nivel de clasificación, como bloquear el uso compartido público, el uso compartido con equipos, el uso compartido con la organización o la replicación de contenido. Por ejemplo, puedes configurar barreras de protección para bloquear el uso compartido público, el uso compartido con equipos, el uso compartido con la organización y la replicación de contenido para usuarios de tableros clasificados como CONFIDENCIAL.

### Requisitos previos

- Debes completar el primer y segundo paso del flujo de auto-clasificación y guardrails, [1: <a href="">Definir los niveles de clasificación](07-define-classification-levels.md) y [2</a>: Definir la clasificación automática](07-define-classification-levels.md).
- Debes conocer las barreras de protección que deseas asignar a cada nivel de clasificación según tus requisitos de seguridad y gobernanza.
- Debes tener el [rol admin de contenido sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar el rol de admin de contenido sensible, ponte en contacto con el admin de empresa.

Los admins tienen dos opciones para implementar las Barreras de Protección Inteligentes en su organización:
**Modo predeterminado:** De forma predeterminada, las barreras de protección no afectarán las opciones de uso compartido activas en los tableros para evitar interrumpir la colaboración en curso, incluso cuando los tableros se reclasifiquen durante la clasificación automática.

**Modo estricto:** Cuando el interruptor de Aplicar barreras de protección en modo estricto está activado, las barreras de protección anulan todas las opciones de uso compartido activas. Esto ofrece a los Admins los niveles más estrictos de control, pero también puede provocar que algunos usuarios pierdan el acceso a los tableros de inmediato.

![guardrails.png](images/26201237843730_guardrails.png)

## Asignar barreras de protección

Para asignar barreras de protección a un nivel de clasificación, sigue estos pasos:

1. En la página **Definir barreras de protección**, haz clic en el icono de **Editar** del nivel de clasificación para el cual deseas asignar las barreras de protección. Por ejemplo, si quieres asignar límites de seguridad para el nivel de clasificación CONFIDENCIAL, haz clic en el icono Editar en la fila del nivel de clasificación CONFIDENCIAL.
2. Selecciona la casilla de verificación para cada etiqueta de guardarraíl que deseas asignar a este nivel de clasificación. Por ejemplo, si deseas bloquear el uso compartido público, bloquear el uso compartido con equipos, bloquear el uso compartido con la organización, bloquear la replicación de contenido para los usuarios de tableros clasificados como CONFIDENCIAL, bloquear el uso compartido fuera de los dominios permitidos y bloquear el uso de Miro AI, selecciona las siguientes casillas:
   - **Bloquear la replicación de contenido**- **Bloquear el uso de Miro AI (Beta)**
   **Bloquear el uso compartido público**
   - **Bloquear el uso compartido con equipos**
   **Bloquear el uso compartido con la organización**
   **- Bloquear el uso compartido fuera de los dominios permitidos (Beta)**
   Después de seleccionar esta casilla, debes agregar los dominios que quieres permitir escribiéndolos y seleccionándolos de la lista de dominios permitidos en la organización, o escribiendo un nuevo dominio en el cuadro y haciendo clic en **Agregar**.
   Para más información sobre cada contenido y directriz de compartición, consulta [Intelligent Guardrails overview and scenarios](01-intelligent-guardrails-overview.md).
3. De forma predeterminada, las barreras de protección no afectarán las opciones de uso compartido activas en los tableros para evitar interrumpir la colaboración en curso, incluso cuando los tableros se reclasifican durante la clasificación automática.

   Si deseas aplicar barreras de protección y anular todas las opciones de uso compartido activas, activa el interruptor **Aplicar barreras de protección en modo estricto**. Esto puede resultar en que los usuarios pierdan el acceso a los tableros. Esto proporciona a los Admins los niveles más estrictos de control, pero también puede resultar en que algunos usuarios pierdan acceso a los tableros de inmediato.
   ![guardrails.png](images/26201237843730_guardrails.png)
4. Haz clic en **Hecho**.
   Tu configuración está guardada, pero solo surtirá efecto después de que hagas clic en **Publicar** en la página de [**Revisar impacto**](06-review-impact.md).
5. Cuando termines de definir las barreras de protección para los diversos niveles de clasificación, procede a [completar la configuración de las barreras de protección](05-define-guardrails.md).

## Completa la configuración de las barreras de protección

Después de que termines de asignar las barreras de protección para diferentes niveles de clasificación, haz clic en **Siguiente**. Tu configuración está guardada, pero solo tendrá efecto después de que hagas clic en **Publicar** en la página de [Revisar impacto](06-review-impact.md).
