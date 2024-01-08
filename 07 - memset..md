Rellena un bloque de memoria con un valor específico.

De las páginas man (Linux) - SYNOPSIS:
```
#include <string.h>
void *memset(void s[.n], int c, size_t n);
```

De las páginas man (Mac) - SYNOPSIS:
```
#include <string.h>
void *memset(void *b, int c, size_t len);
```

La función `memset` en C se utiliza para llenar un bloque de memoria con un valor particular. Su sintaxis es la siguiente: `void *memset(void *ptr, int x, size_t n)`. Donde:

- `ptr` es la dirección de inicio de la memoria a llenar.
- `x` es el valor a llenar.
- `n` es el número de bytes a llenar a partir de `ptr`

**INFORMACION**:
(https://www.geeksforgeeks.org/memset-c-example/)
(https://www.tutorialspoint.com/c_standard_library/c_function_memset.htm).
