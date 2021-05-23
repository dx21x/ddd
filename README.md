#include <stdio.h>
#include <string.h>
#include <cs50.h>
void count_vowels(char str[])
            //homework8
{
    int vowels = 0;
    int i;
    char ch;
    for (i = 0; str[i] != '\0'; i++) 
    {
        ch = str[i];
        if (ch == 'a' || ch == 'e'||
            ch == 'i' || ch == 'o'||
            ch == 'u' || ch == 'A'||
            ch == 'E' || ch == 'I'||
            ch == 'O' || ch == 'U')
            vowels++;
        else if (ch == ' ')
        continue;    }
    printf("\nVowels:%d\n", vowels);
}
int main()
{
    string str =get_string("Please write a sentence:");
    count_vowels(str);
    return 0;
}
