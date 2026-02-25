#include <stdio.h>
int main() {
    char str[100];
    int spaces = 0, vowels = 0, i;
    printf("Enter a string: ");
    fgets(str, 100, stdin);
    for(i = 0; str[i] != '\0' && str[i] != '\n'; i++) {
        if(str[i] == ' ') spaces++;
        else if(str[i] == 'a' || str[i] == 'e' || str[i] == 'i' || str[i] == 'o' || str[i] == 'u' ||
                str[i] == 'A' || str[i] == 'E' || str[i] == 'I' || str[i] == 'O' || str[i] == 'U') vowels++;
    }
    printf("Spaces: %d, Vowels: %d\n", spaces, vowels);
    return 0;
}
