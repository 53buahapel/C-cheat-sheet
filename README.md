# GOD Programming Language (Cheat sheet)

![](https://www.britefish.net/wp-content/uploads/2019/07/logo-c-1.png)

## Comment

```c 
// This is a comment

/* 
This is also comment 
*/
```
## Data types

**character**

- unsigned char range `0 to 255`
- char range `-128 to 127`

**integer**

- unsigned int range `0 to 65535`
- int range `-32768 to 32767`
- unsigned long range `0 to 4294967295`
- long range `-2147483648 to 2147483647`

**decimal**

- float range `1.2e-38 to 3.4e+38`
- double range `2.3e-308 to 1.7e+308`
- long double `more bigger than float`

## format types

- `%c` (character)
- `%s` (string)
- `%i, %d` (integer)
- `%f, %e` (float)
- `%o` (octal)
- `%x` (hexadecimal)
- `%u` (unsigned)

## Variables

**syntax**

Datatypes variable = value;

```c
#include <stdio.h>

void main(){
    int a = 10;
    char b = 'A';
    float c = 1.2;
    printf("int a = %d \nchar b = %c \nfloat c = %f\n", a, b, c);

    // you can specify float number with %.<num>f //
    printf("====================\n");
    printf("float c = %.1f\n", c);
    printf("float c = %.2f\n", c);
}
```

**output:**
```
int a = 10
char b = A
float c = 1.200000
====================
float c = 1.2
float c = 1.20
```

## constant

It's same like variable but it's not changeable.
example:

```c
#define PI 3.14
#define Name "kyruuu."
```

## Output

- **printf** (show **all output** types)
- **puts** (only show **string** and give **new line**)
- **putchar** (only show **one** string)

## Input

- **scanf** (input data types **num, char, and string**)
- **gets** (input **string and char**)  *dangerous command* use fgets() instead
- **getchar** (input **char**)
- **getch** (input **char  data** `no preview` usually to input password)
- **getche** (input **char data**)

```c
#include <stdio.h>

void main(){
    int age;
    char name[20];    // we can use array to input string

    printf("Enter your age: ");
    scanf("%d", &age);
    printf("Enter your name: ");
    scanf("%s", name);
    
    printf("Your age is %d\n", age);
    printf("Your name is %s\n", name);
}
```
