Copia una cadena en otra, asegurando que no se desborde el búfer de destino.

De las páginas man - SYNOPSIS:
```
#include <string.h>
size_t strlcpy(char *restrict dst, const char *restrict src, size_t dstsize);
```

Esta función copia hasta `size - 1` caracteres desde la cadena `src` terminada en NUL a la cadena `dst`, terminando el resultado con NUL. Devuelve la longitud de `src`; si el valor devuelto es mayor o igual que `size`, se produjo una truncación. La función no es estándar en ISO, pero está disponible en varias bibliotecas en sistemas Unix, incluyendo BSD, Mac OS X, Solaris, Android e IRIX, con la notable excepción de glibc en Linux.
La función `strlcpy` no se encuentra en la biblioteca estándar de C, por lo que no es necesario incluir ninguna librería específica para su uso.

(https://ld2011.scusa.lsu.edu/cppreference/wiki/c/string/strlcpy)

(https://en.wikibooks.org/wiki/C_Programming/C_Reference/nonstandard/strlcpy)

(https://linux.die.net/man/3/strlcpy)

La sintaxis de la función es `size_t strlcpy(char *dst, const char *src, size_t size);`[

La función `strlcpy` es una alternativa más segura a `strcpy` y `strncpy`, diseñada para ser más fácil de usar correctamente, ya que toma el tamaño completo del búfer y garantiza la terminación con NUL del resultado, siempre que el tamaño sea mayor que 0[

(https://linux.die.net/man/3/strlcpy)

[[strlcpy.pdf]]
[[11.strlcpy.pdf]]

