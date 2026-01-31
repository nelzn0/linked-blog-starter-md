
`#include "ft_putchar.c"`

```
void    rush(int x, int y)
{

        int contx;
        int conty;

        contx = 0;
        conty = 1;

        while (x != contx)
        {
                contx++;
                if (contx == 1 || contx == x)
                {

                ft_putchar('o');
                }

                else
                {

                ft_putchar('-');

                }


        }
        while (y != conty)
        {
                conty++;
                if (conty == y )
                {

                        ft_putchar('\n');
                        ft_putchar('o');
                        ft_putchar('\n');
                }
                else
                {
                ft_putchar('\n');
                ft_putchar('|');
                }
        }

}
```