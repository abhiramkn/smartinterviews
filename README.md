#include <stdio.h>

int main() {
    char s[101];
    scanf("%s", s);

    int i = 0;

    while (s[i] != '\0') {
        char ch = s[i];
        int count = 0;

        while (s[i] == ch) {
            count++;
            i++;
        }

        printf("%c%d", ch, count);
    }

    return 0;
}
