## Program 33: Write a program to check if a given word is palindromic or not.
```c 
#include <ctype.h>
#include <stdio.h>
#include <string.h>

//Program to check if given word is a palindrome

void toLowerCase(char *word){
    for(int i=0; i<strlen(word); i++){
        word[i] = tolower(word[i]);
    }
}

int isPalindrome(char *word){
    char rev[strlen(word)];
    
    for(int i=strlen(word);i>=0;i--)rev[strlen(word)-1-i] = word[i];

    printf("Reverse of %s -> %s\n",word,rev);
    if(strcmp(word,rev) == 0) return 1;
    return 0;
}

int main(){
    char word[25];

    printf("Enter a word to check -> ");
    scanf("%s",word);
    toLowerCase(word);

    if(isPalindrome(word))printf("%s is a palindrome\n",word);
    else printf("%s is not a palindrome\n",word);
    
    return 0;
}

```
### Output:
```
Enter a word to check -> madam
Reverse of madam -> madam
madam is a palindrome
```
```
Enter a word to check -> RAceCAr
Reverse of racecar -> racecar
racecar is a palindrome
```
```
Enter a word to check -> Risk
Reverse of risk = kisr
risk is not a palindrome
```

