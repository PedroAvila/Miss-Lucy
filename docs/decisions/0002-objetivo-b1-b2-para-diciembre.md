# 2. Cubrir niveles B1 y B2 antes de diciembre 2026

Fecha: 2026-09-04

## Estado

Aceptado

## Contexto

Pedro lleva ~1.5 años estudiando inglés por su cuenta (ver `plan-ingles.md`), con un giro reciente hacia
producción activa (HelloTalk, shadowing, self-talk) tras notar estancamiento por exceso de estudio pasivo de
vocabulario/gramática.

Hasta ahora el trabajo (vocabulario, temas de conversación, ejercicios) no tenía un nivel objetivo
explícito — `temas-hellotalk.md` etiqueta el Día 2 como "nivel B1", pero es la única referencia de nivel en
todo el repo. Sin una meta de nivel y una fecha, es difícil medir si el estudio diario realmente está
avanzando o solo generando más contenido.

Pedro decide fijar una meta concreta: cubrir **B1 y B2** como desafío, con **diciembre de 2026** como
horizonte. Hay margen de tiempo (de inicios de septiembre a diciembre, ~3-4 meses) para lograrlo, yendo
"con todo" — priorizando este objetivo sobre seguir acumulando contenido sin dirección de nivel.

## Decisión

- El objetivo del estudio de aquí a diciembre de 2026 es cubrir los niveles **B1 y B2** (MCER/CEFR), no solo
  seguir practicando en general.
- Todo el material nuevo que se agregue al repo (vocabulario, temas de conversación, ejercicios) debe
  etiquetar el nivel al que apunta (B1 o B2), igual que ya se hace parcialmente en `temas-hellotalk.md`.
- El plan semanal (`plan-ingles.md`) se usa como vehículo para este objetivo: la práctica diaria de HelloTalk,
  shadowing y self-talk debe ir subiendo de dificultad progresivamente, de B1 hacia B2, en vez de quedarse
  estancada en un solo nivel.
- Se usa diciembre de 2026 como fecha de corte para evaluar el progreso, apoyándose en la "métrica de
  progreso cada 4 semanas" ya definida en `plan-ingles.md` (audio de 2 minutos comparado mes a mes).

## Consecuencias

- ~~Se necesita definir, en algún punto, qué significa "cubrir B1" y "cubrir B2" en términos concretos...~~
  **Resuelto** en [0003-criterios-concretos-b1-b2.md](0003-criterios-concretos-b1-b2.md): checklist de
  gramática, rango de vocabulario y criterios de fluidez para cada nivel, con checkpoints trimestrales.
- ~~El contenido futuro... debería organizarse o revisarse pensando en progresión de nivel...~~ **Resuelto**:
  `conversacion/temas-hellotalk.md` ya etiqueta sus temas por nivel (B1) y referencia el ADR 0003;
  `palabras-ingles/vocabulary.txt` adoptó la misma convención (`[B1]`/`[B2]` por palabra) para todo lo que se
  agregue desde 2026-09-04 en adelante — las ~1700 palabras previas no se reclasifican retroactivamente, por
  ser trabajo de bajo valor frente a seguir avanzando.
- Al ser una meta ambiciosa en un plazo de meses, exige consistencia diaria — no intensidad extrema
  puntual. Los checkpoints del ADR 0003 y la tabla de seguimiento semanal de `plan-ingles.md` (columna
  "Nivel/estructura trabajada") son la señal temprana: si un checkpoint no se cumple, o el ritmo real es
  insostenible (ej. muchas horas diarias que no se sostienen en el tiempo), la meta de diciembre debe
  revisarse ahí, no al final.
- Diciembre 2026 dejó de ser el final del plan: es el corte de la fase de estudio (cubrir el temario),
  seguido por la fase de consolidación definida en [ADR 0004](0004-fase-de-consolidacion-dic2026-feb2027.md)
  hasta febrero de 2027, cuando Pedro cumple dos años de estudio.
