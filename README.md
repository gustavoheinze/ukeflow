# 🌺 UkeFlow

**UkeFlow** es una aplicación web minimalista y "single-file" diseñada para ayudarte a practicar y aprender canciones en ukulele. Funciona como un teleprompter musical inteligente que sincroniza los acordes y la letra en tiempo real.

![UkeFlow Screenshot](./screenshot.png)
*(Si tienes una captura de pantalla, puedes agregarla aquí)*

## ✨ Características

*   **Teleprompter de Acordes**: Visualización clara del acorde actual (con diagrama de dedos), el anterior y el siguiente.
*   **Motor de Ritmo**: Los acordes avanzan automáticamente sincronizados con el tempo (BPM) de la canción.
*   **Control de Velocidad**: Slider ajustable del 50% al 150% para practicar lento y acelerar gradualmente.
*   **Transposición en Tiempo Real**: Botones `b` y `#` para cambiar el tono de la canción al instante y adaptarlo a tu voz.
*   **Diseño Responsive**: Interfaz limpia y moderna que funciona perfecto en PC y celulares.
*   **Single-File**: Todo el código (HTML, CSS, JS) vive en un solo archivo `index.html`. No requiere instalación ni servidor.

## 🚀 Cómo usarla

1.  Descarga el archivo `index.html`.
2.  Ábrelo en cualquier navegador web (Chrome, Firefox, Safari, Edge).
3.  Selecciona una canción del menú desplegable.
4.  Dale al **Play** (▶) y ¡comienza a tocar!

### Canciones Incluidas
*   I'm Yours - Jason Mraz
*   Riptide - Vance Joy
*   Somewhere Over The Rainbow - IZ
*   Can't Help Falling in Love - Elvis Presley
*   Stand By Me - Ben E. King

## 🛠️ Personalización (Cómo agregar canciones)

Puedes agregar tus propias canciones editando el archivo `index.html` con cualquier editor de texto (Notepad, VS Code, etc.).

Busca la sección `const SONGS = [...]` y agrega un nuevo objeto siguiendo este formato:

```javascript
{
    title: "Nombre de tu Canción - Artista",
    bpm: 120, // Velocidad en Beats Por Minuto
    chords: [
        { c: 'C', l: "Letra de la primera línea..." },
        { c: 'G', l: "Letra de la segunda línea..." },
        { c: 'Am', l: "Estribillo..." },
        // ...
    ]
}
```

*   `c`: Acorde (Ej: "C", "Am", "G7", "F#m").
*   `l`: Letra o texto a mostrar.

## 💻 Tech Stack

*   **HTML5**
*   **CSS3** (Variables, Flexbox, Grid)
*   **JavaScript** (Vanilla ES6+)
*   **Canvas API** (Para dibujar los diagramas de acordes)

## 📄 Licencia

Este proyecto es de código abierto. ¡Siéntete libre de modificarlo y compartirlo!
