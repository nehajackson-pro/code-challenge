# code-challenge
#include <stdio.h>

void printChristmasTree(int height) 
{
    int width = 2 * height - 1;
    for (int i = 1; i <= height; i++) 
    {
        for (int j = 1; j <= width; j++) 
        {
            if (j >= height - (i - 1) && j <= height + (i - 1)) 
            {
                printf("*");
            } 
            else 
            {
                printf(" ");
            }
        }
        printf("\n");
    }
    for (int i = 0; i < height - 1; i++) 
    {
        printf(" ");
    }
    printf("*\n");
}

void printSnowman() 
{
    printf("   _===_\n");
    printf("  (.,.)\n");
    printf("  ( : )\n");
    printf("  ( : )\n");
}

int main() 
{
    int treeHeight = 5;
    }

    // Print Christmas Tree
    printChristmasTree(treeHeight);

    // Print a blank line between the tree and the snowman
    printf("\n");

    // Print Snowman
    printSnowman();

    return 0;
}
