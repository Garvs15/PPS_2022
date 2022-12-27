## Write a program to concatenate a string using strcat().
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str1[50],str2[50];
    printf("Enter a string -> ");
    scanf("%s",str1);
    printf("Enter another string -> ");
    scanf("%s",str2);
    strcat(str1,str2);
    printf("Concatenated String - %s\n",str1);

    return 0;
}

```
### Output:
```
Enter a string -> Kingdom
String 1 - Kingdom
String 2 - Kingdom
```
