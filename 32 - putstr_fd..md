La función `ft_putstr_fd` se utiliza para escribir una cadena de caracteres en un descriptor de archivo específico.

- **Sinopsis o prototipo**:c
    
    `void ft_putstr_fd(char *s, int fd);`
    

- **Parámetros**:
    
    - `char *s`: La cadena de caracteres que se va a escribir.
    - `int fd`: El descriptor de archivo donde se escribirá la cadena.
    
- **Funcionamiento**:  
    La función `ft_putstr_fd` es parte de la biblioteca libft y se encarga de escribir la cadena de caracteres `s` en el descriptor de archivo `fd`. Emplea la llamada al sistema `write` para realizar la escritura en el descriptor de archivo especificado.
    
- **Ejemplo**:
    
```
#include "libft.h"

int main() {
    char *s = "Ejemplo";
    int fd = 1; // Descriptor de archivo 1 generalmente representa la salida estándar (stdout)
    ft_putstr_fd(s, fd);
    return 0;
}
```

- En este ejemplo, se incluye el encabezado de la biblioteca libft.h que contiene la declaración de `ft_putstr_fd`. Luego, se escribe la cadena "Ejemplo" en la salida estándar (descriptor de archivo 1) utilizando `ft_putstr_fd`.

En resumen, la función `ft_putstr_fd` se utiliza para escribir una cadena de caracteres en un archivo específico, cuyo destino se determina mediante el descriptor de archivo proporcionado como argumento.

##### Referencia:
(https://cpp.hotexamples.com/es/examples/-/-/ft_putchar_fd/cpp-ft_putchar_fd-function-examples.html).