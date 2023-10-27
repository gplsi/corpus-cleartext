
## Corpus ClearText v1.0

Corpus de documentos de la administración pública, en lectura fácil y versión original cuando está disponible. Este corpus sigue en desarrollo y por el momento contiene 140.000 tokens de documentos como el Estatuto de Autonomía de la Comunidad de Madrid o la Guía sobre las instituciones y organismos de la Unión Europea.

Puede ser utilizado para desarrollar métodos de alineamiento entre las versiones en lectura fácil y original, el entrenamiento de modelos de generativos para simplificación, entre otras tareas de Procesamiento del Lenguaje Natural.


#### Estructura de los archivos

Cada documento está disponible como un archivo **.json**, con la siguiente estructura.

```json
{
  "title":"título del documento",
  "version":"mes y año de la versión del documento",
  "url":"localización en línea del documento",
  "lf":"bool: indica si el documento es una versión en lectura fácil",
  "document":[
    {
      "page":"número de página",
      "text":"texto de la página"
    },
    {
      "page":"número de página",
      "text":"texto de la página"
    },
  ]
}
```

