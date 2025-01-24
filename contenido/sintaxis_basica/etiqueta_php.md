# Etiqueta de PHP

Cuando PHP analiza un fichero, utiliza las etiquetas de apertura `<?php` y cierre `?>` para determinar dónde iniciar y finalizar la interpretación del código. Este enfoque permite embeber PHP en diferentes tipos de documentos, ignorando todo lo que esté fuera de dichas etiquetas. Aunque existe una etiqueta de apertura abreviada `<?`, su uso está desaconsejado, ya que requiere habilitar la directiva `short_open_tag` en el archivo `php.ini` o compilar PHP con `--enable-short-tags`.

En archivos que contienen únicamente código PHP, se recomienda omitir la etiqueta de cierre `?>` al final. Esto ayuda a evitar espacios en blanco o líneas adicionales accidentales que podrían generar una salida no deseada, previniendo efectos indeseados relacionados con el manejo del búfer de salida de PHP.

```php
<?php
echo "Hola mundo";

// ... más código

echo "última sentencia";

// el script finaliza aquí sin etiqueta de cierre de PHP
```