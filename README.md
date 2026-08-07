# Vocab Coach — Alexis

Aplicación web local para dominar vocabulario SAT sin una API pagada.

## Qué incluye

- Coach adaptativo con sesiones de 5, 10, 15 o 20 preguntas.
- Flashcards con repetición espaciada.
- Match de palabra y definición.
- Verificación de:
  - selección de definición;
  - selección de palabra;
  - escritura exacta;
  - oración con espacio en blanco;
  - explicación mediante coincidencia de palabras clave;
  - pronunciación mediante reconocimiento de voz del navegador.
- Voces separadas para palabra/oración y definición.
- Selección de voces instaladas en el navegador.
- Importación directa de `SAT_Vocabulary_Master_Alexis_2026.xlsx`.
- Compatibilidad con las columnas:
  `ID`, `Palabra`, `IPA`, `POS`, `Significado ES`, `Definición EN`,
  `Sinónimos`, `Antónimos`, `Prioridad`, `Familia / formas`, `Ejemplo EN`.
- Seguimiento de aciertos, errores, intervalo, próximo repaso y dominio.
- Respaldo JSON y exportación del progreso en CSV.
- Almacenamiento local con IndexedDB.

## Cómo publicarlo en GitHub Pages

Reemplaza el `index.html` actual del repositorio `visual-vocabulary` por el archivo
`index.html` de este proyecto.

En GitHub Pages usa:

- Branch: `main`
- Folder: `/root`

## Importar el banco maestro

1. Abre la app.
2. Entra a **Configuración**.
3. Pulsa **Seleccionar archivo**.
4. Carga `SAT_Vocabulary_Master_Alexis_2026.xlsx`.
5. La app detectará la pestaña `Banco maestro`.

La importación ocurre en el navegador. El archivo no se sube a un servidor.

## Verificación sin IA

La app puede verificar de forma objetiva respuestas cerradas, escritura y cloze.
La explicación libre se evalúa con coincidencia de palabras clave, no mediante comprensión
semántica completa. El reconocimiento oral comprueba la transcripción de la palabra, pero no
produce una calificación fonética profesional.

## Dependencia

Para leer archivos Excel se usa SheetJS Community Edition 0.20.3 desde su CDN oficial.
No requiere clave ni pago.
