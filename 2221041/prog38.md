## Write a program to reverse a string using strrev().
```c
#include <stdio.h>
#include <string.h>

//custom implementation of strrev() as it is non standard(not available in modern c libraries except Turbo C)
void strrev(char *str){
    int len = strlen(str);
    char temp;
    for(int i=0; i<len/2;i++){
        temp = str[i];
        str[i] = str[len-1-i];
        str[len-1-i] = temp;
    }
}

int main() {
    char str1[50],str2[50];
    printf("Enter a string -> ");
    scanf("%s",str1);
    strcpy(str2,str1);
    strrev(str2);
    printf("Reverse of %s = %s\n",str1,str2);

    return 0;
}
```
### Output:
```
Enter a string -> Automobile
Reverse of Automobile = elibomotuA
```
