## Write a program to perform Selection sort.
```c
#include <stdio.h>

void selSort(int *arr,int len){
    int min = 0,temp;
    for(int i=0;i<len;i++){
        min = i;
        //find min
        for(int j=i;j<len;j++){
            if(arr[j]<arr[min])min=j;
        }
        //swap
        temp = arr[i];
        arr[i] = arr[min];
        arr[min] = temp;
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
    selSort(arr, len);

    printf("\nSorted array is :\n");
    for(int i=0;i<len;i++){
        printf("%d\t",arr[i]);
    }
    printf("\n");
}
```
### Output:
```
Enter size of array
10
Enter elements
Enter element at index 0 -> 55
Enter element at index 1 -> 88
Enter element at index 2 -> 22
Enter element at index 3 -> 77
Enter element at index 4 -> 0
Enter element at index 5 -> 99
Enter element at index 6 -> 33
Enter element at index 7 -> 44
Enter element at index 8 -> 66
Enter element at index 9 -> 11

Unsorted array is :
55	88	22	77	0	99	33	44	66	11	

Sorted array is :
0	11	22	33	44	55	66	77	88	99
```
