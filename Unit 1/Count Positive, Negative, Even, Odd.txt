#include <stdio.h>
int main() {
    int n, i, pos = 0, neg = 0, even = 0, odd = 0;
    printf("Enter N: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        if(arr[i] > 0) pos++;
        else if(arr[i] < 0) neg++;
        if(arr[i] % 2 == 0) even++;
        else odd++;
    }
    printf("Positive: %d, Negative: %d, Even: %d, Odd: %d\n", pos, neg, even, odd);
    return 0;
}
