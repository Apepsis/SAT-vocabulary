# Visual Vocabulary

Aplicación web para estudiar vocabulario inglés con:

- imágenes reales de Wikimedia Commons;
- definición, categoría gramatical e IPA mediante Free Dictionary API;
- pronunciación;
- ejemplos y sinónimos;
- selección entre varias imágenes;
- palabras guardadas en el navegador;
- comprobación rápida de recuerdo.

## Cómo ejecutarla

### Opción recomendada: Visual Studio Code

1. Abre la carpeta `vocabulario_visual` en Visual Studio Code.
2. Instala la extensión **Live Server**.
3. Haz clic derecho sobre `index.html`.
4. Selecciona **Open with Live Server**.

### Opción con Python

Abre una terminal dentro de la carpeta y ejecuta:

```bash
python -m http.server 8000
```

Luego abre:

```text
http://localhost:8000
```

### Importante

No abras el archivo únicamente con doble clic si el navegador bloquea solicitudes externas.
Usar Live Server o `python -m http.server` evita ese problema.

## APIs utilizadas

- Wikimedia Commons MediaWiki API: imágenes, autor, licencia y enlace original.
- Free Dictionary API: definiciones, fonética, audios, ejemplos y sinónimos.

No necesita claves privadas y no genera imágenes con inteligencia artificial.
