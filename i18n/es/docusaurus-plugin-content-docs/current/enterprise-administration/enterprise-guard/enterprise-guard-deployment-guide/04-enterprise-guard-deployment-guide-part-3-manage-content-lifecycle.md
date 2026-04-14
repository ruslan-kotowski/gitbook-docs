---
title: 'Guía de implantación de Enterprise Guard - Parte 3: Gestionar el ciclo de
  vida del contenido'
article_id: 17121851926546
translation_id: 17121851926546
locale: es
sidebar_position: 3
created_at: '2024-02-19T10:01:34Z'
updated_at: '2025-11-25T15:41:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
availability:
  notes: 'Equipos relevantes: ** Algunos ejemplos de equipos con los que puedes tener
    que asociarte para implantar las funciones del ciclo de vida del contenido son
    GRC (gobernanza, riesgo, cumplimiento), Gestión del Cumplimiento, Legal y/o Gestión
    de Registros.'
---

## Visión general de la gestión del ciclo de vida del contenido

En la mayoría de las empresas, los contenidos crecen exponencialmente, tanto en volumen como en complejidad. La gestión y el gobierno adecuados de los tableros de Miro son fundamentales por múltiples razones, entre ellas:

- Cumplir de forma proactiva las normativas específicas del sector o las directrices internas de la organización
- Minimizar el riesgo en situaciones como disputas legales o violaciones de la seguridad
- Mantener la eficacia organizativa

Actualmente soportamos las siguientes funciones:

- [Políticas papeleras](https://help.miro.com/hc/articles/13860817985426-Trash-Policy)
- [Políticas de retención](https://help.miro.com/hc/articles/16855776325778-Retention-policies)

## Visión general de la implantación de la gestión del ciclo de vida del contenido

Mientras que el proceso recomendado de [Parte 2: Despliega la Seguridad de Datos](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md) incluye la configuración progresiva y la comunicación con el usuario final, la Gestión del ciclo de vida del contenido no.

Es probable que ni las políticas de Papelera ni las de Retención interrumpan la actividad de los usuarios finales en Miro, por lo que pueden configurarse inmediatamente.

## Despliega una Política Global de Retención

Actualmente, Enterprise Guard sólo admite una política de retención global. En el futuro estarán disponibles otras opciones de configuración que ofrecerán mayor flexibilidad. Considera los requisitos normativos de tu sector y las políticas organizativas para determinar cuál debe ser la duración de tu política global de retención.

Como no se dispone de mayor granularidad, puede ser beneficioso configurar tu política de retención global para que coincida con el requisito de mayor duración previsto por tu organización. Por ejemplo, si determinados contenidos de Miro deben conservarse durante 5 años debido a un requisito normativo, tu política de retención global debe establecerse en 5 años.

Puedes reducir el alcance de los tableros mantenidos bajo esta política de retención de 5 años más adelante, a medida que Miro publique ámbitos de retención más granulares, como el nivel de clasificación o el equipo.

[Cómo configurar las políticas de retención](https://help.miro.com/hc/articles/16855776325778-Retention-policies)

## Configurar la política de papelera

Por defecto, los tableros de Miro se eliminan automática y permanentemente de la papelera después de 90 días. Puedes actualizar la configuración por defecto y elegir eliminar tableros de la papelera de forma automática y permanente en 30, 60, 90 ó 180 días.

Cuando actualizas el periodo de borrado automático y permanente de tableros, el periodo actualizado sólo se aplica a los tableros que se mueven de nuevo a la Papelera. Los tableros deben ser movidos manualmente a la papelera por los propietarios o copropietarios del tablero.

Cuando un tablero está en la Papelera pero no ha finalizado el periodo de borrado, determinados usuarios pueden borrar manual y permanentemente los tableros. Elige quién puede hacerlo en la configuración de la papelera entre propietarios de tableros o admins.

[Cómo configurar las políticas de papelera](https://help.miro.com/hc/articles/13860817985426-Trash-settings)

## Trabajo conjunto de retención y papelera

Las políticas de retención anulan las políticas de papelera y borrado manual y permanente. Consulta los ejemplos y el diagrama siguientes.

Ejemplos

- Si el propietario de un tablero lo mueve a la Papelera y lo elimina manualmente de forma permanente, pero el tablero está sujeto a una política de retención, el tablero se conservará. Al final del periodo de retención, el tablero se eliminará de forma inmediata y permanente.
- Si un tablero se mueve a la Papelera y el periodo de borrado permanente finaliza, pero el tablero está bajo una política de retención, el tablero se conservará. Al final del periodo de retención, el tablero se eliminará de forma inmediata y permanente.

![Enterprise Guard-Políticas.pngRetención](images/21017043241234_Enterprise-Guard-Trash-Policies.png)
*y papelera trabajando juntas*
