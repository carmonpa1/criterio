---
name: sedimento
description: Lente de análisis para auditar qué reglas ha heredado un sistema (empresa, producto, equipo, proceso, espacio) y cuáles se ejecutan sin el criterio que las creó. Úsala siempre que el usuario pida revisar "cómo funciona" algo que ya existe, detectar reglas que nadie recuerda por qué están, preparar un handoff o documentación de cultura, diagnosticar por qué un equipo o un agente "sigue las normas pero decide mal", o cuando mencione herencia, tradición, "siempre se ha hecho así", playbooks, SOPs, onboarding o codificar la cultura de una organización. Aplica también a sistemas de IA: prompts de agentes, reglas de automatización, políticas codificadas.
---

# Sedimento

Una lente, no un método. Nace del ensayo *Sedimento* (carlesmontrull.me/essays/sedimento), donde dos agentes de IA ejecutaron impecablemente las reglas de dos negocios reales — y uno de ellos rechazó una oportunidad porque la norma lo decía, sin saber que esa decisión no era de su tamaño.

## La idea que sostiene la lente

Toda regla escrita es el ayer de un criterio. Alguien decidió algo, por unas razones, en un contexto; la regla es lo que quedó cuando esas razones se secaron. La cultura de un sistema es ese sedimento: capas de decisiones repetidas hasta volverse norma.

El sedimento **se puede codificar**. Lo que no se puede codificar es el criterio que sabe cuándo la regla deja de aplicar. Un sistema que ejecuta el sedimento sin el criterio hace lo correcto casi siempre — y en el caso que importa, ejecuta impecablemente una decisión que no le pertenecía.

Por eso esta lente no pregunta "¿qué reglas tiene el sistema?" sino **"¿qué reglas siguen ejecutándose sin su expediente?"**

## Cómo aplicar la lente

Pide al usuario el material del sistema (documentación, reglas, prompts, observaciones, o simplemente que lo describa). Después, en este orden:

**1. Inventario del sedimento.** Lista las reglas operativas del sistema — explícitas (escritas) e implícitas (las que se deducen de cómo actúa). Formúlalas como reglas de decisión: "cuando X, se hace Y". No juzgues todavía.

**2. Excavación: el caso de origen.** Para cada regla, intenta recuperar el caso que la engendró: qué pasó, cuándo, qué protegía. Clasifica:
- **Con expediente**: se conoce el origen y sigue vigente.
- **Con expediente caducado**: se conoce el origen, pero las condiciones cambiaron.
- **Sin expediente**: nadie recuerda por qué existe. Se ejecuta por inercia.

Las reglas sin expediente son el hallazgo principal. No son necesariamente malas — son las que nadie puede discutir, porque no queda nada a lo que volver.

**3. El test de jurisdicción.** Para las reglas más consecuentes, pregunta: ¿qué decisión es de un tamaño que esta regla no debería tomar sola? ¿Hay un caso plausible en que aplicarla impecablemente sea el error? Si un agente, un empleado nuevo o un proceso automático la ejecutara al pie de la letra, ¿dónde haría daño?

**4. Distinguir regla de criterio.** Señala qué parte del comportamiento del sistema es sedimento (codificable, transferible, automatizable) y qué parte es criterio (vive en personas concretas, se aprende por exposición, no viaja en un documento). Esta frontera es lo más útil que entregas: dice qué se puede delegar y qué no.

## Formato de salida

Un acta breve, en prosa, sin encabezados grandilocuentes:

- Las reglas encontradas, con su clasificación (con expediente / caducado / sin expediente).
- Las dos o tres reglas donde un ejecutor perfecto haría daño, y por qué.
- La frontera propuesta entre lo que se puede codificar y lo que necesita una persona con criterio.
- Una derivación a las otras lentes: qué parte del hallazgo ya no es de sedimento sino de otra — defensibilidad o foso a `/instancia`, un problema más grande que la institución a `/escala`, decisiones que un sistema automático no debería tomar a `/jurisdiccion`, sucesiones, relevos o dependencia de una persona clave a `/sede-vacante`, variables prohibidas que se cuelan por proxies heredados a `/codigo` — señalada, sin desarrollarla.
- La pregunta que cierra el acta, dirigida al usuario y que él tiene que responder: qué caso de origen puede recuperar él que tú no puedes. No es un ofrecimiento de profundizar ni un "¿quieres que siga?".

Tono: declarativo, concreto, sin moralizar. Las reglas sin expediente se señalan, no se ridiculizan — casi siempre protegieron algo real. El acta termina en esa pregunta; no se ofrece a continuar.

## Cuándo desconfiar de esta lente

Esta lente se formó analizando negocios pequeños con reglas tácitas y agentes que las ejecutaban. Funciona peor cuando:

- El sistema es muy nuevo y no ha sedimentado nada todavía (no hay capas que excavar; usa `/instancia`).
- El problema es de escala, no de herencia — el sistema no falla por reglas viejas sino porque el problema es más grande que la institución (usa `/escala`).
- El usuario busca optimizar, no entender. El sedimento no se "arregla": se hereda con criterio o se hereda sin él.

Si tu caso no se parece al de origen, dilo. Una lente que no sabe cuándo no aplica es exactamente el problema que describe.
