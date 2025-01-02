#include <stdio.h>
#include <stdbool.h>

int main()
{
int num;
bool est_premier = 1;
printf("Enter your number:\n");
scanf("%d", &num);

if(num <= 1)
{
    est_premier = 0;
}

else
{
for(int i = 2; i <= num / 2; i++)
{
    if(num % i == 0)
    {
    est_premier = 0;
    break;
    }
}
}

if(est_premier)
    {
        printf("Your number is a prime number!");
    }
    else
    {
        printf("Your number is not a prime number!\n");
    }
}
