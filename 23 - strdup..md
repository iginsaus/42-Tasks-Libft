SYNOPSIS:
```
#include <string.h>
char *strdup (const char *s1);
```
##### Parámetros:
s1 - Puntero a la cadena de caracteres que se va a duplicar.

##### Funcionamiento:
La función strdup() devuelve un puntero a una nueva cadena de caracteres que es un duplicado de la cadena apuntada por ***s1***.
La memoria para la nueva cadena se obtiene automaticamente con malloc(), y debe (y puede) liberarse con free().
La función strdup() comienza leyendo la cadena ***str*** byte a byte, comenzando por el primer byte. Cada byte es copiado a la nueva cadena.
La nueva cadena termina en un carácter nulo (\\0).
Si no hay suficiente memoria para la nueva cadena, la función devuelve un puntero a NULL.
