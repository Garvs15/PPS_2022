## Write a program to show the Factorial of a given number using recursion.
```c
#include<stdio.h>
// Program to calculate the factorial of a number.

long int fact(int n)
{
if(n <= 1)
return 1;
else
return fact(n - 1) * n;
}

int main()
{
int n;
printf("Enter the number: ");
scanf("%d", &n);
printf("Factorial of a %d  = %1d\n", n, fact(n));

return 0;
}

**Output:- Enter the number: 15
Factorial of a 15  = 2004310016
Enter the number: 13
Factorial of a 13  = 1932053504**

