## Program 15: Write a program to demonstrate arrays
```c
#include <stdio.h>

int main(){
    int arr[10];
    printf("Enter array elements:\n");
    for(int i=0; i<5; i++){
        printf("Enter %d element: ",i+1);
        scanf("%d",&arr[i]);
    }
    printf("\n\nSquares of array elements:\n");
    for(int i=0; i<5; i++){
        arr[i] = arr[i] * arr[i];
        printf("%d\n",arr[i]);
    }

    return 0;
}
```
### Output: Enter array elements:
```
Enter 1 element: 5
Enter 2 element: 2
Enter 3 element: 8
Enter 4 element: 12
Enter 5 element: 6


Squares of array elements:
25
4
64
144
36
```
