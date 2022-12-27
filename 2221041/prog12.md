## Write a program to demonstrate a comma operator.
```c
#include<stdio.h>
int main()
{
    int num=4,sq,cube;
    // Calculate the square and cube of the number
    sq = (num*num), cube = (num*num*num);
    printf("The square of %d is %d", num, sq);
    printf("\nThe cube of %d is %d", num, cube);
    return 0;
}
```
**Output:- The square of 4 is 16,
The cube of 4 is 64**
