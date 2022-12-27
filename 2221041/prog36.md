## Write a program to calculate the length of a string using strlen().
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str1[50];
    int len;
    printf("Enter a string -> ");
    scanf("%s",str1);
    len = strlen(str1);
    printf("Length of string - %d\n",len);

    return 0;
}


```
### Output:
```
Enter a string -> Ginger
Length of string - 6
```
