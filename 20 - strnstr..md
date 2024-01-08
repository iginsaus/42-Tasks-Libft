SYNOPSIS:
```
#include <string.h>
char *strnstr(const char *haystack, const char *needle, size_t len);
```
##### Parámetros:
haystack - Puntero a la cadena donde se realizará la búsqueda.
needle - Puntero a la cadena que se buscará.
len - Número de bytes a analizar.
##### Funcionamiento:
La función strnstr() busca la primera aparición de la cadena ***needle*** en los primeros ***len*** bytes de la cadena ***haystack***. La búsqueda se realiza byte a byte, comparando cada byte de ***needle*** con los bytes correspondientes en ***haystack***. Si la función encuentra la cadena ***needle***, devuelve un puntero al byte inicial de ***needle*** en ***haystack***. Si no encuentra la cadena ***needle** en los primeros ***len*** bytes, devuelve un puntero ***NULL***.
