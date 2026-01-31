Turn-in directory: ex00/
Files to turn in: main.c, ft_putchar.c, rush0X.c
Allowed functions: write

Your program must display a rectangle on the screen and follow these requirements:

Files to submit:

• main.c

• ft_putchar.c

• rush0X.c, where "0X" represents the rush number (e.g., rush00.c).

◦ The next chapters will describe the specific constraints for each rush number.

Compilation:
• These three files will be compiled together.

• The ft_putchar.c file must contain the ft_putchar function.

Example of main.c file:

int main()
{
rush(5, 5);
return (0);
}

Function requirements:

• You must write a function called rush with the following specifications:

◦ It must take two integer arguments, named x and y.

◦ The function must be placed in the rush0X.c file.

• The function must be prototyped as follows:
void rush(int x, int y);

• Your rush function must display a rectangle on the screen with a width of x characters and a height of y characters.

• Your function must never crash or enter an infinite loop.

• Your main function will be modified during the defense to check whether you have handled all required cases.

Here is an example of a test that will be performed:

int main()
{
rush(123, 42);
return (0);
}

rush(5, 3) should display:

$>./a.out
o---o
|   |
o---o
$>
• rush(5, 1) should display:

$>./a.out
o---o
$>
• rush(1, 1) should display:

$>./a.out
o
$>
• rush(1, 5) should display:

$>./a.out
o
|
|
|
o
$>
• rush(4, 4) should display:

$>./a.out
o--o
|  |
|  |
o--o
$>