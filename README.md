# linearsearch
#include <stdio.h>

int main() {
    int n;
    
    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);
    
    int arr[n]; // Declare an array of size n
    
    printf("Enter the elements of the array:\n");
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]); // Input each element of the array
    }

    int target;

    printf("Enter the element to search: ");
    scanf("%d", &target);

    int i;
    for (i = 0; i < n; i++) {
        if (arr[i] == target) {
            printf("Element %d found at index %d.\n", target, i);
            break; // Exit the loop once the element is found
        }
    }

    if (i == n) {
        printf("Element %d not found in the array.\n", target);
    }

    return 0;
}
