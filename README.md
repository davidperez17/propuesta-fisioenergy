# Propuesta FisioEnergy — Servicios Digitales

Propuesta comercial para **FisioEnergy** (Guatemala): sistema de expediente clínico con
evaluación fisioterapéutica progresiva y agenda sincronizada con Google Calendar.

**Propuesta 1 de 2 · Sistema base (MVP)** · Presentada el 20 de agosto de 2026.

## Ver la propuesta

👉 **https://davidperez17.github.io/propuesta-fisioenergy/**

## Cómo está hecha

`index.html` es un documento autocontenido: sin build, sin framework, sin dependencias.
El único recurso externo es Google Fonts (Inter); los logotipos van embebidos en base64,
así que la página funciona incluso sin conexión una vez cargada.

```
index.html            la propuesta completa
demo/index.html       visor de la demo (barra lateral + pantalla escalada)
demo/pantallas/*.html las 11 pantallas del sistema, una por archivo
robots.txt            Disallow: / — no se indexa en buscadores
.nojekyll             GitHub Pages sirve los archivos tal cual
```

## Demo

👉 **https://davidperez17.github.io/propuesta-fisioenergy/demo/**

Once pantallas del sistema como HTML estático: sin cuenta, sin instalar nada, sin
depender de ningún servicio externo. Las pantallas de evaluación y de sesión tienen
los deslizadores, las pestañas y el selector de fuerza funcionando con JavaScript plano.

Las pantallas se generan desde los artboards `.dc.html` del proyecto con
`demo/build/render.mjs` (resuelve las plantillas y escribe HTML autónomo). El maestro
editable sigue siendo el lienzo de Claude Design; este directorio es la exportación.

La demo está pensada para verse en computadora: las pantallas miden 1440 px de ancho.

## Marca

Sigue el sistema de diseño de [Servicios Digitales](https://serviciosdigitalesgtm.com):
primario `#015AFC`, medium `#012FD3`, dark `#0101A7`, tinta `#1A1C1F`, tipografía Inter,
radios de 16px en tarjetas, pills para acciones, sombras tintadas al azul e iconos Lucide.

## Editar

Editar `index.html` y hacer push. GitHub Pages se actualiza en 1–2 minutos.

> La página lleva `noindex, nofollow` y el `robots.txt` bloquea todo, así que no aparece
> en buscadores. Aun así **el repositorio es público**: no agregar aquí estrategia
> comercial interna ni datos personales de la clienta.

---

© Servicios Digitales · Guatemala · +502 3960 7045 · info@serviciosdigitalesgtm.com
