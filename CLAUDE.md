# Edades — repo de PUBLICACIÓN (solo build)

Esto es la salida compilada que sirve GitHub Pages. **Aquí no se desarrolla nada**: el
fuente vive en `enekodevs/edades-fuente` y este repo se pisa con cada publicación.

## Regla de oro del contexto

**NO leas jamás `assets/index-*.js`**: es 1,3 MB de Phaser + juego minificados
(~350.000 tokens — una sola lectura completa revienta la ventana de contexto y no
enseña nada: los identificadores están mangleados). Tampoco `audio/` ni `splash/`
(binarios). Si necesitas entender el código, ve a `edades-fuente/src/` y usa su skill
`ahorro-tokens`.

Lo único legible aquí: `index.html` (con comentarios útiles sobre PWA/iOS) y
`manifest.webmanifest`.
