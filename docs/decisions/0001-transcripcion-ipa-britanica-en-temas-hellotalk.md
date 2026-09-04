# 1. Transcripción IPA británica en temas-hellotalk.md

Fecha: 2026-09-04

## Estado

Aceptado

## Contexto

Pedro usa [tophonetics.com](https://tophonetics.com/) para obtener la transcripción IPA británica de las
frases que practica antes de sus sesiones de HelloTalk. Eso significa salir del repo, pegar cada frase en
la web, copiar el resultado y volver — un paso extra cada vez que prepara un tema nuevo.

Quiere lo mismo pero sin salir del archivo: que cada frase en inglés de
`conversacion/temas-hellotalk.md` tenga su transcripción IPA (acento británico / RP) escrita justo debajo,
para poder leer y practicar la pronunciación directamente ahí, sin depender de la web en el momento de
estudiar.

## Decisión

Se agrega, debajo de cada frase en inglés de `conversacion/temas-hellotalk.md` (preguntas, respuestas de
ejemplo, estructuras B1 y frases de rescate), una línea con su transcripción fonética en IPA usando el
acento británico (Received Pronunciation), siguiendo las convenciones que aplica tophonetics por defecto:

- Formas débiles en palabras funcionales dentro de la frase (`have` → `həv`, `to` → `tə`, `that` → `ðət`).
- Marcas de acento primario `ˈ` y secundario `ˌ`, y `ː` para vocal larga.
- Los placeholders entre corchetes (`[platillo]`, `[time]`, etc.) se dejan sin transcribir, porque son
  texto que Pedro rellena con su caso real y no tiene una pronunciación fija.

La transcripción se escribe a mano (no se automatiza ni se llama a la API/web de tophonetics), directamente
al editar el archivo markdown.

## Consecuencias

- Pedro puede leer pregunta, IPA y traducción en un solo lugar y una sola pasada, sin cambiar de ventana
  antes de una sesión de HelloTalk.
- Cada tema nuevo que se agregue a `temas-hellotalk.md` deberá incluir su IPA de la misma forma, para
  mantener el archivo consistente.
- La transcripción es manual, así que puede tener pequeñas diferencias frente a lo que devolvería
  tophonetics.com (por ejemplo en formas débiles); no se busca una fidelidad absoluta, sino una guía de
  pronunciación suficientemente buena para practicar.
