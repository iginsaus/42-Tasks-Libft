SYNOPSIS:
```
#include <string.h>
void *memchr (const void *s, int c, size_t n);
```
##### Parámetros:
s - Puntero al bloque de memoria donde se realiza la búsqueda.
c - Carácter que se busca.
n - Número de bytes a analizar.
##### Funcionamiento:
La función memchr() busca la primera aparición del carácter ***c*** en los primeros ***n*** bytes del bloque de memoria apuntado por ***s***. La búsqueda se realiza byte a byte, comparando cada byte con ***c***.
Si la función encuentra el carácter ***c***, devuelve un puntero al byte encontrado. Si no lo encuentra en los primeros ***n*** bytes, devuelve un puntero a NULL.

NOTA: La función memchr() es equivalente a strchr(), pero memchr() funciona con bloques de memoria de cualquier tamaño, mientras strchr() solo funciona con cadenas de caracteres.
