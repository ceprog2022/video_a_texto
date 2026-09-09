Transcribir Clases 🎙️📝

Notebook de Google Colab para transcribir automáticamente clases en español usando Whisper de OpenAI.

¿Qué hace?
Instala openai-whisper y ffmpeg.
Permite subir un archivo de audio (previamente extraído del video de la clase) desde tu computadora.
Transcribe el contenido a texto usando el modelo medium de Whisper, configurado en español.
Guarda la transcripción en un archivo .txt y lo descarga automáticamente.
Cómo usarlo
Extraé el audio del video de la clase (por ejemplo, con ffmpeg en tu computadora o algún conversor de video a audio), para obtener un archivo de audio (mp3, wav, etc.).
Abrí el notebook TranscribirClases.ipynb en Google Colab.
(Recomendado) Activá una GPU: Entorno de ejecución > Cambiar tipo de entorno de ejecución > GPU (T4). Esto acelera mucho la transcripción.
Ejecutá las celdas en orden:
Celda 1: instala las dependencias necesarias.
Celda 2: te permite subir el archivo de audio extraído a transcribir.
Celda 3: carga el modelo Whisper y genera la transcripción.
Celda 4: guarda el resultado en un .txt y lo descarga.
Requisitos
Cuenta de Google (para usar Colab).
Archivo de audio ya extraído del video (mp3, wav, etc.).
Conexión a internet.

No requiere instalación local para la transcripción: todo corre en la nube de Google Colab. La extracción del audio del video sí se hace por fuera, antes de subirlo al notebook.

Notas
El modelo usado es medium. Se puede cambiar por tiny, base, small, large según la precisión y velocidad que necesites (modelos más grandes son más precisos pero más lentos).
El idioma está fijado en español (language="es"). Se puede quitar ese parámetro para que Whisper detecte el idioma automáticamente.
El nombre del archivo de salida (transcripcion14.txt) se puede personalizar editando la última celda.
Licencia

Uso libre y personal.
