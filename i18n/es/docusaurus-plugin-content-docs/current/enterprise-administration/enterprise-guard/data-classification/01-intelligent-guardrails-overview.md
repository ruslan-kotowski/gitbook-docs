---
title: "Descripci\xF3n general de las barreras de protecci\xF3n inteligentes"
article_id: 14375998880018
translation_id: 14375998880018
locale: es
sidebar_position: 0
created_at: '2023-10-12T12:35:03Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Los elementos del tablero de Miro pueden contener datos de privacidad y regulación (como información de identificación personal, información de salud protegida, PCI) o contenido confidencial crítico para el negocio (como información financiera, información de recursos humanos, propiedad intelectual, secretos comerciales). Después del descubrimiento y la clasificación automática de datos, las organizaciones deben implementar controles proactivos que son cruciales para mantener la privacidad, seguridad y el cumplimiento sostenidos de las regulaciones relevantes.

- Con las barreras de protección, ahora puedes aplicar automáticamente controles proactivos, como:
  Restringir automáticamente las capacidades de compartición a varios niveles (público, equipo, organización) basándose en el contenido del tablero y el nivel de clasificación.
- Restringir la replicación de contenido.
- Bloquear el uso de Miro AI para prevenir interacciones impulsadas por IA con datos sensibles o clasificados.

Estos controles proactivos garantizan la privacidad y el cumplimiento sin interferir en las operaciones empresariales.

Los administradores tienen dos opciones para implementar las barreras de protección de Miro en su organización:
- **Modo predeterminado:** De forma predeterminada, las barreras de protección no afectan las opciones de compartición activas de los tableros para evitar interrumpir la colaboración en curso, incluso cuando los tableros son reclasificados durante la auto-clasificación.

- **Modo estricto:** Cuando el interruptor **Aplicar barreras de protección en modo estricto** está activado, las barreras de protección anulan todas las opciones de compartición activas. Esto proporciona a los administradores el nivel más estricto de control, pero también puede resultar en que algunos usuarios pierdan acceso al tablero de inmediato.

Considera un escenario en el que has configurado barreras de protección para asegurar que los usuarios de tableros clasificados como CONFIDENCIAL no puedan compartir el tablero con el público, con equipos, con la organización, ni replicar contenido. Alguien en tu organización creó un nuevo tablero llamado Plan Financiero, añadió algunos números de ingresos y asignó el nivel de *CONFIDENCIAL* para este tablero. Las configuraciones de barreras de protección se aplican automáticamente y todos los usuarios no pueden compartir el tablero y todos los usuarios excepto el propietario del tablero no pueden replicar contenido (Figura 2).

Para obtener más información sobre cada barrera de protección, sus descripciones y los usuarios afectados, consulta la [documentación de referencia de barreras de protección](02-guardrails-reference.md).
