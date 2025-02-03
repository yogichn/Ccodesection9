#include <stdio.h>
int sumarrary(int *arr, int size){
    int sum=0;
    for(int i=0; i<size; i++){
        sum += *(arr+i);
    }
    return sum;
}
int main(){
    int n;
    printf("Enter the value of n: \n");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements: ", n);
    for(int i=0;i<n;i++){
        scanf("%d", arr+i);
    }
    int sum = sumarrary(arr,n);
    printf("The sum of the array is: %d\n", sum);
    return 0;
}
