## Demonstration of fibonacci series upto n terms.
```c
#include<stdio.h>
int main()
{
int i, n;

// initialise  first and second term
int t1 = 0, t2 = 1;

// initialise the next term
int nextterm = t1 + t2;

//get no. of terms from the user
printf("Enter number of terms: ");
scanf("%d", &n);

// print the first two terms t1 and t2
printf("Fabonacci series: %d,%d, " , t1, t2);

// print 3rd to nth terms
for(i = 3; i<=n; ++i)
{
printf("%d, " , nextterm);
t1 = t2;
t2 = nextterm;
nextterm = t1 + t2;
}
return 0;
}

**Output:- Enter number of terms: 20
Fabonacci series: 0,1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, 987, 1597, 2584, 4181,
```
