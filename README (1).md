# Transcribir Clases 🎙️📝

Notebook de Google Colab para transcribir automáticamente clases, videos o audios en español usando [Whisper](https://github.com/openai/whisper) de OpenAI.

## ¿Qué hace?

1. Instala `openai-whisper` y `ffmpeg`.
2. Permite subir un archivo de video o audio desde tu computadora.
3. Transcribe el contenido a texto usando el modelo `medium` de Whisper, configurado en español.
4. Guarda la transcripción en un archivo `.txt` y lo descarga automáticamente.

## Cómo usarlo

1. Abrí el notebook `TranscribirClases.ipynb` en [Google Colab](https://colab.research.google.com/).
2. (Recomendado) Activá una GPU: `Entorno de ejecución > Cambiar tipo de entorno de ejecución > GPU (T4)`. Esto acelera mucho la transcripción.
3. Ejecutá las celdas en orden:
   - **Celda 1:** instala las dependencias necesarias.
   - **Celda 2:** te permite subir el archivo de audio/video a transcribir.
   - **Celda 3:** carga el modelo Whisper y genera la transcripción.
   - **Celda 4:** guarda el resultado en un `.txt` y lo descarga.

## Requisitos

- Cuenta de Google (para usar Colab).
- Archivo de audio o video (mp3, mp4, wav, etc.).
- Conexión a internet.

No requiere instalación local: todo corre en la nube de Google Colab.

## Notas

- El modelo usado es `medium`. Se puede cambiar por `tiny`, `base`, `small`, `large` según la precisión y velocidad que necesites (modelos más grandes son más precisos pero más lentos).
- El idioma está fijado en español (`language="es"`). Se puede quitar ese parámetro para que Whisper detecte el idioma automáticamente.
- El nombre del archivo de salida (`transcripcion14.txt`) se puede personalizar editando la última celda.

## Licencia

Uso libre y personal.
