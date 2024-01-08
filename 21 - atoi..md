SYNOPSIS:
```
#include <stdlib.h>
int atoi (const char *str);
```
##### Parámetros:
str - Puntero a la cadena de caracteres que se va a convertir en un entero.
##### Funcionamiento:
La función atoi() convierte la cadena de caracteres ***str*** en un número entero. La cadena de caracteres ***str*** debe contener un número entero en formato decimal, con o sin signo.
La función atoi() comienza leyendo la cadena ***str*** byte a byte, comenzando por el primer byte. Cada byte es interpretado como un dígito decimal.
Si la función encuentra un carácter que no es un dígito decimal, la función termina la conversión y devuelve el valor convertido hasta ese momento.
Si la función encuentra un carácter de signo (+ o -), el signo se ignora para los números sin signo. Para los números con signo, el carácter de signo determina el signo del número convertido.
Si la cadena ***str*** no contiene un número entero válido, la función devuelve ***0***.

**NOTA**: La función atoi() no es segura contra desbordamiento. Si la cadena ***str*** contiene un número entero que es demasiado grande para el tipo int, la función atoi() devoverá un valor incorrecto.
