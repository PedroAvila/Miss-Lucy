# 4. Fase de consolidación B1/B2: diciembre 2026 → febrero 2027

Fecha: 2026-09-04

## Estado

Aceptado

## Contexto

Los ADRs [0002](0002-objetivo-b1-b2-para-diciembre.md) y [0003](0003-criterios-concretos-b1-b2.md) fijan
diciembre de 2026 como fecha para *cubrir* B1 y B2: temario gramatical completo, rango de vocabulario
activo, criterios de fluidez definidos. Pero cubrir el temario no es lo mismo que dominarlo — hablar B2 de
forma sostenida requiere repetición real, no solo haber tocado cada estructura una vez.

Pedro fija **febrero de 2027** como el verdadero cierre: cumple dos años de estudio ese mes. Es el punto
natural para evaluar el resultado real de los dos años completos, no solo lo acumulado en archivos hasta
diciembre.

## Decisión

- De **diciembre 2026 a febrero 2027** se abre una fase de consolidación. Durante estos tres meses se
  **congela la incorporación de contenido nuevo**: no se agregan más tandas de `palabras-ingles/README.md`,
  no se suman estructuras gramaticales nuevas al checklist del ADR 0003. Todo el tiempo de estudio va a
  producción activa — HelloTalk, shadowing, self-talk — sobre lo que ya está cubierto.
- **Criterio de consolidación**: una estructura o palabra está consolidada cuando sale en conversación real
  sin pensarla, no cuando está escrita en el repo. Se apoya en los criterios de fluidez B2 ya definidos en
  el ADR 0003.
- **Plan mes a mes:**
  - **Diciembre 2026**: rotar las 10 tandas temáticas de `palabras-ingles/` en sesiones reales de HelloTalk,
    una o dos por semana, revisando también los temas de `conversacion/temas-hellotalk.md`.
  - **Enero 2027**: temas libres e imprevistos, sin guion preparado de antemano — es el paso que falta para
    que la fluidez B2 sea real y no solo ensayada.
  - **Febrero 2027**: mes de evaluación de cierre, sin contenido nuevo ni ensayo — solo hablar.
- **Cierre de los dos años (febrero 2027)**: grabar un audio de 5 minutos de tema libre y compararlo con los
  audios mensuales previos (métrica de `plan-ingles.md`), más un repaso del checklist gramatical del ADR
  0003 marcando qué quedó realmente activo frente a lo que solo se estudió.

## Nota de coach

El riesgo real de esta fase no es quedarse corto de contenido — es lo contrario: llegar a diciembre y seguir
agregando material nuevo porque "siento que falta algo". Consolidar se siente como no avanzar, y por eso es
la fase que más se abandona. La regla acá es explícita: **en estos tres meses, agregar contenido nuevo es
salirse del plan**, no una mejora. Si en diciembre aparece la tentación de sumar una tanda 11 o un tema
nuevo, la respuesta correcta es no — se anota como idea para después de febrero y se sigue practicando lo
que ya hay.

## Consecuencias

- `docs/decisions/0003-criterios-concretos-b1-b2.md` extiende su tabla de checkpoints con diciembre, enero y
  febrero, para que la línea de tiempo completa (septiembre 2026 → febrero 2027) quede en un solo lugar.
- `plan-ingles.md` referencia este ADR y dejará de hablar solo de "diciembre" como horizonte final.
- El repo necesitará, después de febrero de 2027, una revisión honesta: si el checklist B2 no quedó
  consolidado en la práctica, la conclusión no es alargar la fecha de nuevo sin más — es diagnosticar qué
  parte del método (no de la fecha) no funcionó.
