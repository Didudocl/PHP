# Separación de instrucciones

PHP requiere que las instrucciones terminen en `punto y coma` al final de cada sentencia. La etiqueta de cierre de un bloque de código de PHP automáticamente implica un punto y coma.

```php
<?php
    echo 'Esto es una prueba';
?>

<?php echo 'Esto es una prueba' ?>

<?php echo 'Hemos omitido la última etiqueta de cierre';
```

Output:

```markdown
Esto es una prueba
Esto es una prueba
Hemos omitido la última etiqueta de cierre
```