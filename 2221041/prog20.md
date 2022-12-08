## Demonstration of Binary Search.
```c
#include<stdio.h>
int main()
{
int range[50], T,i,j,NUM;
int first = 0, last, mid = 0, find = 0, search;
printf("Enter the total numbers in Array:");
scanf("%d", &NUM);
for(i = 0; i < NUM; i++)
{
 printf("Value %d, ", i+1);
scanf("%d", &range[i]);
}

// Sorting procedures before binary search.
for(i = 0; i < NUM - 1; i++)
{
 for(j = i +1; j < NUM; j++)
{
 if(range[i] > range[j])
{
 T = range[i];
 range[i] = range[j];
 range[j] = T;
  }
}
}
first = 0;
find = 0;
last = NUM - 1;
printf("The sorted elements are :");
for(i = 0; i < NUM; i++)
printf("%d\n", range[i]);

// Binary search procedure.
printf("\nEnter ther element to search in the above list:");
scanf("%d", &search);
while((first <= last) &&(find == 0))
{
mid =(first + last)/2;
if(range[mid] == search)
 find = mid;
else
  if(range[mid] < search)
 first = mid + 1;
else
 last = mid -1;
}
if(find > 0)
printf("\nThe position of the element is: %d", ++find);
else
printf("\nSearch not perfect");
 // To make auto break
return 0;
}
      
**Output:- Enter the total numbers in Array: 10
Value 1, 32
Value 2, 11
Value 3, 22
Value 4, 33
Value 5, 44
Value 6, 1
Value 7, 28
Value 8, 6
Value 9, 7
Value 10, 8
The sorted elements are :1
6
7
8
11
22
28
32
33
44

Enter ther element to search in the above list:22

The position of the element is: 6 
  ```
      
      
