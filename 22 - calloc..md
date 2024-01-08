SYNOPSIS:
```
#include <stdlib.h>
void *calloc (size_t count, size_t size);
```
##### Parámetros:
count - Número de elementos que se van a reservar.
size - tamaño de cada elemento.

##### Funcionamiento:
La función calloc() reserva memoria para ***count*** elementos de tamaño ***size***.
La memoria reservada se inicializa todos a cero (inicializa todos los elementos de la memoria a cero).
La función calloc() devuelve un puntero a la memoria reservada. Si no se puede reservar la memoria, la función devuelve un puntero a NULL.
