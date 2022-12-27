## Write a Program to compare two strings using strcmp().
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str1[50],str2[50];
    printf("Enter a string -> ");
    scanf("%s",str1);
    printf("Enter another string -> ");
    scanf("%s",str2);

    int x = strcmp(str1,str2);
    if(x>0)printf("First string is greater/longer\n");
    else if(x<0)printf("First string is smaller/lesser\n");
    else printf("Both strings are equal\n");

    return 0;
}
```
### Output:
```
Enter a string -> Cat
Enter another string -> Kitten
First string is smaller/lesser
```
```
Enter a string -> Dog
Enter another string -> Puppy
First string is smaller/lesser
```
```
Enter a string -> Bat
Enter another string -> Bat
Both strings are equal
```
