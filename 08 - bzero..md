Establece los primeros n bytes del área de memoria apuntada por s a cero; más concretamente: La función *bzero()*  escribe **n** bytes a cero al string **s**. Si **n** es cero, evidentemente, *bzero()* no hace nada.


De las páginas man - SYNOPSIS:
```
#include <string.h> 
void bzero(void *s, size_t n);
```

Es importante tener en cuenta que la función `memset()` se prefiere para portabilidad, ya que `bzero()` ha sido designada como obsoleta en algunas especificaciones y puede ser retirada en futuras versiones.
https://man7.org/linux/man-pages/man3/bzero.3.html
https://pubs.opengroup.org/onlinepubs/009696899/functions/bzero.html
