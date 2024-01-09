La función `ft_substr` es una función de la biblioteca `libft`, la cual reserva y devuelve una subcadena de la cadena dada. Toma como parámetros la cadena original `s`, el índice de inicio `start` y la longitud máxima de la subcadena `len`. Devuelve la subcadena resultante o NULL si falla la reserva de memoria. Esta función utiliza la función `malloc` para la asignación dinámica de memoria. A continuación se muestra un ejemplo de prototipo de la función:

`char *ft_substr(char const *s, unsigned int start, size_t len);`

##### Fuentes:

(https://github.com/keulee/libft/blob/master/ft_substr.c)
(https://en.wikibooks.org/wiki/C_Programming/C_Reference/nonstandard/strlcpy)
(https://www.geeksforgeeks.org/c-library-string-h/)

##### Ejemplo:

El archivo C para la función `ft_substr` se vería así:

```                    
#include "libft.h"

char	*ft_substr(char const *s, unsigned int start, size_t len)
{
	char	*substr;
	size_t	s_len;
	size_t	substr_len;

	if (!s)
		return (NULL);
	s_len = ft_strlen(s);
	if (start >= s_len)
		return (ft_strdup(""));
	substr_len = (s_len - start < len) ? s_len - start : len;
	substr = (char *)malloc((substr_len + 1) * sizeof(char));
	if (!substr)
		return (NULL);
	ft_strlcpy(substr, s + start, substr_len + 1);
	return (substr);
}

```



Explicación paso a paso del código:

1. Se incluye el archivo de encabezado `libft.h`, que contiene los prototipos de las funciones y las definiciones de las estructuras utilizadas en la biblioteca `libft`.
2. Se define la función `ft_substr` con los parámetros especificados: una cadena `s`, un índice de inicio `start` y una longitud máxima `len`.
3. Se declara un puntero `substr` que se utilizará para almacenar la subcadena resultante.
4. Se obtiene la longitud de la cadena `s` utilizando la función `ft_strlen` de la biblioteca `libft`.
5. Se verifica si la cadena `s` es nula. En caso afirmativo, se devuelve NULL, ya que no se puede crear una subcadena a partir de una cadena nula.
6. Se comprueba si el índice de inicio `start` es mayor o igual que la longitud de la cadena `s`. Si es así, se devuelve una cadena vacía utilizando la función `ft_strdup` de la biblioteca `libft`.
7. Se calcula la longitud real de la subcadena, que es el mínimo entre la longitud restante de la cadena `s` a partir del índice `start` y la longitud máxima `len`.
8. Se reserva memoria para la subcadena utilizando la función `malloc`. La longitud de la subcadena se incrementa en 1 para el carácter nulo al final.
9. Se copia la subcadena de la cadena `s` a `substr` utilizando la función `ft_strlcpy` de la biblioteca `libft`. Se asegura que la subcadena esté terminada con un carácter nulo.
10. Se devuelve el puntero `substr` que apunta a la subcadena resultante.
