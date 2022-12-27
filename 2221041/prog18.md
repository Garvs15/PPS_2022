## Demonstration of a program using a Bubble sort
```c
#include<stdio.h>
int array[8] = {25,57,48,37,12,92,86,33};
void bubble_sort(int a[], int N);
int main(void)
{
int i;
putchar('\n');
printf("Unsorted elements: , \n");
for(i = 0; i < 8; i++)
printf("%d ,",  array[i]);
bubble_sort(array, 8);
putchar('\n');
printf("Sorted elements: , \n");
for(i = 0; i < 8; ++i)
printf("%d , ",  array[i]);
return 0;
}
void bubble_sort(int a[], int N)
{
int i, j, temp;
for(i = 0; i < N; ++i)
for(j = 0; j < N - 1; j++)
if(a[j] > a[j+1])
  {
  temp = a[j];
  a[j] = a[j + 1];
 a[j + 1] = temp;
  }
}
 
 **Output:- Unsorted elements: 
25 ,57 ,48 ,37 ,12 ,92 ,86 ,33 ,
Sorted elements: , 
12 , 25 , 33 , 37 , 48 , 57 , 86 , 92 ,    

```

