#include <stdio.h>
int main() {
    char str[100];
    int i, j = 0, len = 0, isPal = 1;
    printf("Enter a string: ");
    scanf("%s", str);
    while(str[len] != '\0') len++;
    for(i = 0, j = len - 1; i < j; i++, j--) {
        if(str[i] != str[j]) {
            isPal = 0;
            break;
        }
    }
    printf("Palindrome: %s\n", isPal ? "Yes" : "No");
    return 0;
}
