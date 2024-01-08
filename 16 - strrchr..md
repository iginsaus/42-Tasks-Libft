SYNOPSIS:
```
#include <string.h>
char *strrchr (const char *s, int c);
```
##### Parámetros:
s - puntero a la cadena en la que se va a buscar el carácter.
c - carácter que se va a buscar.

##### Funcionamiento:
1 - La función comienza a buscar el caracter ***c*** desde el ***final*** de la cadena ***s***.
2 - Si encuentra el carácter ***c***, la función devuelve un puntero al carácter ***c***.
3 - Si no encuentra el carácter ***c***, la función devuelve un puntero a NULL.

NOTA: La diferencia entre **strchr** y **strrchr**, es que la primera comienza la búsqueda desde el principio de la cadena, mientras la segunda comienza la busqueda desde el final de la cadena.
