Turn-in directory: ex03/
Files to turn in: ft_print_numbers.c
Allowed functions: write

• Create a function that displays all digits on a single line, in ascending order.

• The function should be prototyped as follows:

![[Pasted image 20260128192520.png]]

## solution

apparently, I cannot use int just yet.. only if I converted it

seems like this write function is mostly compatible with char

`#include <unistd.h>`

`void ft_print_numbers(void)`
`{`
        `char number;`
        `{`
                `number = '0';`
                `while (number <='9')`
                `{`
                        `write(1, &number, 1);`
                        `number++;`
                `}`
        `}`
`}`


## to test it

`int main(void)`
`{`
        `ft_print_numbers();`
        `return (0);`
`}`


## IF i wanted to convert it (perplexity suggested)

`#include <unistd.h>`

`void ft_print_numbers(void)`
`{`
		`int n;`
        `char number;`
        `{`
                `number = '0';`
                `while (number <='9')`
                `{`
			            `number = n + '0';`
                        `write(1, &number, 1);`
                        `number++;`
                `}`
        `}`
`}`

I would have to still have a char var, but create also a int var

then, inside the while loop, I would need to store in number, the conversion of n (0) to the char value '0'

