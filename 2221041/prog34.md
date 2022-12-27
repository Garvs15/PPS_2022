## Write a program to copy a string into another using strcpy.
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str1[50],str2[50];
    printf("Enter a string -> ");
    scanf("%s",str1);
    strcpy(str2,str1);
    printf("String 1 - %s\n",str1);
    printf("String 2 - %s\n",str2);

    return 0;
}

```
### Output:
```
Enter a string -> Kingdom
String 1 - Kingdom
String 2 - Kingdom
```
