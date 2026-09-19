---
name: jurisdiccion
description: Lente para delimitar autoridad de decisión en agentes, automatizaciones y procesos delegados. Úsala al definir límites de autonomía o escalado, o al investigar decisiones que cumplieron una regla pero excedieron el mandato. No se activa por cualquier tarea de programación o automatización.
---

# Jurisdicción

Una lente, no un método. Nace de [Sedimento](https://carlesmontrull.me/essays/sedimento), con el rechazo de una oferta estratégica por un agente operativo en una cafetería ficticia, y de [La instancia](https://carlesmontrull.me/essays/la-instancia), que explora organizaciones operadas por agentes. Son una prueba exploratoria y un escenario de futuro, no una frontera universal de delegación.

## La idea que sostiene la lente

Poder ejecutar una decisión y estar autorizado para tomarla son preguntas distintas. La **jurisdicción** delimita qué puede decidir el sistema, bajo qué condiciones y quién responde cuando el caso sale de ellas.

Una regla operativa puede cubrir la letra de una decisión cuya consecuencia excede su mandato. Un sistema puede también tener una delegación suficiente y funcionar bien: añadir una aprobación no mejora automáticamente ese reparto.

La frontera se diseña a partir de consecuencias, capacidad y autoridad. Debe permitir actuar dentro del mandato y reconocer el punto donde actuar requeriría otro.

## Cómo aplicar la lente

Parte del sistema, su mandato y las decisiones que toma. Usa los responsables y límites ya definidos; pide solo lo que falte para juzgar la delegación. Consulta los ensayos si necesitas apoyar una conclusión en un detalle de sus casos; si no puedes acceder, no lo presentes como verificado.

**1. Mapa de decisiones.** Separa tareas de elecciones con consecuencias. "Enviar el email" puede ejecutar una decisión ya tomada; escoger destinatario, condiciones o compromisos puede introducir otras. Identifica qué autoridad se ha delegado y qué parte estás proponiendo, sin confundir propuesta con permiso vigente.

**2. Los cuatro tests.** Para cada decisión relevante:

- *Reversibilidad*: qué puede deshacerse, en cuánto tiempo y con qué consecuencias residuales.
- *Visibilidad*: qué registro permite detectar y revisar el error, y quién lo mira a tiempo.
- *Alcance*: qué personas, relaciones o recursos quedan afectados fuera de lo observado por el sistema.
- *Excepcionalidad*: qué condiciones definen un caso conocido y qué señal indica que dejó de serlo.

Los tests requieren contexto, no una suma automática de puntuaciones. Una consecuencia reversible puede exceder el mandato; una irreversible puede estar expresamente autorizada dentro de condiciones precisas.

**3. Trazar la frontera.** Reparte las decisiones con una razón concreta:

- **Propias**: el mandato y las condiciones observables bastan para ejecutar con los controles habituales.
- **De borde**: sigue existiendo autorización para ejecutar, pero se activa un aviso y revisión definidos. Explica por qué esa revisión posterior llega a tiempo.
- **Ajenas**: quedan fuera del mandato o requieren una decisión previa que el sistema no puede suplir. Detiene esa decisión y la remite al responsable designado.

Si un aviso posterior no protege lo que está en juego, no lo uses como sustituto de la aprobación previa. No es necesario llenar las tres zonas. Si falta el mandato, la clasificación queda provisional. Para el escalado identifica destinatario, suplencia y conducta mientras no responda; no inventes nombres ni amplíes autoridad por silencio. Mantén el reparto actual si está justificado.

**4. El test del evaluador.** Examina si se puede mejorar la métrica perjudicando el propósito. Describe el mecanismo plausible y distingue un incentivo de una conducta observada. Si existe, valora qué combinación de límites, evaluación y supervisión lo aborda. Contrasta también si un incidente procede de un fallo de ejecución dentro de un mandato correcto: restringir autoridad no corrige necesariamente ese fallo.

## Formato de salida

Un acta breve, en prosa. Desarrolla solo lo que el caso permita; si la lente no aplica o falta evidencia decisiva, explica el límite y cierra con la pregunta pertinente, sin completar apartados ficticios:

- Las zonas y sus condiciones, distinguiendo mandato vigente, propuesta y datos pendientes.
- Los límites operativos que se deben mantener o cambiar y las señales que los activan. Puede no haber nuevas restricciones.
- El posible conflicto entre métrica y propósito, si se encuentra, y su evidencia.
- Para cada escalado necesario, destinatario, suplencia y conducta de espera; señala las designaciones pendientes. Incluye qué evidencia cambiaría una frontera discutible.
- Si hay un hallazgo fuera de su alcance, una derivación a las otras lentes: qué parte del hallazgo ya no es de jurisdicción sino de otra — reglas heredadas que nadie revisó a `/sedimento`, defensibilidad o foso a `/instancia`, un problema más grande que la institución a `/escala`, sucesiones, relevos o dependencia de una persona clave a `/sede-vacante`, variables prohibidas que se cuelan por proxies heredados a `/codigo` — señalada, sin desarrollarla.
- La pregunta que cierra el acta pide resolver la frontera pendiente, designar a quien recibe el escalado o identificar qué cambio haría revisar un reparto hoy adecuado. No presupongas que haya que devolver decisiones a una persona. No es un ofrecimiento de profundizar ni un "¿quieres que siga?".

Tono: operativo. Esto se escribe para pegarlo en un prompt, en una política o en un contrato. El acta termina en esa pregunta; no se ofrece a continuar.

## Cuándo desconfiar de esta lente

Se formó con escenarios de agentes en negocios pequeños. Funciona peor cuando:

- La tarea ya está completamente decidida y autorizada, sin discreción pendiente. No añadas aprobaciones por el simple hecho de automatizarla.
- El problema son reglas caducadas: considera `/sedimento` antes de restringir a quien las ejecuta.
- Se busca acreditar cumplimiento normativo. La lente propone un reparto operativo; no lo certifica.

Toda frontera escrita envejece. Explicita qué cambio de mandato, consecuencias o capacidad obligaría a revisarla. La intervención humana también puede fallar o llegar tarde.
