# Inktensa Daff — portfolio

Sitio de una sola página: una caída por la madriguera del conejo, en scroll, que
desemboca en la galería de tatuajes, cover-ups, citas y contacto.

**Ver online:** https://michellesalcedovallenilla-ai.github.io/portfolio-daff/

## Cómo está hecho

Un único `index.html` sin dependencias ni compilación — HTML, CSS y JavaScript a mano.
Lo único externo son las tipografías de Google (Cormorant Garamond y Cinzel).
Se puede abrir haciendo doble clic en el fichero.

- La ilustración de fondo se mueve con `transform` sobre un `<img>` fijo, ligada al scroll.
- La caída son **10 fotogramas ilustrados** que pasan como una animación según bajas
  (`alice-fall-1..10.png`), ordenados para que el giro de frente a espaldas fluya.
- La navegación es el reloj de bolsillo dorado, siempre visible arriba a la izquierda.
- Polvo de hadas en `<canvas>`, con estela que sigue al cursor.

## Rellenar antes de enseñarlo

En el HTML están marcados con la clase `.fill`:

- correo de contacto
- ciudad y estudio
- precios y seña
- horario
- bio de «Sobre mí»
- política de retoques

## Fotos de la galería

Van en `assets/portfolio/` con estos nombres:

- `01.jpg` … `12.jpg` — trabajos de la galería
- `cover-1-antes.jpg` / `cover-1-despues.jpg` (y 2, 3) — cover-ups

Los títulos y categorías se editan en los arreglos `GALERIA` y `COVERS`, al principio
del `<script>`. Si una foto falta, sale un marco con «Pendiente» — nunca una imagen rota.
