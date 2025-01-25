# Booleanos

Un dato de tipo booleano expresa un valor que indica verdad. Puede ser `true (verdadero)` o `false (falso)`.

### Sintaxis

Para especificar un literal de tipo booleano se emplean las constantes true o false. Ambas no son susceptibles a mayúsculas y minúsculas.

```php
<?php
#foo = True;    // Asigna el valor TRUE a $foo
?>
```

Usualmente, el resultado de un operador que devuelve un valor de tipo booleano es pasado a una estructura de control, como se puede ver en el siguiente ejemplo:

```php
<?php
/*
 * // == es un operador que comprueba la
 * igualdad y devuelve un booleano
*/
if ($accion == "mostrar_version") {
    echo "La versión es 1.23";
}

// Esto no es necesario...
if ($mostrar_separadores = TRUE) {
    echo "Hola";
}

// ... Porque se puede escribir simplemente de la siguiente manera:
if ($mostrar_separadores) {
    echo "Hola";
}
?>
```

### Conversión a booleano

Para convertir explícitamente un valor al tipo booleano, se utilizan los amoldamientos `bool` o `boolean`, como se puede ver en el ejemplo:

```php
<?php
var_dump((bool) "");        // bool(false)
var_dump((bool) 0);         // bool(false)
var_dump((bool) 1);         // bool(true)
var_dump((bool) -2);        // bool(true)
var_dump((bool) "foo");     // bool(true)
var_dump((bool) 2.3e5);     // bool(true)
var_dump((bool) array(12)); // bool(true)
var_dump((bool) array());   // bool(false)
var_dump((bool) "false");   // bool(true)
?>
```

[⬅️ Regresar a tipos de datos.](../tipos.md)