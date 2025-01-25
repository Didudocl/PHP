# Salir de HTML

Cualquier cosa fuera de un par de etiquetas de apertura y cierre es ignorado por el intérprete de PHP, lo que permite que los ficheros de PHP tengan contenido mixto. Esto hace que PHP pueda ser embebido en documentos HTML para, por ejemplo, crear plantillas.

```php
<p>Esto va a ser ignorado por el intérprete de PHP.</p>
<?php echo 'Mientras que esto va a ser interpretado.'; ?>
<p>Esto tambien será ignorado.</p>
```

Esto ocurre debido a que el intérprete de PHP intercepta las etiquetas de cierre `?>`, simplemente comienza a imprimir cualquier cosa que encuentre hasta que dé con otra etiqueta de apertura a menos que se encuentre con una sentencia condicional, por ejemplo:

```php
<?php $expresion = true; ?>
<?php if ($expresion == true) : ?>
    Esto se mostrará si la expresión es verdadera.
<?php else: ?>
    En caso contrario se mostrará esto.
<?php endif; ?>
```

Output:

```md
Esto se mostrará si la expresión es verdadera
```

[⬅️ Regresar al contenido.](../sintaxis_basica.md)