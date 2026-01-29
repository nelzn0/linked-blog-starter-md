Turn-in directory: ex02/
Files to turn in: ft_swap.c
Allowed functions: None

• Create a function that swaps the values of two integers using their addresses received as parameters.

• The function should be prototyped as follows:

![[Pasted image 20260129141112.png]]

`void ft_swap(int *a, int *b);`

## resolution

`//#include <stdio.h>`

`void    ft_swap(int *a, int *b)`
`{`
        `int temp;`

        `temp = *a;`
        `*a = *b;`
        `*b = temp;`
`}`

## testing

`//int   main(void)`
`//{`
`//      int n1 = 6;`
`//      int n2 = 7;`
`//      printf("number 1 is %d \n", n1);`
`//      printf("number 2 is %d \n", n2);`
`//      ft_swap(&n1, &n2);`
`//      printf("number 1 is now %d \n", n1);`
`//      printf("number 2 is now %d \n", n2);`
`//      return (0);`
`//}`

