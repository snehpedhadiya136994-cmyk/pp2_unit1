#include <stdio.h>
int main() {
    char str1[100], str2[100];
    int i, same = 1;
    printf("Enter first string: ");
    scanf("%s", str1);
    printf("Enter second string: ");
    scanf("%s", str2);
    for(i = 0; str1[i] != '\0' && str2[i] != '\0'; i++) {
        if(str1[i] != str2[i]) {
            same = 0;
            break;
        }
    }
    if(str1[i] != str2[i]) same = 0;
    printf("Same: %s\n", same ? "Yes" : "No");
    return 0;
}
