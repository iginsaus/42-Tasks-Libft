SYNOPSIS:
```
#include <string.h>
int strncmp (const char *s1, const char *s2, size_t n);
```
##### Parámetros:
s1 - Un puntero a la primera cadena a comprobar.
s2 - Un puntero a la segunda cadena a comprobar.
n - El número de caracteres a comprobar.
##### Funcionamiento:
- La función compara los primeros ***n*** carácteres de las cadenas ***s1*** y ***s2***.
- Si las cadenas son iguales, la función devuelve 0.
- Si la primera cadena es menor que la segunda cadena, la función devuelve un valor negativo.
- Si la primera cadena es mayor que la segunda cadena, la función devuelve un valor positivo.
