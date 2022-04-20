# About Project

The printf project is a collaboration between Emmanuel Nyarko-[Emmankoko](https://github.com/Emmankoko)  and Henry Quaye -[jayamon99](https://github.com/jayamon99) .Two students currently enrolled in the ALX Software Engineering Training program - a 12 months training program that nurtures potential and molds student into top-notch software engineers. The printf projects focuses on a _printf() function created based on the printf() function located in the stdio.h library.

>_printf() variadic function produces output according to a format specifier(s). A variadic function is a function that accepts a variable number of arguments. If the last parameter of a function definition is prefixed by ellipsis ..., then the function can accept any number of arguments for that parameter.
>
>_printf prototype: int_printf(const char *format, ...).

**Below we look at the various format specifiers and their data type outputs**

|  Specifier |Output Datatype |
| ------------ | ------------ |
| c  | char(character)  |
| d or i  | signed decimal or integer  |
| u   | unsigned int(integer)  |
| s   |  string(character array)   |
| b  | signed binary  |
| o  | signed octal  |
| x  | unsigned hexadecimal  |
| X  | unsigned hexadecimal(uppercase)  |
| p  | pointer address  |
| r  | reverse string of characters  |
| R  | ROT13 translating of string  |
| S  | string with special chars replaced by their ASCII values  |
| %    | character    |

|Flags   | Descriptions  | Specifier  |
| ------------ | ------------ | ------------ |
| +  | prints a plus sign(+) when the argument is positive and a minus sign(-) when otherwise.  |  i,d  |
|(space)   | prints a blank space if the argument is a positive number.  | i,d  |
|(#)| prints 0,0x and 0X for o,x and X specifier respectively. it doesn't print anything if argument is zero.|o,x,X|

| Length  |Description   | Specifier  |
| ------------ | ------------ | ------------ |
| l  |prints along int or unsigned long int   |i,d,o,u,x and X   |
| h  |prints a short int or unsigned short int   |i,d,o,u,x and X   |

### Use Cases of _printf() on format specifiers

1.Printing the string of characters "Hello World"

>Use Case:
>int main() {
>
> printf("%s", "Hello World");
> return 0;
>}
>Output: Hello World

2.Printing an integer number:

>Use case:
>int main() {
>
> printf("Hello contains %d characters", 5);
> return 0;
>}
>Output: Hello contains 5 characters

3.Printing a decimal, octal and hexadecimal:

>Use case:
>int main ()
>{
> int value = 2567;
>
> printf("Decimal value is: %d\n",value);
> printf("Octal value is: %o\n",value);
> printf("Hexadecimal value is (Alphabet in small letters): %x\n",value);
> printf("Hexadecimal value is (Alphabet in capital letters): >%X\n",value);
>
> return 0;
>}
>Output: Decimal value is: 2567
 >>Octal value is: 5007
 >>Hexadecimal value is (Alphabet in small letters): a07
 >>Hexadecimal value is (Alphabet in capital letters): A07

### Using flags and length tags

1.Printing signed integers:

>Use Case:
>int main()
>{
> printf("%+d %+i",10,-10);
> return 0;
>}
>Output: +10 -10

2.Printing a long integer number and short integer number:

>Use Case:
>int main() {
>
> printf("%ld, %hd", 1000000, 1000000);
> return 0;
>}
>Output: 1000000, 16960
