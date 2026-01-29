Turn-in directory: ex02/
Files to turn in: ft_print_reverse_alphabet.c
Allowed functions: write

• Create a function that displays the alphabet in lowercase, on a single line, in descending order, starting from the letter ’z’.

• The function should be prototyped as follows:

![[Pasted image 20260128192423.png]]

same thing, but reverse

## solution

`#include <unistd.h>`

`void ft_print_reverse_alphabet(void)`
`{`
        `char letter;`
        `{`
                `letter = 'z';`

                `while (letter >= 'a')`
                `{`
                        `write(1, &letter, 1);`
                        `letter--;`
                `}`
        `}`
`}`

same things BUT

while z is greater or equal than a

then

write

and this time, decrease the var letter (letter-1)

## to test

`int main (void)`
`{`
        `ft_print_reverse_alphabet();`
        `return (0);`
`}`
