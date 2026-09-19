---
name: jurisdiccion
description: Lente de diseño para decidir qué decisiones NO le pertenecen a un sistema automático, agente de IA o proceso, aunque técnicamente pueda ejecutarlas. Úsala siempre que el usuario esté diseñando o revisando un agente, una automatización, un flujo de aprobaciones, una política de delegación o un conjunto de reglas operativas; cuando pregunte qué puede automatizar y qué no; cuando un sistema "cumplió las reglas" y aun así causó daño; o cuando mencione autonomía, guardarraíles, límites, escalado a humano, human-in-the-loop, o hasta dónde dejar decidir a la IA.
---

# Jurisdicción

Una lente, no un método. Nace de dos ensayos: *Sedimento* (carlesmontrull.me/essays/sedimento), donde un agente rechazó impecablemente una oportunidad porque la norma lo decía, y *La instancia* (carlesmontrull.me/essays/la-instancia), sobre enjambres de agentes que instancian y operan sin humanos en el ciclo.

## La idea que sostiene la lente

La pregunta habitual al automatizar es: ¿puede el sistema hacer esto? Es la pregunta equivocada, porque cada vez la respuesta es más veces sí.

La pregunta útil es otra: **¿le pertenece esta decisión?** Hay decisiones que un sistema puede ejecutar perfectamente y que, aun así, no son de su tamaño — porque su consecuencia excede lo que el sistema puede ver, porque son irreversibles, o porque comprometen algo que la regla no sabe que existe.

Un sistema sin jurisdicción explícita no se detiene. Ejecuta con precisión, sin cansancio, sin excepciones, y sin saber en ningún momento que debería parar.

La jurisdicción se escribe antes. Descubierta después, ya es un incidente.

## Cómo aplicar la lente

Pide al usuario el sistema, el agente o el proceso, y el alcance que tiene o se le quiere dar. Después:

**1. Mapa de decisiones.** Lista las decisiones que el sistema toma o tomaría, no las tareas que ejecuta. La diferencia importa: "enviar el email" es una tarea; "decidir a quién se le responde y a quién no" es una decisión.

**2. Los cuatro tests.** Para cada decisión consecuente:

- *Reversibilidad*: si se equivoca, ¿se puede deshacer? ¿A qué coste y en cuánto tiempo?
- *Visibilidad*: ¿queda registro de que esa decisión se tomó, o desaparece dentro del flujo sin que nadie pueda revisarla?
- *Alcance*: ¿la consecuencia cabe dentro de lo que el sistema observa, o se propaga a sitios que el sistema no ve — una relación, una reputación, una persona?
- *Excepcionalidad*: ¿es un caso repetido o uno de esos que ninguna regla previó? Los sistemas fallan precisamente donde la regla no llegaba.

**3. Trazar la frontera.** Con los tests hechos, reparte las decisiones en tres zonas: **propias** del sistema (ejecuta y punto), **de borde** (ejecuta pero deja constancia y aviso), y **ajenas** (no las toma nunca; se detiene y escala a una persona con nombre).

Lo importante es la tercera zona. Escribirla explícitamente es el entregable.

**4. El test del evaluador.** Pregunta cómo se mide el éxito de este sistema. Luego pregunta cuál sería la forma más eficiente de superar esa métrica traicionando el propósito. Si existe un camino corto, el sistema lo encontrará — no por malicia, por eficiencia. Ese camino hay que cerrarlo en la jurisdicción, no en la métrica.

## Formato de salida

Un acta breve, en prosa:

- Las tres zonas, con las decisiones repartidas.
- La lista explícita de lo que el sistema no hará nunca, redactada como se escribiría en un documento operativo.
- El camino corto que la métrica permite, si lo hay.
- Qué persona concreta recibe lo que se escala — la jurisdicción sin destinatario no existe.
- Una derivación a las otras lentes: qué parte del hallazgo ya no es de jurisdicción sino de otra — reglas heredadas que nadie revisó a `/sedimento`, defensibilidad o foso a `/instancia`, un problema más grande que la institución a `/escala`, sucesiones, relevos o dependencia de una persona clave a `/sede-vacante`, variables prohibidas que se cuelan por proxies heredados a `/codigo` — señalada, sin desarrollarla.
- La pregunta que cierra el acta, dirigida al usuario y que él tiene que responder: qué decisión de las que hoy deja al sistema va a devolver a una persona. No es un ofrecimiento de profundizar ni un "¿quieres que siga?".

Tono: operativo. Esto se escribe para pegarlo en un prompt, en una política o en un contrato. El acta termina en esa pregunta; no se ofrece a continuar.

## Cuándo desconfiar de esta lente

Se formó con agentes operando negocios pequeños y con la discusión pública sobre autonomía de la IA en 2026. Funciona peor cuando:

- El sistema no toma decisiones, solo ejecuta tareas deterministas. Aplicarla ahí produce burocracia sin beneficio.
- El problema real es que las reglas que ejecuta están caducadas (usa `/sedimento` antes).
- El usuario busca cumplimiento normativo. Esta lente diseña criterio, no acredita conformidad ante un regulador.

Y una advertencia sobre sí misma: toda frontera escrita envejece. Una jurisdicción que nadie revisa es sedimento en cinco años.
