# Program-5-e
## C-Module 5
## EX_NO-05)e)-Arrays
### Date: 19-10-2025
### Name: Anish D
### Register Number:25010086
## AIM:
Write a C Program to displays the lower triangular of a matrix
## ALGORITHM:
1. Start the program.
2. Declare two integer variables to store the number of rows and columns.
3. Read the values of rows and columns from the user using scanf.
4. Declare a two-dimensional array with the given number of rows and columns.
5. Use nested for loops to read elements into the matrix:

    a. Outer loop iterates over rows.

    b. Inner loop iterates over columns.

    c. Read each element using scanf.
6. Print the message "matrix is".
7. Use nested for loops to display the entire matrix:
 
    a. Print each element followed by a space.

    b. Move to a new line after each row.
8. Use nested for loops to display specific elements based on conditions:
 
    a. If the current position satisfies (i==1 && j==1) or (i==2 && j!=3) or (i==3), print the element.

   b. Move to a new line after each row.
9. End the program.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int row,col;
    scanf("%d%d",&row,&col);
    int arr[row][col];
    for(int i=1;i<=row;i++)
    {
        for(int j=1;j<=col;j++)
        scanf("%d",&arr[i][j]);
    }
    printf("matrix is\n");
    for(int i=1;i<=row;i++)
    {
        for(int j=1;j<=col;j++)
        {
            printf("%d ",arr[i][j]);
        }
        printf("\n");
    }
    printf("\n");
    for(int i=1;i<=row;i++)
    {
        for(int j=1;j<=col;j++)
        {
            if((i==1&&j==1)||(i==2&&j!=3)||i==3)
            printf("%d ",arr[i][j]);
        }
        printf("\n");
    }
}
```
## OUTPUT:
<img width="831" height="592" alt="Screenshot 2025-10-20 090503" src="https://github.com/user-attachments/assets/b4f94e25-650f-48e3-b22e-dbc695ac9d81" />

## RESULT:
Thus the program to displays the lower triangular of a matrix has been executed successfully
