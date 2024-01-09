La función `ft_strtrim` de la biblioteca libft.h se utiliza para eliminar los caracteres especificados al principio y al final de una cadena. Toma como argumentos la cadena de la que se desean eliminar los caracteres y un conjunto de caracteres que se quieren eliminar, y devuelve una nueva cadena que representa la cadena original sin los caracteres especificados al principio y al final. La implementación típica de la función `ft_strtrim` es la siguiente:

```
char	*ft_strtrim(const char *s1, const char *set)
{
	size_t	start;
	size_t	end;
	char	*trimmed;

	if (!s1)
		return (NULL);
	start = 0;
	while (s1[start] && ft_strchr(set, s1[start]))
		start++;
	end = ft_strlen(s1);
	while (end > start && ft_strchr(set, s1[end - 1]))
		end--;
	trimmed = ft_substr(s1, start, end - start);
	return (trimmed);
}
```

En esta implementación, se buscan los índices de inicio y fin de la subcadena que no contiene caracteres del conjunto especificado. Luego, se utiliza la función `ft_substr` para extraer la subcadena sin los caracteres especificados al principio y al final. Es importante realizar la verificación adecuada para la cadena de entrada, en este caso, si es nula, para garantizar un comportamiento seguro de la función. 

##### Referencias:

(https://github.com/Oksanatishka/42_libft/blob/master/ft_strtrim.c)
(https://www.nicolamanzini.com/libft-my-own-first-c-library/)