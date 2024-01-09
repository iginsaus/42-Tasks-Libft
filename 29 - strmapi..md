La función `ft_strmapi` de la biblioteca libft.h aplica una función a cada carácter de una cadena para crear una nueva cadena con la asignación dinámica de memoria. El prototipo de la función es el siguiente:

`char *ft_strmapi(char const *s, char (*f)(unsigned int, char));`

Donde `s` es la cadena a la que se aplicará la función y `f` es la función que se aplicará a cada carácter de la cadena. La función `f` toma como argumentos el índice del carácter y el carácter en sí, y devuelve el nuevo carácter resultante. A continuación se muestra un ejemplo de cómo se puede usar la función `ft_strmapi`:

```
#include "libft.h"
#include <stdio.h>

char add_index(unsigned int index, char c) {
    return c + index;
}

int main() {
    const char *str = "abc";
    char *new_str = ft_strmapi(str, &add_index);
    printf("La cadena resultante es: %s\n", new_str);
    // Salida esperada: "ace"
    return 0;
}
```

En este ejemplo, se define una función `add_index` que toma un índice y un carácter, y devuelve el carácter original más el índice. Luego, se aplica esta función a cada carácter de la cadena "abc" utilizando `ft_strmapi`, y se imprime la cadena resultante. La implementación de `ft_strmapi` implica la asignación dinámica de memoria para la nueva cadena y la iteración a través de cada carácter de la cadena original para aplicar la función especificada.
El índice de la cadena se utiliza para sumarlo al carácter correspondiente. Por lo tanto, al aplicar la función `add_index` a la cadena "abc", el índice se suma a cada carácter, como en el caso de a+0 = a, b+1 = c, y c+2 = e. El índice se obtiene automáticamente a medida que la función recorre la cadena, sin que necesites preocuparte por su implementación.

##### Referencias:
(https://github.com/15Galan/Libft)
(https://www.coursehero.com/file/110789092/ft-strmapic/)