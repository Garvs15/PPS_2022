## Write a program to demostrate continue statement.
```c
#include<stdio.h>
int main()
{
int i;

for(i=0; i<10; i++) {
if (i==4) {
 continue;
}
printf("%d\n",i);
}
return 0;
}
```
### Output:- 
```
0
1
2
3
5
6
7
8
9
```
