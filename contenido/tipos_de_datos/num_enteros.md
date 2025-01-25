# Números enteros (Integers)

Un número entero es un número del conjunto ℤ = {..., -2, -1, 0, 1, 2, ...}. En programación, los enteros son esenciales para representar conteos, índices, identificadores y otros valores discretos.

### Sintaxis

Los enteros pueden especificarse mediante notación decimal (base 10), hexadecimal (base 16), octal (base 8) o binario (base 2), opcionalmente precedidos por un signo (- o +).

```php
<?php
$a = 1234;      // Número con notación decimal positivo
$a = -123;      // Número con notación decimal negativo
$a = 0123;      // Número con notación octal (equivale a 83 en notación decimal)
$a = 0x1A;      // Número con notación hexadecimal (equivale a 26 en notación decimal)
$a = 0b1111111; // Número con notación binaria (equivale a 255 en notación decimal)  
```

Formalmente, la estructura de los literales de tipo entero es:

- Notación decimal: `[1-9][0-9]* | 0`
- Notación hexadecimal: `0[xX][0-9a-fA-F]+`
- Notación octal: `0[0-7]+`
- Notación binaria: `0b[01]+`

### Conversión a números enteros

Para convertir explícitamente un valor al tipo entero se puede emplear tanto **int** como **integer**. Sin embargo, la mayoría de las veces la conversión no es necesaria, ya que un valor es convertido de forma automáticamente cuando un operador, función o estructura de control requiera un argumento de tipo entero.

```php
<?php
$a = true;          // Booleano
$b = (int)$a;       // Conversión explícita a entero (1)
$c = (integer)$a;   // Conversión equivalente (1)
```

[⬅️ Regresar a tipos de datos.](../tipos.md)