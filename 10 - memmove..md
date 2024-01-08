Copia un bloque de memoria de una ubicación a otra, incluso si los bloques se superponen.

De las páginas man Linux - SYNOPSIS:
```
#include <string.h> 
void *memmove(void dest[.n], const void src[.n], size_t n);
```

De las páginas man Mac - SYNOPSIS:
```
#include <string.h> 
void *memmove(void *dst, const void *src, size_t len);
```

##### Los parámetros son:
dst - Puntero a la ubicación de destino.
src - Puntero a la ubicación de origen.
len - Número de bytes a copiar.
##### Funcionamiento:
1 - Comprueba si los bloques de memoria se superponen.
2 - Si los bloques no se superponen, copia los bytes directamente de origen al destino.
3 - Si los bloques se superponen, copia los bytes a un bufer temporal. A continuación, copia los bytes del buffer temporal a la ubicación de destino.

El anterior memcpy - Copia los bytes directamente de la ubicación de origen a la ubicación de destino.
