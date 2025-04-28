
# EX-06 - Looping  
## AIM:  
Write a C program to print even numbers ranging from M to N (including M and N values).

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int M, N, i;
    scanf("%d%d", &M, &N);
    for (i = M; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }
    printf("\n");
    return 0;
}
```

## OUTPUT:
```
Input:
3 10
Output:
4 6 8 10
```

## RESULT:  
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully.


# EX-07 - Nested-loop  
## AIM:  
Write a C program to print the given triangular pattern using loop.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int rows, i, j;
    scanf("%d", &rows);
    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= i; j++) {
            printf("* ");
        }
        printf("\n");
    }
    return 0;
}
```

## OUTPUT:
```
Input:
5
Output:
* 
* * 
* * * 
* * * * 
* * * * * 
```

## RESULT:  
Thus the program to print the given triangular pattern using loop has been executed successfully.


# EX-08 - Functions  
## AIM:  
Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## PROGRAM:
```c
#include <stdio.h>
void addition(int a, int b) {
    printf("Addition: %d\n", a + b);
}
void subtraction(int a, int b) {
    printf("Subtraction: %d\n", a - b);
}
int main() {
    int num1, num2;
    scanf("%d%d", &num1, &num2);
    addition(num1, num2);
    subtraction(num1, num2);
    return 0;
}
```

## OUTPUT:
```
Input:
8 3
Output:
Addition: 11
Subtraction: 5
```

## RESULT:  
Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully.


# EX-09 - Use For Loop  
## AIM:  
Write a C program to find the sum of odd digits using for loop.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int num, digit, sum = 0;
    scanf("%d", &num);
    for (; num > 0; num /= 10) {
        digit = num % 10;
        if (digit % 2 != 0) {
            sum += digit;
        }
    }
    printf("Sum of odd digits: %d\n", sum);
    return 0;
}
```

## OUTPUT:
```
Input:
12345
Output:
Sum of odd digits: 9
```

## RESULT:  
Thus the program to find the sum of odd digits using for loop has been executed successfully.


# EX-10 - Factorial of a Number Using a Function  
## AIM:  
To write a C program that calculates the factorial of a given number using a user-defined function.

## PROGRAM:
```c
#include <stdio.h>
void fact() {
    int i, N, factorial = 1;
    scanf("%d", &N);
    for (i = 1; i <= N; i++) {
        factorial *= i;
    }
    printf("Factorial of %d is %d\n", N, factorial);
}
int main() {
    fact();
    return 0;
}
```

## OUTPUT:
```
Input:
5
Output:
Factorial of 5 is 120
```

## RESULT:  
The program correctly computes the factorial of a given number using a separate function and displays the result.


