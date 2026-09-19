---
name: codigo
description: Lente de auditoría para detectar variables prohibidas que se cuelan por proxies heredados — datos aparentemente neutros (código postal, centro de estudios, antigüedad, dispositivo, barrio) que reconstruyen una discriminación que la norma ya prohíbe. Úsala siempre que el usuario diseñe o revise un sistema de scoring, segmentación, precios personalizados, selección de personal, concesión de crédito, admisión, priorización de clientes o cualquier modelo que decida sobre personas; cuando pregunte si un sistema es justo o si tiene sesgo; o cuando mencione datos demográficos, variables sensibles, discriminación, equidad o cumplimiento normativo en algoritmos.
---

# Código

Una lente, no un método. Nace del ensayo *El código* (carlesmontrull.me/essays/el-codigo), sobre un mapa dibujado en 1937 que sigue prediciendo hoy la temperatura de una calle y la esperanza de vida de quien nace en ella.

## La idea que sostiene la lente

Prohibir una variable no elimina la información. La desplaza.

Cuando una decisión discriminatoria se toma durante décadas, no se queda en el papel: se ejecuta sobre el mundo. Se convierte en dónde hay árboles, por dónde pasa la autopista, qué barrio tiene hospital. Y entonces la ley puede derogar la norma, pero no puede derogar la geografía que la norma produjo.

Por eso, cuando un modelo tiene prohibido usar una variable sensible y sin embargo lee un dato operativo y neutro —el código postal, el instituto, el código de sucursal—, está leyendo, sin saberlo y sin que nadie lo programara, la decisión antigua que quedó inscrita en el terreno.

El sesgo más difícil de ver no es el que alguien introduce. Es el que el sistema redescubre solo, a partir de datos que nadie pensó como sensibles.

## Cómo aplicar la lente

Pide al usuario el sistema de decisión y las variables que usa. Después:

**1. Inventario de variables.** Lista todas las entradas del modelo o del criterio, incluidas las que parecen puramente administrativas. La tentación es descartar las obvias por inocuas; esas son justamente las candidatas.

**2. Caza de proxies.** Para cada variable, pregunta: ¿qué más sabe esto de la persona que no es lo que dice saber? Un código postal sabe de renta, origen y salud. Un centro de estudios sabe de clase. Un dispositivo sabe de poder adquisitivo. Un hueco en el currículum sabe de maternidad o enfermedad. Marca las variables que correlacionan fuerte con algo que la ley o la ética prohíben usar.

**3. Excavación del origen.** Para los proxies encontrados, intenta reconstruir por qué correlacionan. Casi siempre hay una decisión antigua —urbanística, administrativa, comercial— que produjo esa correlación y que hoy está derogada u olvidada. Nombrarla convierte una sospecha estadística en un hecho discutible.

**4. El bucle de refuerzo.** Comprueba si la decisión del sistema empeora la variable que usó para decidir. Si a este grupo se le da peor precio o menos acceso, ¿eso lo empuja a seguir siendo el grupo que estadísticamente falla más? Si la respuesta es sí, el modelo no describe la realidad: la fabrica y luego la presenta como prueba de que acertaba.

**5. Qué se puede hacer de verdad.** Quitar el proxy rara vez basta —la información reaparece por otro—. Las salidas reales son tres, y conviene ponerlas sobre la mesa sin optimismo: sustituir el proxy por el dato causal que de verdad importa, medir el impacto del sistema por grupo aunque no se use la variable, o decidir explícitamente que el sistema no decidirá ese caso (y ahí entra `/jurisdiccion`).

## Formato de salida

Un acta breve, en prosa:

- Las variables con su clasificación: operativas limpias, proxies sospechosos, proxies confirmados.
- Para cada proxy confirmado, qué sabe de más y de qué decisión antigua viene, si se puede reconstruir.
- Si existe bucle de refuerzo, descrito paso a paso.
- Qué salida es viable aquí, sin prometer que quitar la variable resuelve nada.
- Una derivación a las otras lentes: qué parte del hallazgo ya no es de código sino de otra — reglas heredadas que nadie revisó a `/sedimento`, un problema más grande que la institución a `/escala`, decisiones que el sistema no debería tomar a `/jurisdiccion` — señalada, sin desarrollarla.
- La pregunta que cierra el acta, dirigida al usuario y que él tiene que responder: qué campo de los que hoy pide sin pensar está dispuesto a dejar de pedir. No es un ofrecimiento de profundizar ni un "¿quieres que siga?".

Tono: técnico y sin denuncia. Los proxies no se ridiculizan ni se moralizan — casi ninguno se puso ahí con mala intención, y por eso son difíciles de ver. El acta termina en esa pregunta; no se ofrece a continuar.

## Cuándo desconfiar de esta lente

Se formó con casos de vivienda, crédito y salud en contextos de segregación documentada. Funciona peor cuando:

- El sistema no decide sobre personas. Aplicarla a decisiones sobre objetos o procesos produce paranoia sin hallazgo.
- El usuario busca acreditar conformidad ante un regulador. Esta lente encuentra problemas; no firma certificados, y un acta suya puede complicar más que ayudar en esa conversación.
- El dato sospechoso es genuinamente causal y no un proxy. Si la variable explica el resultado por sí misma, quitarla empeora el modelo sin mejorar la equidad. La lente debe poder decir que no hay caso.
