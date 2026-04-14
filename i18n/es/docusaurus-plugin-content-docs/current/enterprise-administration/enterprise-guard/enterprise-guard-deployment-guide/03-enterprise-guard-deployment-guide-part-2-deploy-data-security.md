---
title: 'Guía de despliegue de Enterprise Guard - Parte 2: Despliega la seguridad de
  los datos'
article_id: 17121026396690
translation_id: 17121026396690
locale: es
sidebar_position: 2
created_at: '2024-02-19T09:32:48Z'
updated_at: '2025-11-25T15:41:10Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: api-security
availability:
  notes: 'Equipos relevantes: Algunos ejemplos de equipos con los que puedes tener
    que asociarte para implantar funciones de Seguridad de Datos son Protección de
    Datos, Prevención de Pérdida de Datos, Gobernanza y Riesgo, Seguridad de Aplicaciones,
    Información y Seguridad Digitales y/o Amenaza Interna.'
---

## Visión general de la seguridad de los datos

Encuentra, clasifica y protege el contenido sensible utilizando las funciones de Seguridad de Datos de Enterprise Guard.

- **Descubrimiento de datos:** Descubre datos sensibles como la Información Personal Identificable (IPI), la Información Personal de Salud (IPS) y los datos de la Industria de Tarjetas de Pago (PCI) con sólo unos clics.
- **Clasificación automática:** establece criterios para que Miro clasifique automáticamente tus tableros en función de los datos sensibles que contengan.
- **Barreras de protección inteligentes:** Aplica reglas de seguridad en tiempo real y restringe lo que los usuarios pueden hacer con un tablero basándote en la clasificación manual o automatizada del tablero.
- **Explorador de contenido:** Obtén una vista unificada de todos los tableros de Miro con contenido sensible y la clasificación de cada tablero.

![Enterprise Guard-Seguridad de datos.png](images/21016941885458_Enterprise-Guard-Data-Security.png)*Encuentra, clasifica y protege los datos sensibles*

## Resumen de la implantación

Este enfoque de despliegue da prioridad a la seguridad de los datos sensibles encontrados mediante el Descubrimiento de Datos de Enterprise Guard, al tiempo que minimiza la interrupción de la actividad de los usuarios finales.

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="390" scrolling="no" src="https://miro.com/app/live-embed/uXjVNrjv8h8=/?moveToViewport=-3966,-1331,10269,3273&amp;embedId=881755370090" width="690"></iframe> *Descripción general de la implantación de Enterprise Guard*

#### Pasos para la configuración

1. Auditar datos sensibles
2. Ajustar los parámetros de clasificación
3. Publicar la clasificación
4. Despliega las barreras de protección
5. Afloja las restricciones de la manta

#### Pasos de comunicación y habilitación del usuario final

1. Crea un plan de despliegue
2. Anuncio inicial de Enterprise Guard
3. Anuncio de despliegue de clasificaciones
4. Resolver la aparición innecesaria de datos sensibles
5. Anuncio de despliegue de las barreras de protección

## Auditar datos sensibles

Completa la auditoría descrita en esta sección lo antes posible en tu despliegue de Enterprise Guard. No afecta en absoluto a los usuarios finales, pero te permitirá evaluar el alcance y la gravedad de los casos de datos sensibles en tu instancia de Miro.

Utiliza los resultados de la auditoría para crear un plan de implantación que equilibre la gestión de cambios de los usuarios finales con las políticas de seguridad de tu organización.

### Activa el descubrimiento de datos

El primer paso para configurar tu marco de clasificación de datos es habilitar el Descubrimiento de datos en tu cuenta de Miro. A continuación, Miro escaneará todos tus tableros en busca de datos sensibles según la Región y/o las Políticas de Regulación de la Privacidad (etiquetas) habilitadas.

[Cómo habilitar el descubrimiento de datos en tu entorno Miro](../../canvas-25-admin-features/data-discovery/13-activate-privacy-related-data-discovery.md)

Los contenidos sensibles pueden tardar hasta 24 horas en ser detectados. Una vez que Miro ha identificado el contenido sensible que coincide con estas etiquetas de sensibilidad (es decir, GDPR, PCI), se puede utilizar el Explorador de contenido para revisar los resultados con más detalle.

### Auditoría con el Explorador de contenido

El explorador de contenido ofrece a los admins de contenido sensible una forma de revisar las incidencias de datos sensibles descubiertas por Miro Enterprise Guard, revelando dónde se han producido (nombre del tablero), quién es el actor (propietario del tablero), por qué se ha marcado la incidencia (etiqueta) y cuál es el contenido.

Utiliza los filtros del explorador de contenido, como "Clasificación = Confidencial", para centrarte en las apariciones más importantes de datos sensibles.

## Crea un plan de despliegue

Una vez habilitado el descubrimiento de datos y revelados los casos de contenido sensible, es hora de crear un plan de despliegue de clasificaciones y barreras de protección de acuerdo con las políticas de tu organización, los requisitos, la gravedad de los hallazgos y los recursos disponibles. En las secciones siguientes se sugieren las mejores prácticas de comunicación para informar a los usuarios finales y apoyar tu proceso de gestión del cambio.

### Anunciar los próximos cambios

Antes de publicar tu marco de clasificación en Miro, se recomienda informar a los usuarios de la decisión de tu organización de habilitar Enterprise Guard en todo el contenido de Miro, y proporcionar el contexto de acuerdo con las políticas y prácticas de seguridad de datos de tu organización.

Considera la posibilidad de incluir la siguiente información:

- Qué es Enterprise Guard
- Por qué es importante para tu organización
- Visión general de los aspectos de la experiencia del usuario final que se verán afectados
- Explicación del marco de clasificación de tu organización
- Qué políticas de regulación de datos se incluirán en el descubrimiento de datos
- Cronograma de los próximos cambios
- Dónde dirigirse con preguntas y comentarios

## Ajustar los parámetros de clasificación

### Añadir marco de clasificaciones

El establecimiento de clasificaciones de datos en Miro está diseñado para ser flexible y adaptable a cualquier marco de clasificación de datos existente en tu organización.

Los niveles de clasificación en Miro mostrarán su orden de sensibilidad actual. Haz coincidir el orden de sensibilidad con la jerarquía de clasificación de tu organización, donde el orden de sensibilidad 1 es el nivel de clasificación menos sensible.

[Cómo configurar las Clasificaciones](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md)

### Aplanar los marcos de clasificación

La estructura de clasificación de Miro Enterprise Guard está diseñada para adaptarse a tu política de clasificación de datos existente.

Si el marco de clasificación existente en tu organización tiene más de un nivel de jerarquía (como niveles de subclasificación o etiquetas), puede ser necesario aplanar tu marco de clasificación. El ejemplo siguiente muestra un marco de clasificación con 3 etiquetas que necesitaría 3 niveles de clasificación distintos por etiqueta y por nivel.

Se recomienda reducir al mínimo los niveles de clasificación.

![Enterprise-Guard-Aplanar la jerarquía de clasificación.pngAplanar los](images/21016941886226_Enterprise-Guard-Flatten-Classification-Hierarchy.png)
*marcos de clasificación*

### Enlazar documentación y escribir descripciones

Unas descripciones y directrices de clasificación claras informarán a tus usuarios finales sobre la política de clasificación, a escala. Mientras los usuarios finales estén en el tablero, aparecerán descripciones de la clasificación junto a la etiqueta de clasificación. Los usuarios finales verán un signo de interrogación "más información" en cada panel que enlaza con la documentación de clasificación.

|  |  |
| --- | --- |
| **Descripción de la clasificación** | Cuando los usuarios hacen clic en la insignia de clasificación del tablero, aparece la descripción del nivel de clasificación actual.  Añade una descripción significativa que informe a tus usuarios sobre la sensibilidad de este tablero y las precauciones o acciones recomendadas.  Clasificación-descripción.png |
| **Enlace a los lineamientos** | Cuando el usuario hace clic en el icono de más información (icono de interrogación) situado junto a la insignia de clasificación del tablero, esta URL se carga en una nueva pestaña del navegador.  Proporciona a tus usuarios más información sobre los niveles de clasificación de tus tableros y cómo trabajar con ellos.  Considera la posibilidad de incluir:   - Qué es Enterprise Guard - Por qué es importante para tu organización - Visión general de los aspectos de la experiencia del usuario final que se verán afectados - Explicación del marco de clasificación de tu organización - Qué políticas de regulación de datos se incluirán en el descubrimiento de datos - Dónde dirigirse con preguntas y comentarios |

### Definir criterios de autoclasificación

Miro aplicará las clasificaciones automáticamente a los tableros en los que se detecte contenido que coincida con la normativa de privacidad correspondiente. Cada nivel de clasificación puede vincularse a varias [etiquetas de Sens](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md) ibilidad, pero cada etiqueta de Sensibilidad sólo puede vincularse a un único nivel de clasificación.

Si se cumplen varios criterios, se aplicará el nivel de clasificación más sensible.

[Cómo definir Autoclasificaciones](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md)

### Configuración de las barreras de protección Skip

Como ya se ha dicho, esta guía pretende dar prioridad a la gestión del cambio del usuario final, además del despliegue de Enterprise Guard. Recomendamos publicar clasificaciones sin barreras de protección. La clasificación de los tableros en esta configuración será un indicador visual, pero no afectará a la experiencia del usuario final.

Antes de añadir barreras de protección a las clasificaciones, resuelve los casos innecesarios de datos sensibles y pasa a los usuarios a la clasificación manual para garantizar una transición fluida sin interferir en el trabajo crítico que se realiza en los tableros.

### Configura las barreras de protección para las clasificaciones más altas

Utilizando las conclusiones de tu auditoría inicial, puedes decidir desplegar barreras de protección sin demora. Considera la posibilidad de aplicar barreras de protección sólo a las clasificaciones más sensibles. Esto equilibra la urgencia de proteger los datos sensibles sin afectar a la gran mayoría de los usuarios finales.

## Publicar la clasificación

Antes de publicar autoclasificaciones, tendrás la oportunidad de revisar su impacto para tus usuarios finales. Si has configurado los niveles de clasificación sin barreras de protección, no habrá un impacto sustancial para los usuarios finales cuando publiques.

[Cómo publicar Clasificaciones](https://help.miro.com/hc/articles/16494764223378-Review-impact)

### Anuncio de clasificación

Después de publicar las clasificaciones, envía un anuncio a tus usuarios finales.

Considera la posibilidad de incluir la siguiente información:

- Una breve reseña de Enterprise Guard o consulta el anuncio anterior
- Visión general de los aspectos de la experiencia del usuario final que se verán afectados
- Explicación del marco de clasificación de tu organización
- Qué políticas de regulación de datos se incluirán en el descubrimiento de datos
- Cronograma de los próximos cambios
- Dónde dirigirse con preguntas y comentarios

## Resolver la aparición innecesaria de datos sensibles

Antes de liberar las barreras de protección inteligentes, recomendamos comunicarse con los propietarios de tableros cuyos tableros contengan información sensible. Es posible que los datos sensibles sean involuntarios y puedan eliminarse.

Informa a los usuarios de que pronto se implantarán barreras de protección inteligentes de acuerdo con las políticas de seguridad de tu organización. Tus usuarios finales pueden aprovechar la oportunidad para eliminar datos sensibles innecesarios de sus tableros y evitar interrupciones en su trabajo.

## Usuarios a bordo a clasificación manual

Incluso con la clasificación automática habilitada, muchos tableros permanecerán sin clasificar o en la clasificación por defecto si no son reclasificados manualmente por los usuarios finales.

### Clasificación manual Experiencia del usuario final

[El propietario del tablero,](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) [los copropietarios del tablero](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), los editores miembros del equipo y los admins de empresa con permisos de admins de contenido pueden actualizar la etiqueta de clasificación haciendo clic en la insignia de clasificación o desde los detalles del tablero. Selecciona una nueva etiqueta y haz clic en Actualizar.

Al ajustar las clasificaciones inferiores en el orden de sensibilidad (por ejemplo, de Confidencial a Público), los usuarios deberán proporcionar una justificación que se registra en los registros de auditoría de tu cuenta de Miro.

### Comunicación con el usuario final

Tras el despliegue inicial de Enterprise Guard, se recomienda enviar comunicaciones periódicas a los usuarios finales que fomenten el uso de clasificaciones en cada tablero. Esto garantizará que se utiliza el conjunto completo de barreras de protección y clasificaciones y, por tanto, aumentará la seguridad de tu instancia de Miro.

Considera la posibilidad de incluir la siguiente información:

- Un recordatorio para clasificar los tableros con regularidad
- Instrucciones para clasificar los tableros
- Información sobre la justificación
- Vídeo | Clasificación de tableros para usuarios finales (puedes insertar enlaces más abajo)

<iframe allowfullscreen="" frameborder="0" height="315" src="//fast.wistia.com/embed/iframe/3ado2k4f6c" width="560"></iframe>
*Clasificación de tableros en Miro*

### Recursos

- Vídeo | Clasificaciones de tableros para usuarios finales
  - [Enlace Wistia](https://mirohq.wistia.com/medias/3ado2k4f6c)
  - Insertar código
    - ```
      <script src="https://fast.wistia.com/embed/medias/3ado2k4f6c.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_3ado2k4f6c seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/3ado2k4f6c/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>
      ```

## Despliega las barreras de protección restantes

En este punto, los usuarios finales deberían haber tenido tiempo suficiente para comprobar sus tableros en busca de datos sensibles innecesarios, y ajustar manualmente sus clasificaciones de tableros.

[Cómo desplegar barreras de protección inteligentes](../../canvas-25-admin-features/data-classification/05-define-guardrails.md)

> ⚠️ Ten cuidado al aplicar barreras de protección a la clasificación por defecto de los tableros. Aplicar barreras de protección a la clasificación por defecto tendrá un impacto significativo en los usuarios finales , porque muchos tableros tendrán la clasificación por defecto.

### Anuncio de las barreras de protección

Después de publicar las barreras de protección, envía un aviso a tus usuarios finales.

Considera la posibilidad de incluir la siguiente información:

- Una referencia a anuncios anteriores sobre Enterprise Guard
- Qué son las barreras de protección
- Una visión general de las clasificaciones y sus barreras de protección asociadas
- Cómo ajustar manualmente las clasificaciones
- Dónde dirigirse con preguntas y comentarios

## Afloja las restricciones de colaboración de Blanket

Enterprise Guard te permite desplegar controles específicos. Sin embargo, antes de Enterprise Guard no había tantas opciones para adaptar los controles a casos concretos. Lo más probable es que el resultado fueran "controles generales", es decir, ajustes preventivamente estrictos que se aplican a la mayoría de tableros y que, por tanto, añaden fricción a la colaboración de tus usuarios de Miro.

Aplicar controles generales, como bloquear la colaboración externa para todos los usuarios y tableros, carece de precisión. Los usuarios pueden experimentar fricciones cuando el contenido en el que están colaborando no es sensible y puede bloquear casos de uso enteros de Miro.

En definitiva, los controles generales pueden afectar al ROI que obtienes de Miro, pero ahora con Enterprise Guard, tus usuarios finales pueden obtener más valor de Miro al tiempo que se aseguran de que el contenido sensible está protegido. Tendrás que reevaluar algunos ajustes de tu cuenta para aprovechar al máximo las ventajas de Enterprise Guard.

*Aflojar las restricciones de los tableros*

### Otras configuraciones vs Enterprise Guard

En Miro, hay 3 áreas de configuración que trabajan juntas para determinar la experiencia real del usuario.

- Ajustes en el ámbito de la empresa
- Ajustes a nivel del equipo
- Enterprise Guard

Siempre que haya configuraciones contrapuestas, se aplica la más estricta. Consulta aquí más información.

### Ajustes relevantes y dónde encontrarlos

Tendrás que reevaluar algunos ajustes para asegurarte de que Miro está configurado de forma integral. Aquí tienes una lista de ajustes relevantes y dónde encontrarlos en tu cuenta de Miro. Algunos ajustes pueden controlarse tanto desde el nivel de empresa como desde el nivel de equipo.

Recuerda, si dos ajustes se aplican a la misma parte de la experiencia Miro, el ajuste más estricto dictará la experiencia.

|  |  |  |
| --- | --- | --- |
| **Configuración** | **Descripción** | **Dónde está disponible** |
| Enlaces públicos | Un enlace público permite acceder a un tablero sin necesidad de identificarse. Puede configurarse para ver, comentar o editar el acceso y requerir una contraseña. | Nivel de empresa  Nivel del equipo  Enterprise Guard |
| inserción | Controla si y cómo los usuarios pueden insertar tableros de Miro en otro software o sitios web. | Nivel de empresa |
| Configuración de invitados | Un invitado es un usuario invitado sólo a un tablero y no a todo un equipo o a una cuenta. | Nivel de empresa  Nivel del equipo |
| Uso compartido del tablero | Controla cómo se pueden compartir los tableros con otros usuarios de la cuenta, en y entre equipos. | Nivel del equipo  Enterprise Guard |
