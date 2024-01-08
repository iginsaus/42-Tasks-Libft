SYNOPSIS:
```
#include <string.h>
char *strchr (const char *s, int c);
```

##### Parámetros:
s - puntero a la cadena en la que se va a buscar el carácter.
c - carácter que se va a buscar.

##### Funcionamiento:
Busca la ***primera*** aparición de un carácter en una cadena.
1 - Inicializa un puntero a la cadena ***s***.
2 - Mientras el puntero no esté al final de la cadena, realiza las siguientes comprobaciones:
	- Si el carácter apuntado por el puntero es igual al carácter ***c***, la función devuelve el puntero.
	- Si el carácter apuntado por el puntero no es igual al carácter ***c***, el puntero avanza al siguiente carácter de la cadena.
	- Si el caracter ***c*** no se encuentra en la cadena, la función devuelve NULL.

[[strchr.pdf]]
[[15-strchr.pdf]]
