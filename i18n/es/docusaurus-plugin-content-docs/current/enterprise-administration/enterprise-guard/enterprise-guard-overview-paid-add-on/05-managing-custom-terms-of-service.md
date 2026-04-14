---
title: "Administraci\xF3n de Condiciones del Servicio personalizadas"
article_id: 27621616452882
translation_id: 27621616452882
locale: es
sidebar_position: 3
created_at: '2025-06-24T23:29:13Z'
updated_at: '2025-11-04T14:10:40Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

## Creación de Condiciones del Servicio personalizadas

:::note
Notas:

- Los admins deben tener los siguientes privilegios de Enterprise Guard para ver y administrar las Condiciones del Servicio personalizadas:
  - El admin de contenido tiene permisos incorporados.
  - Los roles de admin personalizadas deben incluir:
    - Ver Condiciones del Servicio personalizadas
    - Administrar Condiciones del Servicio personalizadas
- Los invitados y usuarios externos están excluidos.
- Miro no almacena las condiciones, solo el enlace y metadatos.
:::

1. Ve a **Configuración** > **Enterprise Guard** > **Condiciones del Servicio Personalizadas**
2. Si estás creando condiciones del servicio personalizadas por primera vez, haz clic en **Agregar condiciones del servicio**.
   Si ya tienes una configuración existente y quieres agregar otra, haz clic en **Crear nueva** desde la vista de lista
3. En **Configurar** → **Condiciones**:
   - **Activador**: Elige entre **Inicio de sesión exitoso** o **Uso de IA**.
     **Inicio de sesión exitoso**

     - El diálogo aparece inmediatamente después del inicio de sesión.
     - Los usuarios pueden hacer clic en **Continuar** para aceptar y proceder, o en **Cerrar sesión**.

     **Uso de IA**

     - El diálogo aparece cuando el usuario interactúa con Miro AI, como al cambiar la disposición de AI, abrir el panel lateral de AI o iniciar una herramienta o acción de AI (por ejemplo, compañeros de IA).
     - Los usuarios pueden hacer clic en **Continuar** para aceptar y usar funciones de AI. Si los usuarios hacen clic en **Cancelar**, permanecen conectados y pueden continuar usando todas las funciones que no son de AI.
   - **Alcance**: **Todos los usuarios y admins de la organización**.
   - **Período de recurrencia**: introduce un número y selecciona **Días**, **Semanas** o **Meses**.Por defecto: dos semanas.
     No se solicita a los usuarios de nuevo hasta que finalice el periodo de recurrencia o se actualicen las condiciones.
4. En **Configurar** → **Contenido**:
   - **Título** (máx. 32 caracteres)
   - **Descripción** (máx. 200 caracteres)
   - **Enlace:** Enlaces a políticas (alojados externamente). Para incluir enlaces adicionales, haz clic en +Añadir enlace. Se admiten hasta tres enlaces. Cada URL de enlace debe ser única.
   - **Texto del enlace** (máx. 60 caracteres). Cada texto de enlace debe ser único.
5. Haz clic en **Mostrar vista previa** (arriba a la derecha) para revisar el contenido del cuadro de diálogo de las condiciones del servicio personalizadas. Realiza ajustes al contenido de las condiciones del servicio personalizadas, si es necesario.
6. Una vez que hayas terminado con el contenido de las Condiciones del Servicio personalizadas, haz clic en **Siguiente**.
7. Revisa las Condiciones del Servicio personalizadas, confirma tu configuración y contenido, luego haz clic en **Publicar**.
   La aplicación es inmediata para el desencadenante seleccionado.

## Editar Condiciones del Servicio personalizadas

1. Abre **Configuración** > **Enterprise Guard** > **Condiciones del Servicio personalizadas**.
2. En la lista, selecciona la configuración de condiciones del servicio personalizada que deseas actualizar y luego haz clic en **Editar**.
3. Actualiza los campos según sea necesario en **Condiciones** y **Contenido**.
4. Si deseas actualizar las condiciones del servicio personalizadas y restablecer todos los aceptaciones de usuarios inmediatamente, haz clic en **Publicar inmediatamente.**
   Si deseas actualizar las condiciones del servicio personalizadas e instruir a los usuarios nuevamente después de que finalice el período de recurrencia configurado, haz clic en la flecha hacia abajo, selecciona **Publicar en el próximo ciclo** y luego haz clic en **Publicar en el próximo ciclo**.

## Eliminar Condiciones del Servicio personalizadas

La eliminación deshabilita las Condiciones del Servicio personalizadas de inmediato y no se puede deshacer.

1. Abre **Ajustes** > **Enterprise Guard** > **Condiciones del Servicio personalizadas**.
2. En la lista, selecciona la configuración de Condiciones del Servicio personalizadas que deseas eliminar y haz clic en **Eliminar**.
3. Para eliminar permanentemente las Condiciones del Servicio personalizadas que seleccionaste, haz clic en **Eliminar condiciones**.
