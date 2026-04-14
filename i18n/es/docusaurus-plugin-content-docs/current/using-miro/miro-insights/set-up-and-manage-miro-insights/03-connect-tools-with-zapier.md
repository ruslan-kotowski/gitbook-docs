---
title: Conecta herramientas con Zapier
article_id: 30124629305106
translation_id: 30124629305106
locale: es
sidebar_position: 2
created_at: '2025-10-10T11:48:03Z'
updated_at: '2025-10-14T12:37:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Conecta Miro Insights con cientos de herramientas a través de [Zapier](http://zapier.com/) para capturar automáticamente comentarios y datos de fuentes que no tienen integraciones directas. Esto te permite centralizar opiniones de clientes de toda tu pila tecnológica.

La integración de Zapier te permite:

- Crear automáticamente elementos de comentarios a partir de tickets de soporte al cliente, encuestas o conversaciones de chat.
- Capturar datos de cualquier herramienta que Zapier soporte, incluso si Miro Insights no tiene una integración directa.
- Reducir la entrada manual de datos configurando flujos de trabajo automáticos.

## Crear comentarios

Zapier ofrece dos acciones principales para crear elementos de comentarios en Miro Insights.

### Crear comentarios

La acción estándar para crear elementos de comentarios generales en Miro Insights con los siguientes campos:

- **Título del comentario**: Breve resumen del comentario.
- **Contenido**: Contenido detallado del comentario o descripción.
- **Nombre del reportero**: Nombre de la persona que proporciona el comentario.
- **Correo electrónico del reportero**: Dirección de correo electrónico del proveedor del comentario.
- **Correo electrónico del propietario**: Propietario o asignado interno para el comentario.
- **Fecha y hora proporcionadas**: Momento en que se dio originalmente la opinión.
- **URL de origen**: Enlace a la fuente original (ticket, respuesta a encuesta, etc.).
- **Nombre de la empresa**: Organización con la que se asocia la opinión.
- **Dominio de la empresa**: Dominio del sitio web de la empresa.

### Crear comentarios (Llamada)

Una acción especializada diseñada específicamente para capturar comentarios de llamadas y conversaciones con estos campos:

- **Título de la llamada**: Título o asunto de la llamada.
- **Transcripción de la llamada**: Transcripción completa o notas de la llamada.
- **URL de origen**: Enlace a la grabación de la llamada o detalles de la reunión.
- **Participantes**: Información sobre los participantes de la llamada.
  - **Correo electrónico**: Dirección de correo del participante.
  - **Nombre**: Nombre del participante.
- **Correo electrónico del propietario**: Propietario o asignado interno para el feedback de la llamada.
- **Fecha y hora de inicio**: Cuándo tuvo lugar la llamada.
- **Nombre de la empresa**: Organización asociada con la llamada.
- **Dominio de la empresa**: Dominio del sitio web de la empresa.

## Configuración de la integración de Zapier

Para comenzar con Zapier y Miro Insights, sigue estos pasos.

### Requisitos previos

- Cuenta activa de Miro Insights
- Cuenta de Zapier (gratuita o de pago)
- Acceso a la herramienta fuente que deseas conectar

### Inicio rápido con plantillas

Miro Insights ofrece plantillas de Zapier predefinidas para herramientas populares de inteligencia conversacional, como Grain, Fathom y Fireflies.

Para configurar un Zap usando una plantilla:

1. Ve a la configuración de Miro Insights > sección de **Integraciones y Automatizaciones**.
2. Selecciona tu herramienta de conversación. Por ejemplo, Grain.
3. Inicia sesión en Zapier, si es necesario.
4. Conecta tu cuenta de Grain.
5. Mapea campos de Grain a campos de Miro Insights.
6. Prueba y activa la integración preconfigurada.

Las plantillas proporcionan una experiencia de configuración más rápida con mapeos de campo optimizados para cada herramienta específica, lo que facilita comenzar a capturar comentarios de los clientes de tus conversaciones grabadas.

### Configuración básica

1. **Crea un nuevo Zap** en tu panel de Zapier.
2. Elige tu **aplicación de disparo**. La herramienta de donde se originan los comentarios.
3. Selecciona **Miro Insights** como tu aplicación de acción.
4. Elige tu **evento de acción**:
   - **"Crear Comentario"** para elementos generales de comentarios.
   - **"Crear Comentario (Llamada)"** para comentarios específicos de llamadas.
5. Conecta tu **cuenta de Miro Insights** cuando se te solicite.
6. **Mapea los campos** de tu aplicación de activación a los campos de Miro Insights.
7. Prueba la integración para asegurarte de que los datos fluyan correctamente.
8. **Activa el Zap** para comenzar con la recolección de datos automatizada.

### Prácticas recomendadas para la creación de mapas de campos

Al mapear campos desde tu herramienta de origen a Miro Insights, considera las siguientes prácticas recomendadas para asegurar una captación de datos de alta calidad.

**Campos requeridos:**

- **Título de los comentarios**: Utiliza títulos claros y descriptivos de tus datos de origen.
- **Contenido**: Mapea el contenido principal de los comentarios o combina varios campos.

**Campos recomendados:**

- **Información del reportero**: Captura los datos de contacto del cliente cuando estén disponibles.
- **Datos de la empresa**: Esencial para la gestión de productos basada en cuentas.
- **URL de origen**: Mantén la trazabilidad hasta las fuentes originales.
- **Fecha proporcionada**: Usa la fecha real de los comentarios, no la fecha de procesamiento.

**Consejos para mapear campos:**

- Utiliza las herramientas de formato de Zapier para combinar múltiples campos de origen.
- Incluye el nombre de la herramienta de origen en el título o contenido para mayor claridad.
- Usa formatos consistentes para fechas, nombres de empresas y categorías.
- Configura valores predeterminados para los campos opcionales.
