## Write a program to perform insertion sort.
```c
#include <stdio.h>

void insertSort(int *arr,int len){
    int j,curr;
    for(int i=1;i<len;i++){
        curr=arr[i];
        for(j=i-1;j>=0 && arr[j] > curr;j--) arr[j+1] = arr[j];
        arr[j+1] = curr;
    }
}

int main(){
    int len;
    printf("Enter size of array\n");
    scanf("%d",&len);
    int arr[len];
    printf("Enter elements \n");
    for(int i=0;i<len;i++){
        printf("Enter element at index %d -> ",i);
        scanf("%d",&arr[i]);
    }
    printf("\nUnsorted array is :\n");
    for(int i=0;i<len;i++){
        printf("%d\t",arr[i]);
    }
    printf("\n");
    insertSort(arr, len);

    printf("\nSorted array is :\n");
    for(int i=0;i<len;i++){
        printf("%d\t",arr[i]);
    }

```
### Output:
```
Enter size of array
10
Enter elements
Enter element at index 0 -> 88
Enter element at index 1 -> 33
Enter element at index 2 -> 44
Enter element at index 3 -> 22
Enter element at index 4 -> 66
Enter element at index 5 -> 99
Enter element at index 6 -> 0
Enter element at index 7 -> 77
Enter element at index 8 -> 55
Enter element at index 9 -> 11

Unsorted array is :
88	33	44	22	66	99	0	77	55	11	

Sorted array is :
0	11	22	33	44	55	66	77	88	99
```
