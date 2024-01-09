La función `ft_putchar_fd` se utiliza para escribir un carácter en un descriptor de archivo específico.

SINOPSIS:
`void ft_putchar_fd (char c, int fd);

- **Parámetros**:
    
    - `char c`: El carácter que se va a escribir.
    - `int fd`: El descriptor de archivo donde se escribirá el carácter.
    
- **Funcionamiento**:  
    La función `ft_putchar_fd` es parte de la biblioteca libft, y su propósito es escribir el carácter `c` en el descriptor de archivo `fd`. Utiliza la llamada al sistema `write` para realizar la escritura en el descriptor de archivo especificado.
- **Ejemplo:
    
    ```
    ```

- En este ejemplo, se incluye el encabezado de la biblioteca libft.h que contiene la declaración de `ft_putchar_fd`. Luego, se escribe el carácter 'A' en la salida estándar (descriptor de archivo 1) utilizando `ft_putchar_fd`.

La función `ft_putchar_fd` es útil para escribir caracteres en un descriptor de archivo específico, lo que puede ser útil al trabajar con E/S en C.

Un descriptor de archivo es un identificador numérico que el sistema operativo asigna a un archivo abierto. En el contexto de la función `ft_putchar_fd`, el descriptor de archivo `fd` especifica dónde se escribirá el carácter.
Por ejemplo, el descriptor de archivo 1 generalmente representa la salida estándar (stdout), por lo que al usar `ft_putchar_fd('A', 1)`, el carácter 'A' se escribirá en la salida estándar. La salida esperada del uso de la función `ft_putchar_fd` es la escritura del carácter especificado en el descriptor de archivo indicado.
En el ejemplo anterior, el carácter 'A' se escribirá en la salida estándar, lo que significa que se mostrará en la pantalla. En resumen, la función `ft_putchar_fd` se utiliza para escribir un carácter en un archivo específico, cuyo destino se determina mediante el descriptor de archivo proporcionado como argumento.

##### Referencias:

(https://gitlab.com/TakuyaSama/42_madrid_cursus_libft/-/blob/master/ft_putchar_fd.c).
(https://github.com/mcombeau/libft/blob/main/ft_putchar_fd.c).
(https://es.wikipedia.org/wiki/Descriptor_de_archivo).