## Program 14: Write a program to use goto statement.

```c
#include <stdio.h>

int main(){
    int i = 0;
    start:
    printf("%d\t",i);
    i++;
    if(i<10)goto start;

    return 0;
}
```

### Output:
```
0	1	2	3	4	5	6	7	8	9
