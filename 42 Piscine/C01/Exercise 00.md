Turn-in directory: ex00/
Files to turn in: ft_ft.c
Allowed functions: None

• Create a function that takes a pointer to an int as a parameter and sets the value of that int to "42".

• The function should be prototyped as follows:

![[Pasted image 20260129140925.png]]

`void ft_ft(int *nbr);`

//#include <stdio.h>

`void	ft_ft(int *nbr)`
`{`
	`*nbr = 42;`
`}`

## to test it

cc -Wall -Wextra -Werror

`//int	main(void)`
`//{`
`//	int n = 5;`
`//	printf("number before: %d \n", n);`
`//`
`//	ft_ft(&n);`
`//`	
`//	printf("number after: %d \n", n);`
`//	return (0);`
`//}`


`*(value)` = points to the address of a value

on main, just added a `var n` (number)

added a `printf`, from library `stdio.h`

`%d` = so it can print a int argument, as a placeholder

if u use `%s`, it would be to print a string, on

printing the number of choice (i chose 5)

afterwards, ran the function `ft_ft` on the var `n`

printed again the same number, which after the function, will switch from 5 to 42



