La función `ft_putnbr_fd` se utiliza para escribir un número en un descriptor de archivo específico. 

- **Sinopsis o prototipo**:c
    
    `void ft_putnbr_fd(int n, int fd);`
    

- **Parámetros**:
    
    - `int n`: El número que se va a escribir.
    - `int fd`: El descriptor de archivo donde se escribirá el número.
    
- **Funcionamiento**:  
    La función `ft_putnbr_fd` es parte de la biblioteca libft y se encarga de escribir el número `n` en el descriptor de archivo `fd`. Emplea un enfoque recursivo o iterativo para descomponer el número en sus dígitos y luego escribirlos en el descriptor de archivo especificado.
- **Diferencia con las funciones anteriores**:  
    La principal diferencia entre `ft_putnbr_fd` y las funciones anteriores (`ft_putstr_fd` y `ft_putendl_fd`) es que `ft_putnbr_fd` está diseñada para escribir números, mientras que las otras dos funciones se utilizan para escribir cadenas de caracteres. Además, `ft_putnbr_fd` no agrega un salto de línea al final del número, a diferencia de `ft_putendl_fd`.
- **Ejemplo**:
```
#include "libft.h"

int main() {
    int num = 42;
    int fd = 1; // Descriptor de archivo 1 generalmente representa la salida estándar (stdout)
    ft_putnbr_fd(num, fd);
    return 0;
}
```


- En este ejemplo, se incluye el encabezado de la biblioteca libft.h que contiene la declaración de `ft_putnbr_fd`. Luego, se escribe el número 42 en la salida estándar (descriptor de archivo 1) utilizando `ft_putnbr_fd`.

En resumen, la función `ft_putnbr_fd` se utiliza para escribir un número en un archivo específico, cuyo destino se determina mediante el descriptor de archivo proporcionado como argumento. A diferencia de las funciones anteriores, esta función está diseñada para manejar la escritura de números en lugar de cadenas de caracteres.

##### Referencias:
(https://github.com/elidlocke/libft/blob/master/src/ft_putnbr_fd.c).
(https://cpp.hotexamples.com/es/examples/-/-/ft_putchar_fd/cpp-ft_putchar_fd-function-examples.html).