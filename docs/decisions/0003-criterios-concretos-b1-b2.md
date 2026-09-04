# 3. Criterios concretos para "cubrir" B1 y B2

Fecha: 2026-09-04

## Estado

Aceptado — resuelve el pendiente dejado en [0002-objetivo-b1-b2-para-diciembre.md](0002-objetivo-b1-b2-para-diciembre.md)

## Contexto

[ADR 0002](0002-objetivo-b1-b2-para-diciembre.md) fijó diciembre de 2026 como meta para cubrir B1 y B2, pero
dejó pendiente definir qué significa "cubrir" cada nivel en términos medibles. Sin esa definición, no hay
forma de saber si el estudio diario de `plan-ingles.md` está realmente cerrando la brecha o solo generando
más contenido sin dirección.

Este ADR define los criterios de referencia (basados en el marco MCER/CEFR, adaptados a cómo está
estructurado este repo) para las tres dimensiones mencionadas en el ADR 0002: estructuras gramaticales,
rango de vocabulario y fluidez esperada.

## Decisión

### 1. Estructuras gramaticales (checklist académico completo, dominio activo no solo reconocimiento)

Basado en el temario gramatical estándar de CEFR/Cambridge (B1 Preliminary / B2 First), agrupado por
categoría para que sea fácil verificar qué falta.

**B1 — debe poder usarlas hablando, sin pararse a pensar la regla:**

*Tiempos verbales*
- Presente simple vs. presente continuo (incluyendo verbos de estado: `know`, `like`, `believe`)
- Pasado simple vs. pasado continuo (`I was cooking when she called`)
- Presente perfecto simple (`I've done that before`) y continuo (`I've been living here for...`)
- Pasado perfecto simple, uso básico (`I had already left when...`)
- Futuro: `will` vs. `going to` vs. presente continuo con valor de futuro (`I'm meeting her tomorrow`)
- `used to` / `would` para hábitos pasados

*Modales y condicionales*
- Modales de habilidad, permiso y obligación (`can/could`, `have to`, `must`, `should`)
- Modales de deducción (`must be`, `might`, `can't be`)
- Primer y segundo condicional (`If I have time, I'll...` / `If I could..., I would...`)

*Voz pasiva y forma*
- Voz pasiva simple en presente/pasado (`It's made with...`, `It was built in...`)
- Verbo + gerundio vs. verbo + infinitivo (casos regulares: `enjoy doing`, `want to do`)
- Phrasal verbs de uso frecuente (`give up`, `look after`, `find out`)

*Oraciones y conectores*
- Oraciones de relativo básicas, defining (`who`, `which`, `that`)
- Comparativos y superlativos con matices (`not as good as`, `by far the best`)
- Conectores de secuencia y causa (`first`, `then`, `because`, `so`, `although`)
- Cuantificadores (`a few`, `a little`, `too much/many`, `enough`)
- Preguntas indirectas (`Do you know what time it is?`) y question tags básicos

**B2 — se suman estas encima de las de B1:**

*Tiempos verbales*
- Pasado perfecto continuo (`I'd been waiting for an hour when...`)
- Futuro continuo y futuro perfecto (`I'll be working`, `I'll have finished by...`)
- Todos los tiempos combinados con narrativa compleja (mezclar pasado simple/continuo/perfecto en un mismo
  relato sin perder el hilo)

*Modales y condicionales*
- Modales de deducción en pasado (`must have been`, `can't have done`, `should have done`)
- Tercer condicional y condicionales mixtos (`If I had known, I would have...`)
- Wish/if only para pasado, presente y futuro (`I wish I hadn't...`, `I wish I could...`)

*Voz pasiva y forma*
- Voz pasiva en todos los tiempos, incluyendo con modales (`It should have been done`)
- Verbos con infinitivo/gerundio con cambio de significado (`stop to do` vs `stop doing`, `remember to do`
  vs `remember doing`)
- Causativo (`have/get something done`)
- Phrasal verbs de tres partículas y de registro más formal (`come up with`, `put up with`)

*Oraciones y conectores*
- Discurso indirecto, incluyendo preguntas y órdenes (`She said that she would...`, `He asked me if I had...`,
  `He told me to...`)
- Cláusulas relativas non-defining, con coma (`My brother, who lives in Spain, ...`)
- Cláusulas de propósito y contraste (`in order to`, `despite`, `even though`, `whereas`)
- Inversión enfática básica (`Not only did I..., but I also...`)
- Subjuntivo en sugerencias/exigencias (`I suggest that he be...`)
- Participle clauses para reducir cláusulas relativas/temporales (`Having finished..., I...`)

Fuente de seguimiento: la tabla semanal de `plan-ingles.md` — cada semana se marca qué estructura de la
lista se practicó activamente (no solo se vio pasivamente).

### 2. Rango de vocabulario

- **B1:** ~2500-3000 palabras activas (las que puede usar produciendo, no solo reconocer). Cubre temas
  cotidianos: trabajo, rutina, comida, viajes, familia, opiniones simples — el tipo de temas ya usados en
  `conversacion/temas-hellotalk.md`.
- **B2:** ~4000-5000 palabras activas. Se agrega vocabulario abstracto y de opinión matizada: expresar
  acuerdo/desacuerdo con matices, hablar de causas y consecuencias, temas de actualidad, vocabulario
  específico del propio trabajo/profesión.
- Medición práctica: cada palabra nueva en `palabras-ingles/vocabulary.txt` ya se registra con su oración de
  ejemplo (ver ajuste en `plan-ingles.md`). A partir de ahora, cada 4 semanas contar cuántas palabras nuevas
  activas se agregaron y en qué categoría temática caen, para verificar que se está ampliando hacia temas
  de nivel B2 y no solo repitiendo vocabulario B1.

### 3. Fluidez esperada

Se apoya en la métrica ya definida en `plan-ingles.md` (audio de 2 minutos cada 4 semanas), con criterios
explícitos de qué buscar en cada nivel:

- **B1 (meta: octubre 2026):**
  - Habla con pausas notorias pero mantiene el hilo sin cambiar a español mentalmente.
  - Oraciones de una sola cláusula, ocasionalmente dos conectadas con `and`/`but`/`because`.
  - Errores de gramática presentes pero no impiden entender el mensaje.
  - Usa circunlocución cuando le falta una palabra, sin trabarse por completo.

- **B2 (meta: diciembre 2026):**
  - Pausas menos frecuentes, ritmo más natural, menos "muletillas" de relleno en español.
  - Oraciones compuestas con al menos 2-3 cláusulas conectadas (relativas, condicionales, contraste).
  - Puede argumentar una opinión con al menos una razón y un matiz/contraejemplo (`..., although...`).
  - Autocorrección en vivo de errores simples sin perder el hilo del discurso.

**Generación de oraciones en tiempo real (identificado 2026-09-04):** el objetivo no es solo hablar con
fluidez sobre temas preparados — es **construir la oración en el momento**, con la gramática y el
vocabulario que ya se tienen, no recitar una frase memorizada de antemano. Es la diferencia real entre
"sonar fluido en un tema ensayado" y estar fluido de verdad, y hoy es el punto más débil identificado.

Cómo se entrena y se mide:
- **Self-talk sin guion** (ya está en `plan-ingles.md`, martes/jueves): la regla es no escribir la frase
  antes de decirla. Si aparece la tentación de escribirla primero, es la señal de que se está evitando el
  ejercicio real.
- **Preguntas de seguimiento no preparadas en HelloTalk**: además de las 5-6 preguntas que se preparan antes de
  cada sesión (ajuste del 2026-09-02 de `plan-ingles.md`), prestar atención a las repreguntas que el
  interlocutor hace en el momento — esas nunca están guionadas y son la prueba real de esta habilidad.
- **B1**: puede responder una pregunta no anticipada con una oración simple correcta, aunque tarde unos
  segundos en armarla.
- **B2**: puede responder y encadenar una segunda oración relacionada (dar una razón, un ejemplo) sin volver
  a un guion mental, con la pausa de construcción ya casi imperceptible.
- Esto se revisa en la fase de consolidación de enero 2027
  ([ADR 0004](0004-fase-de-consolidacion-dic2026-feb2027.md), "temas libres e imprevistos, sin guion
  preparado") — ese mes existe específicamente para entrenar esto, no los temas preparados de antemano.

### Checkpoints en el tiempo

| Fecha | Nivel objetivo | Qué revisar |
|-------|-----------------|-------------|
| Fin de septiembre 2026 | B1 en curso | Checklist gramatical B1 al 50%+, primer audio de referencia grabado |
| Fin de octubre 2026 | B1 cubierto | Checklist gramatical B1 completo, vocabulario activo ~2500+, audio muestra fluidez B1 |
| Fin de noviembre 2026 | B2 en curso | Checklist gramatical B2 al 50%+, vocabulario activo ~3500+ |
| Diciembre 2026 | B2 cubierto | Checklist gramatical B2 completo, vocabulario activo ~4000+, audio muestra fluidez B2 |
| Diciembre 2026 – febrero 2027 | Consolidación (sin contenido nuevo) | Ver [ADR 0004](0004-fase-de-consolidacion-dic2026-feb2027.md): rotar tandas ya hechas, luego temas libres |
| Febrero 2027 | Cierre de 2 años de estudio | Audio de 5 min comparado con septiembre 2026, checklist B2 revisado como consolidado o no |

## Consecuencias

- `plan-ingles.md` debería referenciar estos checkpoints en su tabla de seguimiento semanal, para que cada
  4 semanas la revisión de progreso compare contra estos criterios concretos y no sea solo subjetiva.
- El contenido nuevo (vocabulario, temas de conversación) debería etiquetarse con el nivel (B1/B2) al que
  apunta, tal como ya pedía el ADR 0002, usando esta lista de estructuras como referencia de qué gramática
  meter en cada tema nuevo.
- Si a fin de octubre el checklist B1 no está cerca de completarse, la fecha de diciembre para B2 debe
  revisarse — es una señal temprana de que el ritmo no alcanza, mejor detectarla en el checkpoint intermedio
  que al final.
