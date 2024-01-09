La función `ft_strjoin` de la biblioteca libft.h se utiliza para concatenar dos cadenas de caracteres. Toma como argumentos las dos cadenas que se desean unir y devuelve una nueva cadena que resulta de la concatenación de las dos cadenas de entrada. Es importante recordar que la cadena resultante debe ser liberada con la función `free` una vez que ya no se necesite para evitar fugas de memoria. La implementación típica de la función `ft_strjoin` en la biblioteca libft.h es similar a la siguiente:

```
char	*ft_strjoin(const char *s1, const char *s2)
{
	size_t	len1;
	size_t	len2;
	char	*result;

	if (!s1 || !s2)
		return (NULL);
	len1 = ft_strlen(s1);
	len2 = ft_strlen(s2);
	result = (char *)malloc(sizeof(char) * (len1 + len2 + 1));
	if (!result)
		return (NULL);
	ft_strlcpy(result, s1, len1 + 1);
	ft_strlcat(result, s2, len1 + len2 + 1);
	return (result);
}
```

Esta implementación primero obtiene la longitud de las dos cadenas de entrada, luego asigna memoria para la cadena resultante y finalmente copia y concatena las cadenas de entrada en la cadena resultante. Es importante realizar las verificaciones adecuadas, como comprobar si las cadenas de entrada son nulas y si la asignación de memoria fue exitosa, para garantizar un comportamiento seguro de la función. 

#####  Referencias:

(https://github.com/vittoric/Libft)
(https://giters.com/caroldaniel/42sp-cursus-libft)