## Write a program to demonstrate the swapping of two variables by using a temporary variable.
```c
#include<stdio.h>
int main()
{
int n1, n2;
printf("Enter first number -> ");
scanf("%d", &n1);
printf("Enter second number -> ");
scanf("%d", &n2);

int temp = n1;
n1 = n2;
n2 = temp;

printf("\nAfter swapping:\n");
printf("First number -> %d\n", n1);
printf("Second number -> %d\n", n2);

return 0;
}

## Output: Enter first number -> 50
Enter second number -> 30

After swapping:
First number -> 30
Second number -> 50
```
