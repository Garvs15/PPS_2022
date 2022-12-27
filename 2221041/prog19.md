## Search an element and its position in an array(Linear search).
```c
#include<stdio.h>
int main()
{
int num[10], i, pos = 0, value;
printf("Please enter the values ");
for(i = 0; i < 10; i++)
{
   scanf("%d", &num[i]);
}
printf("Enter search value ");
scanf("%d", &value);
for(i = 0; i < 10; ++i)
{
  if(value ==num[i])
  {
 pos = i + 1;
  }
}
printf("The search value %d's position is %d", value, pos);
return 0;
}

## Output:- Please enter the values 32
11
22
33
44
1
28 
6
7
8
Enter search value 11
The search value 11's position is 2                                                                                                                                                                        
```
