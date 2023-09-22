# Number_Guessing_game_in_c
number guessing game in c
//Number Gussesing Game
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main()
{
    int number, gusses, nggusses = 1;
    srand(time(0));
    number = rand() % 100 + 1;
    // printf("Random number is %d\n", number);
    do
    {
        printf("Enter the number only 1 to 100\n");
        scanf("%d", &gusses);
        if (gusses > number)
        {
            printf("Enter lowest value\n");
        }
        else if(gusses<number)
        {
            printf("Enter highest value\n");
        }
        else{
            printf("You are attempt the %d\n",nggusses);
        }
        nggusses++;
    } while (gusses != number);
    return 0;
}
