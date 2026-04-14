---
title: Trae tu propia IA (BETA)
article_id: 21885197978642
translation_id: 21885197978642
locale: es
sidebar_position: 20
created_at: '2024-10-09T18:45:40Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: ai-generate-image
---

Trae tu propia IA (BYOAI) te habilita a utilizar tu propio proveedor de IA en lugar de Miro AI, para algunas funciones de Miro AI.

> **Disponible para:** Enterprise
> **Disponible en:** Escritorio

Puedes conectar tu proveedor de IA a Miro con BYOAI, y aprovechar [las funciones de IA que dependen de GPT](18-miro-ai-reference.md). Las funciones de Miro AI no deshabilitadas por BYOAI, como la generación de imágenes. Para más información, consulta Deshabilitar las funciones de IA que no funcionan con "Trae tu propia IA".

Actualmente, BYOAI soporta OpenAI y Azure OpenAI.

:::note
BYOAI sólo soporta las funciones de Miro AI con GPT. Para saber qué funciones de Miro AI funcionan con GPT, consulta [Visión general de Miro AI](18-miro-ai-reference.md).
:::

## Cómo configurar "Trae tu propia IA

> **Disponible para:** admins de empresa

Los siguientes procedimientos explican cómo configurar Trae tu propia IA (BYOAI) para Open AI, y Azure OpenAI.

### OpenAI

Sigue estos pasos:

1. En la configuración de admins, selecciona **Apps e integraciones**.
2. En **Integración empresarial**, para **Trae tu propia IA** selecciona **OpenAI**.
3. Para la **clave API**, introduce tu clave OpenAI.
   > ⚠️ Para mayor seguridad, copia y pega la clave API.
4. Selecciona **Conectar**.
5. Asegúrate de que tienes habilitada Miro AI en tu organización.
   Más información Consulta Habilitar Miro AI para Traer tu propia IA.

   Has configurado correctamente la BYOAI con OpenAI.

:::note
Miro utiliza un sistema de almacenamiento unidireccional para almacenar y encriptar de forma segura tu clave API, que nunca es visible durante la introducción de la clave. Ni Miro ni los admins pueden recuperar la clave API después de actualizarla y almacenarla de forma segura.
:::

### Azure OpenAI

Sigue estos pasos:

1. En la configuración de admins, selecciona **Apps e integraciones**.
2. En **Integración empresarial**, para **Trae tu propia IA** selecciona **Azure OpenAI**.
3. Introduce tu clave API de Azure, el nombre y la URL de despliegue.
   > ⚠️ Para mayor seguridad, copia y pega la clave API. Asegúrate de que la implantación utiliza GPT-4o.
4. Selecciona **Conectar**.
5. Asegúrate de que tienes habilitada Miro AI en tu organización.
   Más información Consulta Habilitar Miro AI para Traer tu propia IA.

   Has configurado correctamente la BYOAI con Azure OpenAI.

:::note
Miro utiliza un sistema de almacenamiento unidireccional para almacenar y encriptar de forma segura tu clave API, que nunca es visible durante la introducción de la clave. Ni Miro ni los admins pueden recuperar la clave API después de actualizarla y almacenarla de forma segura.
:::

### Habilita Miro AI para Trae tu propia IA

Después de haber conectado Open AI o Azure Open AI, asegúrate de que tienes habilitada Miro AI para tu organización.

Sigue estos pasos:

1. En la configuración de admins, selecciona **Acceso a funciones**.
2. En **Activación de funciones**, para **Miro AI** selecciona una de las siguientes opciones:
   - **Disponible para todos**
   - **Solo disponibles para equipos específicos**
3. (Opcional) **Habilita las funciones beta de Miro** AI en la posición de activado.

   Has habilitado correctamente Miro AI para tu organización.

:::note
Por defecto, todas las funciones de Miro AI están disponibles cuando habilitas Miro AI. Para deshabilitar las funciones de Miro AI no admitidas por tu proveedor de AI, ponte en contacto con el Soporte de Miro. Para saber más, consulta Deshabilitar las funciones de IA que no funcionan con IA propia.
:::

## Deshabilitar las funciones de la IA que no sean de Trae tu propia IA

Por defecto, todas las funciones de Miro AI están disponibles cuando habilitas Miro AI. Trae tu propia IA (BYOAI) sólo admite funciones LLM, que aprovechan GPT. Para asegurarte de que BYOAI utiliza sólo las funciones LLM que admite tu proveedor de IA, puedes deshabilitar opcionalmente las funciones no LLM de Miro AI.

Para deshabilitar las funciones de Miro AI que no sean LLM, ponte en contacto con tu gerente de Customer Success de Miro o con [Soporte de Miro](../tools/troubleshooting/06-contacting-miro-support.md).

Más información Ver [la visión general de Miro AI](18-miro-ai-reference.md).

## Preguntas frecuentes

**¿Quién es responsable de crear la salida de IA cuando utilizo la BYOAI?**

Con BYOAI, tú tomas el control de la generación de resultados con IA, con la calidad que hayas establecido con tu proveedor de IA.

**¿Cómo influye en la moderación de las aportaciones el hecho de aprovechar mi propio proveedor de IA?**

Con BYOAI, Miro no filtra el contenido antes de que tu proveedor de IA genere la salida. Si prefieres que se habilite la moderación, comprueba si tu proveedor ha habilitado la moderación de entradas y, a continuación, ponte en contacto con tu gerente de Customer Success o con [el Soporte de Miro](../tools/troubleshooting/06-contacting-miro-support.md).

**¿Cómo afecta la BYOAI al consumo de créditos de IA?**

Con BYOAI, consumes tokens de tu propio proveedor de IA para ejecutar las funciones de Miro AI. También sigues consumiendo créditos de Miro AI. Para más información, consulta [Créditos Miro AI para planes Enterprise](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md).

**¿Qué ocurre si mi clave API caduca o me quedo sin tokens?**

Como admins, verás un mensaje de error y los usuarios finales ya no podrán utilizar las funciones de IA de BYOAI.

**¿Cómo obtengo Soporte si tengo problemas con la integración de mi proveedor de IA?**

Ponte en contacto con tu gestor de éxito del cliente o con el servicio de atención al cliente. Te recomendamos que también te pongas en contacto con tu proveedor de AI.

**¿Utilizará Miro alguna entrada o salida si utilizo BYOAI?**

No, la entrada y salida de datos está sujeta al acuerdo que tengas con tu proveedor.
