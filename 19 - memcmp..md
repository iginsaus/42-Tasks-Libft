SYNOPSIS:
```
#include <string.h>
int memcmp (const void *s1, const void *s2, size_t n);
```
##### Parámetros:
s1 - Puntero al primer bloque de memoria a comparar.
s2 - Puntero al segundo bloque de memoria a comparar.
n - Número de bytes a comparar.
##### Funcionamiento:
La función memcmp() compara los primeros ***n*** bytes de los bloques de memoria apuntados por ***s1*** y ***s2***. La comparación se realiza byte a byte, comparando cada byte de ***s1*** con el byte correspondiente en ***s2***.
Si los primeros ***n*** bytes de ambos bloques son iguales, la función devuelve ***0***. Si el primer byte que difiere es menor en ***s1*** que en ***s2***, la función devuelve un valor negativo. Si el primer byte es mayor en ***s1*** que en ***s***, la función devuelve un valor positivo.
