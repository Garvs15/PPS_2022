## Write a program to show that given number is Palindromic or not.
```c
#include<stdio.h>

// Program to check if given number is palindrome or not.

int reverse(int n)
{
int rev  = 0;
while(n > 0)
{
rev = rev * 10 + n % 10;
n/=10;
}
return rev;
}

int isPalindrome(int n)
{
if(reverse(n) == n)
return 1;
return 0;
}

int main()
{
int n;
printf("Enter a number to check -> ");
scanf("%d", &n);

if(isPalindrome(n))
printf("%d is a Palindrome number\n", n);
else
printf("%d is not a Palindrome number\n", n);

return 0;

## Output:- Enter a number to check -> 121
121 is a Palindrome number
Enter a number to check -> 125621
125621 is not a Palindrome number
```                                 
