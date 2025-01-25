# Comentarios

En PHP, los comentarios son una herramienta fundamental para documentar el código, describir su funcionalidad y mejorar su legibilidad tanto para el programador como para otras personas que trabajen en el proyecto. Existen tres tipos principales de comentarios:

- Los comentarios de una sola línea.
- Los comentarios de múltiples líneas.
- Los comentarios estilo **PHPDoc**, diseñados específicamente para documentar funciones, clases y otros elementos del código.

Código en PHP que muestra los tipos de comentarios:

```php
// Comentario de una sola línea: Se usa para notas rápidas o breves explicaciones.

# Otra forma de comentario de una sola línea: Similar al estilo de shell scripts.

/*
 * Comentario de múltiples líneas:
 * Es ideal para documentar secciones más grandes del código
 * o agregar detalles extensos sobre la lógica implementada.
 */

/**
 * Comentario estilo PHPDoc:
 * Se utiliza para documentar funciones, clases o métodos.
 * Incluye etiquetas como @param y @return para una mejor descripción.
 * 
 * @param string $nombre Nombre del usuario
 * @return string Mensaje de saludo personalizado
 */

function saludar($nombre) {
    return "¡Hola, $nombre!";
}
```

[⬅️ Regresar al contenido.](../sintaxis_basica.md)