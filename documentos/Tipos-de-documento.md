# Tipos de documentos aceptados por NotebookLM

*Última actualización: miércoles, 19 de marzo de 2024*

NotebookLM puede procesar una variedad de formatos de documentos para crear su base de conocimiento. A continuación se detallan los tipos de documentos aceptados y sus características.

## Resumen de fuentes soportadas

NotebookLM actualmente soporta:
- Google Docs
- Google Slides
- Archivos PDF, Texto y Markdown
- URLs web
- Texto copiado y pegado
- URLs de YouTube (videos públicos)
- Archivos de audio

**Limitaciones generales:**
- Cada fuente puede contener hasta 500,000 palabras o hasta 200MB para archivos cargados
- Evita cargar documentos sobre los que no tengas los derechos aplicables

## Documentos de texto

### Formatos aceptados:
- Google Docs
- Google Slides
- PDF (`.pdf`)
- Microsoft Word (`.docx`)
- Texto plano (`.txt`)
- Markdown (`.md`)
- Páginas web (URLs)
- Texto copiado y pegado

### Características específicas:
- **Google Docs/Slides**: NotebookLM crea una copia estática. Los cambios en el documento original requieren sincronización manual con el botón "Click to sync with Drive".
- **PDFs**: A partir de septiembre 2024, se soportarán PDFs que contienen solo imágenes. La carga de PDFs a través de Drive no está soportada actualmente.
- **URLs web**: Solo se extrae el contenido de texto visible. No se importan imágenes, videos o páginas anidadas. No funciona con páginas con paywall o que hayan deshabilitado el web scraping.

### Consejos para mejores resultados:
- Asegúrate que los PDF tengan texto seleccionable y no sean escaneados sin OCR
- Los documentos bien estructurados con títulos, subtítulos y párrafos claros funcionan mejor
- Documentos con tablas de contenido ayudan a NotebookLM a entender la estructura
- Evita documentos con demasiados elementos no textuales sin contexto
- La calidad es más importante que la cantidad

## Archivos de audio

### Formatos aceptados:
- MP3 (`.mp3`)
- WAV (`.wav`)
- Otros formatos de audio comunes

### Características específicas:
- El audio se transcribe durante la importación y su texto se guarda como fuente nueva
- Audio sin habla no es compatible
- Soporta más de 30 idiomas para importación de audio

## Videos de YouTube

### Características:
- Solo videos públicos con subtítulos (subidos por el usuario o generados automáticamente)
- Solo se importa la transcripción de texto del video
- Videos recientes (menos de 72 horas) pueden no estar disponibles para importar
- Videos sin habla no son compatibles
- Las fuentes se eliminan automáticamente del notebook en 30 días si el video se elimina o se hace privado

## Imágenes y PDF con contenido textual

### Formatos aceptados:
- PDF escaneados con texto
- Imágenes con texto (son procesadas mediante OCR)

### Consejos para mejores resultados:
- Asegúrate que las imágenes tengan buena resolución
- El texto debe ser claramente legible
- Para documentos escaneados, Notebook convierte las imágenes en texto 

## Recomendaciones generales

- Revisa y limpia los datos antes de cargarlos (elimina contenido irrelevante)
- Organiza tus documentos por temas para facilitar la creación de conocimiento contextual
- Asegúrate que los documentos no contengan información sensible o confidencial que no debas compartir
- Para solicitar resúmenes específicos, formula preguntas concretas (ej: "Resumir hallazgos clave sobre X del documento titulado Y")
- Recuerda que NotebookLM no puede responder a preguntas si la información no está en las fuentes
- El historial de chat no persiste entre sesiones (puedes guardar notas importantes fijando las respuestas)
