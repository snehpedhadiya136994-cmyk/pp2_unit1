#include <stdio.h>
int main() {
    int n, i;
    float sum = 0;
    printf("Enter N: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        sum += arr[i];
    }
    printf("Total: %.0f\n", sum);
    printf("Average: %.2f\n", sum / n);
    return 0;
}
