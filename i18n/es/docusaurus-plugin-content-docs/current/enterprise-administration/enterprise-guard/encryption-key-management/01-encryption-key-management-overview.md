---
title: "Descripci\xF3n general de la gesti\xF3n de claves de cifrado"
article_id: 14634334255250
translation_id: 14634334255250
locale: es
sidebar_position: 0
created_at: '2023-10-24T14:24:53Z'
updated_at: '2026-02-05T15:17:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

El complemento Enterprise Guard incluye una opción para la gestión de claves de cifrado (EKM). La EKM proporciona control centralizado sobre las claves de cifrado para ayudar a proteger tus datos. Esta solución basada en la nube habilita la supervisión de los registros de actividad asociados a las claves de cifrado y permite revocar el acceso de las claves a tus datos.

Para obtener un control y visibilidad adicionales sobre cómo se utilizan las claves de cifrado en Miro, también puedes utilizar Bring Your Own Key (BYOK). Con BYOK, gestionas el cifrado de los datos de tu organización dentro de la plataforma Miro.

## Experimenta las ventajas de la gestión de claves de cifrado

- **Implementación sin Problemas:** Integra sin esfuerzo EKM en tu sistema, sin necesidad de instalación de hardware ni mantenimiento, gracias a su solución 100% basada en la nube.

- **Control Total de Acceso a Claves:** Disfruta de total autoridad sobre tus claves de cifrado. Tienes la posibilidad de revocar tu clave, haciendo que todos los datos cifrados sean inaccesibles tanto para Miro como para los usuarios finales.

- **Visibilidad Mejorada de Acceso:** Obtén información sobre actividades relacionadas con las claves con visibilidad de acceso. Monitoriza y rastrea los registros a través de AWS CloudTrail para conocer a fondo el uso de tu clave de cifrado.

![Enterprise Key Management Diagram](images/21016121487634_EKM.png)

## ¿Cómo protege EKM los datos de los clientes?

Miro proporciona EKM ofreciendo el cifrado de tus Datos de producción y Datos de copia de seguridad en reposo mediante la clave de cifrado personalizada, mientras que el cliente concede a Miro acceso a la clave de cifrado personalizada. Miro respalda EKM con una clave alojada en tu propia cuenta de AWS a través de AWS KMS. Con EKM, obtienes una mayor visibilidad de auditoría y un mayor control de acceso a los datos (contenido generado por el usuario), como formas, widgets y archivos cargados.

## Cifrado de datos en Miro

Garantizar la máxima seguridad de tus datos es una preocupación primordial en Miro. Por defecto, empleamos medidas de cifrado para los datos de los clientes, tanto en tránsito como en reposo, independientemente de su plan de suscripción. Cuando accedes a Miro a través de Internet, tus datos gozan de protección mediante cifrado TLS 1.3 y certificados PKI emitidos por Amazon Web Services (AWS). Al llegar a nuestros servidores, tus datos se protegen aún más mediante el cifrado AES-256 en reposo, utilizando claves gestionadas por Miro a través de AWS Key Management Service. [Más información sobre la seguridad en Miro.](https://miro.com/trust/security/)

> Nota: Tú eres el único responsable de la seguridad y protección de todos y cada uno de los datos de copia de seguridad que descargues o transfieras a tus sistemas o a los de terceros. Tú eres el único responsable de la clave de cifrado personalizada. Si pierdes tu clave de cifrado personalizada, Miro no puede ayudarte a recuperar el acceso a los datos. Una vez que tus datos de producción o datos de copia de seguridad estén en tránsito o fuera del control de Miro, Miro no puede garantizar su protección.

## ¿Cómo habilito la gestión de claves de cifrado?

Configurar e implementar la gestión de claves de cifrado requiere la ayuda de los equipos internos de Miro. Si necesitas ayuda, ponte en contacto con tu representante de Miro o [solicita asistencia a través del equipo de Soporte de Miro aquí](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).

## Glosario

- **Backup Data:** Una instantánea de tu contenido creado o enviado al servicio Miro que Miro almacena para su recuperación y otros fines.

- **Clave de Cifrado Personalizada:**  Una clave de seguridad única, personalizada e implementada por ti, que los individuos necesitan para acceder a tus datos de Producción y Datos de Copia de Seguridad.

- **Datos de Producción:** Todos los datos a los que tú y tus usuarios acceden durante el uso y funcionamiento diario de los servicios de Miro.
