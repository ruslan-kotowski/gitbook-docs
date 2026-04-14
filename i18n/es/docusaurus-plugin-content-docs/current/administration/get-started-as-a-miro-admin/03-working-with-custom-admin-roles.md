---
title: Trabajar con roles de admin personalizados
article_id: 22182074695698
translation_id: 22182074695698
locale: es
sidebar_position: 3
created_at: '2024-10-24T13:17:04Z'
updated_at: '2025-04-25T13:57:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Los admins de empresa y aquellos que tengan los privilegios necesarios ahora pueden crear y administrar roles personalizados adaptados a necesidades específicas de la organización. Esta funcionalidad mejora el control de la administración de usuarios, la seguridad y el ciclo de vida del contenido al ofrecer privilegios personalizables. Los admins pueden asignar, actualizar o eliminar roles de admin personalizados según sea necesario, lo que garantiza la alineación con los flujos de trabajo de la organización. Los beneficios clave de los roles de admin personalizados incluyen los siguientes:

- **Flexibilidad:** ajusta los roles de admin personalizados para satisfacer diversas necesidades administrativas.
- **Escalabilidad:** adapta los privilegios a medida que tu organización crece y evolucionan los requisitos.
- **Seguridad mejorada:** asigna privilegios precisos para mantener el cumplimiento y la integridad de los datos.
- **Facilidad de uso:** accede a una interfaz intuitiva para crear y administrar roles.

## Crear un rol de admin personalizado

:::note
Para crear un rol de admin personalizado, debes ser un admin de empresa o un admin personalizado que tenga privilegios para ver, editar y asignar roles de admin.
:::

1. Ve a tu [consola de admin](https://miro.com/app/settings).
2. En el panel izquierdo, en **Usuarios**, haz clic en **Roles de admin**.
3. En la esquina superior derecha de la página **Roles de admin**, haz clic en **Crear rol**.
4. En la página **Ingresar detalles**:
   a. En el cuadro **Nombre del rol**, ingresa un nombre único y descriptivo para el nuevo rol de admin personalizado que vas a crear. Puede tener 60 caracteres como máximo y debe ser único entre todos los nombres de roles personalizados de una organización.
   b. En el cuadro **Descripción del rol**, ingresa una descripción que ayude a otros admins a comprender este rol de admin personalizado. La descripción del rol puede tener 120 caracteres como máximo.
   c. Haz clic en **Siguiente**.
5. En la página **Establecer los privilegios**:
   a. Selecciona la casilla de verificación de cada privilegio que quieres habilitar para este rol personalizado. Si quieres seleccionar todos los privilegios de una categoría específica, haz clic en **Seleccionar todo**.
   b. Haz clic en **Siguiente**.
6. En la página **Asignar usuarios**:
   a. Selecciona la casilla de verificación junto a cada usuario para el que quieres habilitar este rol personalizado. También puedes usar la barra de búsqueda para buscar en la lista por nombre, correo electrónico o dominio.
   b. Haz clic en **Siguiente**.
7. En la página **Revisar**:
   a. Revisa toda la información de este rol personalizado para garantizar que los detalles, los privilegios y los usuarios sean correctos.
   b. Si los detalles del rol personalizado son correctos, haz clic en **Crear rol**.
   Si necesitas realizar cambios después de revisar los detalles del rol personalizado, haz clic en el botón **Anterior**, realiza los cambios necesarios y luego vuelve a revisarlos.

   Una vez creado el rol personalizado, aparecerá en la lista de roles de admin y se marcará con la etiqueta PERSONALIZADO.

:::note
Si un usuario pierde el rol de membresía ORGANIZATION_INTERNAL_USER u ORGANIZATION_INTERNAL_ADMIN en la organización, también perderá todos los roles personalizados o predefinidos asociados.
:::
