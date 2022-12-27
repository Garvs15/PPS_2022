## Write a program to use switch statement.
```c
#include<stdio.h>
int main()
{
int i;
printf("Enter 1 for Fan, 2 for AC, 3 for Light, 4 for Heater : ");
scanf("%d",&i);
switch(i)
{
case 1 :
  printf("Fan On\n");
  break;
case 2 :
  printf("AC On\n");
  break;
case 3 :
  printf("Light On\n");
  break;
case 4 :
  printf("Heater On\n");
  break;
default :
  printf("Invalid Input\n");
  break;
}
 return 0;
}

**Output:- Enter 1 for Fan, 2 for AC, 3 for Light, 4 for Heater : 1
  Fan On
Enter 1 for Fan, 2 for AC, 3 for Light, 4 for Heater : 4
  Heater On
Enter 1 for Fan, 2 for AC, 3 for Light, 4 for Heater : 3
  Light On
 Enter 1 for Fan, 2 for AC, 3 for Light, 4 for Heater : 10
  Invalid Input
  ```     
