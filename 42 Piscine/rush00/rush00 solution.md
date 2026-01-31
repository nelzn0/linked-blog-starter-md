
```
void	ft_putchar(void);

char	ft_symbols(int contx, int conty, int x, int y)
{
	if ((conty == 1 && contx == 1) || (conty == 1 && contx == x)
		|| (conty == y && contx == 1) || (conty == y && contx == x))
	{
		return ('o');
	}
	if (conty == 1 || conty == y)
	{
		return ('-');
	}
	if (contx == 1 || contx == x)
	{
		return ('|');
	}
	return (' ');
}

void	ft_print(int x, int y)
{
	int	contx;
	int	conty;

	conty = 1;
	while (conty <= y)
	{
		contx = 1;
		while (contx <= x)
		{
			ft_putchar(ft_symbols(contx, conty, x, y));
			contx++;
		}
		ft_putchar('\n');
		conty++;
	}
}

void	rush(int x, int y)
{
	ft_print(x, y);
}

```