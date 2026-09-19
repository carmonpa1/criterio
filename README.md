# Criterio — lentes para mirar sistemas

Lentes de análisis destiladas de los ensayos de [carlesmontrull.me](https://carlesmontrull.me).

Carles Montrull — [carlesmontrull.me](https://carlesmontrull.me) · [LinkedIn](https://www.linkedin.com/in/carlesmontrull)

No son métodos ni checklists. Las lentes transmiten preguntas, distinciones y hábitos de atención nacidos de los ensayos. Ayudan a ejercitar el criterio; no sustituyen el juicio de quien decide.

Cada una conserva una síntesis del caso de origen, sus límites y el enlace al ensayo. Volver a ese origen permite discutir qué se conserva y qué se pierde al trasladarlo a otro contexto. Los casos incluyen experimentos ficticios y ejercicios de diseño de futuros: se identifican como tales, no como validaciones generales.

## Instalación

En Claude Code:

```
/plugin marketplace add carmonpa1/criterio
/plugin install criterio
```

## Lentes

| Lente | Comando | Cuándo usarla | Ensayo de origen |
|---|---|---|---|
| **Sedimento** | `/sedimento` | Auditar qué reglas heredó un sistema y cuáles se ejecutan sin el criterio que las creó | [Sedimento](https://carlesmontrull.me/essays/sedimento) |
| **Instancia** | `/instancia` | Distinguir estructura reproducible y posición acumulada, contrastando su valor y dificultad de sustitución | [La instancia](https://carlesmontrull.me/essays/la-instancia) |
| **Escala** | `/escala` | Comprobar si un problema cabe dentro de la institución que intenta resolverlo | [Escala](https://carlesmontrull.me/essays/escala) |
| **Jurisdicción** | `/jurisdiccion` | Decidir qué decisiones no le pertenecen a un sistema automático, aunque pueda ejecutarlas | [Sedimento](https://carlesmontrull.me/essays/sedimento) · [La instancia](https://carlesmontrull.me/essays/la-instancia) |
| **Sede vacante** | `/sede-vacante` | Diseñar cómo se atraviesa el vacío cuando falta quien dirige | [Sede vacante](https://carlesmontrull.me/essays/sede-vacante) |
| **Código** | `/codigo` | Investigar si variables aparentemente neutras transportan información sensible y cómo afecta su uso | [El código](https://carlesmontrull.me/essays/el-codigo) |

## Cómo usarlas

Cada lente se aplica sobre un sistema real: una empresa, un producto, un equipo, un proceso, un espacio, un agente. Le das el material — documentación, reglas, o simplemente la descripción — y la lente devuelve un acta: qué encuentra, en qué se apoya, qué sigue sin saber y qué pregunta queda abierta.

El acta puede encontrar un problema, justificar mantener lo existente o reconocer que faltan datos. Su valor está en esclarecer una decisión, aunque confirme la intuición inicial. Las propuestas de diseño son propuestas: aplicarlas requiere la decisión de quien tiene autoridad.

Por ejemplo, `/sedimento` puede distinguir una regla obsoleta de otra cuyo expediente simplemente no se ha aportado. `/codigo` puede señalar un proxy sospechoso sin declararlo confirmado. `/jurisdiccion` puede concluir que el reparto de decisiones ya es adecuado.

La pregunta final nace del análisis: puede pedir una decisión, una evidencia ausente o una condición de revisión. No obliga a cambiar algo para demostrar que la lente funcionó. Las derivaciones a otras lentes se señalan solo cuando el caso las necesita.

## Cuándo desconfiar

Cada `SKILL.md` termina con una sección propia de "cuándo desconfiar de esta lente": dónde se formó, dónde funciona peor y a qué otra lente derivar.

Es deliberado. Una lente que no sabe cuándo no aplica es exactamente el problema que estas lentes describen.

Al contrastar una lente, incluye un caso donde aporta, otro donde no hay hallazgo y otro con información insuficiente. Examina si distingue evidencia de inferencia, considera una explicación alternativa relevante y puede cambiar de conclusión. Un resultado incómodo no demuestra que sea correcto.

El molde también es revisable: si obliga a encontrar lo que el caso no contiene, debe cambiar. El ensayo conserva la procedencia; no convierte sus conclusiones en inmunes a la crítica.

## Licencia

MIT. Las lentes se publican para que se usen, se critiquen y se bifurquen. Los ensayos de los que nacen son de Carles Montrull y viven en [carlesmontrull.me](https://carlesmontrull.me).
