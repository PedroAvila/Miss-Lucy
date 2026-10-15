# ADR 0005: Numeración consecutiva y no repetición de temas de HelloTalk

## Estado
Aceptado

## Fecha
2026-10-15

## Contexto

En el archivo `conversacion/temas-hellotalk.md` se van añadiendo temas diarios para practicar en HelloTalk, etiquetados como `## Día N — YYYY-MM-DD: ... (nivel X)`.

Se ha detectado confusión al crear un nuevo tema: en una ocasión se propuso un número de día sin verificar correctamente en qué día se había quedado el archivo (el último tema registrado era **Día 14 — 2026-09-23**). Esto puede provocar saltos de numeración, desorden o riesgo de reutilizar un número ya existente.

Al tratarse de un registro histórico y secuencial del estudio, conviene establecer una regla clara para mantener la numeración consecutiva y evitar repeticiones entre temas.

## Decisión

Cuando se cree un nuevo tema para HelloTalk (`conversacion/temas-hellotalk.md`), **siempre** se debe seguir este procedimiento:

1. **Verificar el último día registrado.** Antes de añadir cualquier tema nuevo, se debe leer el archivo y localizar el último encabezado `## Día N — YYYY-MM-DD` para identificar con seguridad el número de día (`N`) en el que se quedó el registro.

2. **Seguir la numeración consecutiva obligatoria.** El siguiente tema debe usar **Día N+1**, incrementando exactamente en +1 respecto al último día existente. No se permiten saltos arbitrarios, ni reutilizar números anteriores.

3. **Verificar que no se repita el tema.** Antes de crearlo, hay que comprobar que el título, el enfoque o las preguntas propuestas no existan ya en el archivo. En caso de duda, se debe buscar por palabras clave para descartar cualquier repetición.

4. **Mantener coherencia de fechas.** La fecha (`YYYY-MM-DD`) debe seguir una secuencia lógica respecto al último tema. No se deben retroceder fechas sin una justificación explícita por parte del usuario.

5. **Añadirlo siempre al final del archivo.** El nuevo tema debe agregarse justo después del último tema existente, preservando el orden cronológico y consecutivo.

6. **Verificación obligatoria tras añadirlo.** Tras escribirlo en el archivo, se debe leer los últimos párrafos para confirmar que el nuevo tema aparece con el número `Día (N+1)` correcto y que no se ha alterado ningún tema anterior.

## Consecuencias

- Garantiza que siempre se sabe con claridad «en qué día se quedó» el registro antes de crear el siguiente tema.
- Mantiene la numeración estrictamente consecutiva y libre de duplicados.
- Preserva el orden y la coherencia del archivo como registro histórico de estudio.
- Reduce errores y evita confusiones al generar nuevos temas para HelloTalk.
- Establece un criterio claro y reutilizable para futuras incorporaciones de temas.