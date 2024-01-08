La función memcpy() copia **n** bytes del área de memoria **src** al área de memoria **dest**. Las áreas de memoria no deben solaparse. Si las areas de memoria van a solaparse debe usarse *memmove(3)*.

De las páginas man BSD - SYNOPSIS:
```
#include <string.h> 
void *memcpy(void *restrict dst, const void *restrict src, size_t n);
```

[[memcpy.pdf]]

NOTA: Lás páginas man de Linux (aqui en pdf) muestran una ligera diferencia con las páginas man de la  Biblioteca BSD del Manual de Funciones de los Mac.
Usamos las del Mac; pero hay que tener en cuenta por ejemplo en este caso que la última actualización del BSD del Mac para esta función es del 04-Jun-1993; mientras la de Linux es del 29-Dec-2022.
[[9-memcpy.pdf]]

