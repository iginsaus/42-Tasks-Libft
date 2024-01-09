La función `ft_split` de la biblioteca libft.h se utiliza para dividir una cadena en subcadenas basadas en un delimitador especificado. El prototipo de la función es el siguiente:

`char	**ft_split(const char *s, char c);`

Donde `s` es la cadena que se va a dividir y `c` es el carácter delimitador. La función devuelve un array de cadenas (también conocido como matriz de cadenas) que representan las subcadenas resultantes de la división. A continuación se muestra un ejemplo de cómo se puede usar la función `ft_split`:

```
#include "libft.h"
#include <stdio.h>

int main() {
    const char *str = "Ejemplo-de-cadena-a-dividir";
    char **result = ft_split(str, '-');
    int i = 0;
    while (result[i] != NULL) {
        printf("%s\n", result[i]);
        i++;
    }
    // Salida esperada: "Ejemplo", "de", "cadena", "a", "dividir"
    return 0;
}

```

En este ejemplo, la cadena "Ejemplo-de-cadena-a-dividir" se divide en subcadenas utilizando el delimitador '-'. El resultado es un array de cadenas que contiene las subcadenas resultantes.

##### Referencias:
(https://github.com/krios-fu/libft/blob/master/ft_split.c)
(https://cpp.hotexamples.com/es/examples/-/-/ft_strsub/cpp-ft_strsub-function-examples.html)