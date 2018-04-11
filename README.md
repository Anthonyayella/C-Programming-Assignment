# Assignment
This is a simple repository you will use to finish the assignments contained in this 
README.md document.

## Instruction
You are to create separate files for each question and upload those to your repositories. 
After which you will create a pull request when you are done with your assignment. 
For more information on how to use GitHub, check out this link on 
[GitHub Flow](https://guides.github.com/introduction/flow/,"GitHub Flow").

In essence, you will fork this repository to create your own master copy of it. Do the 
assignment and create a pull request with your different files. which I will observe and
score. 

## Question One
Fix the Bug in the following code so that it runs correctly
```objectivec
                    /* a program with problems... */
                    #include <stdio.h>
                    int x= 1:
                    main()
                    {
                        if( x = 1);
                            printf(" x equals 1" );
                        otherwise
                            printf(" x does not equal 1");
                        return 0;
                    }
```
ANSWER

#include
<stdio.h> 
int x = 1; 
main(){ 
    if(x==1) 
    printf ("x equals 1"); 
    else     printf ("x isn'tequal to  1");    
    return 0; 
    } 





## Question Two
Write a header for a function named ```do_it()``` that takes three type char 
arguments and returns a type float to the calling program.

#ifndef Do_it_h
#define Do_it_h

float do_it(char a,char b,char c);
#endif//Do_it_h






Write a header for a function named ```print_a_number()``` that takes a single
type int argument and doesn't return anything to the calling program.

#ifndef PRINT_A_NUMBER_H
#define PRINT_A_NUMBER_H
void print_a_number(int x);
#endif//PRINT_A_NUMBER_H






What's wrong with the following program ?
```objectivec
                    #include <stdio.h>
                    void print_msg( void );
                    main(){
                        print_msg("This is a message to print");
                        return 0;
                    }
                    void print_msq( void )
                    {
                        puts("This is a message to print");
                        return 0;
                    }
```

THE MAIN FUNCTION CALLS print_msg()function WITH A STRING ARGUMENT EVEN IF THEprint_msg() isnt supposed to take any arguments



## Question Three
Write a declaration for an array that will hold 50 type long values

longvalues[50];


Show a statement that assigns the value of 123.456 to the 50th element in the array
from the above question

longvalues[49] = 123456;

What is the values of x when the following statement in complete ?
```objectivec
    for (x = 0; x < 100; x++)
``` 

x=100



What is the value of ctr when the following statement is compelte ?
```objectivec 
   for(ctr = 2; ctr < 10; ctr += 3)
```

ctr=11

Write a while statement to count from 1 to 100 by 3s



What is wrong with the following code fragment (MAXVALUES is not the problem !)
```objectivec
    for (counter = 1; counter < MAXVALUES; counter++ );
    printf("\nCounter = %d", counter);
```
THE SEMICOLON CAUSES THE FOR LOOP TO EXECUTE ONLY ONCE
## Question Four
Write a function named ```addarrays()``` that accepts two arrays that are the same size. 
The function should add each element in the arrays together and place the values in a
third array.




void
addarrays(int array1[], int array2[], int destination_array[], int SIZE){ 
    for(int i=0;i<SIZE;i++){ 
    destination_array[i] = array1[i] +
array2[i]; 
} 

} 





Modify the function you created to return a pointer to the array containing the totals.
Place this function in a program that also displays the values in all three array






#include
<stdio.h> 
int*addarrays(int array1[], int array2[], int SIZE); 
 main(){ 
   int array1[] = {1,2,6,8,7}; 
   int array2[] = {100,120,600,180,700}; 
 int *array3 = addarrays(array1, array2, 5);
    for(int i=0;i<5;i++) {         printf("%d \n", array3[i]);     } 

} 
int
*addarrays(int array1[], int array2[], int length){     int *destination_array = malloc(length *
sizeof(int));     for(int
i=0;i<length;i++){ 
        destination_array[i] = array1[i] +
array2[i]; 
    } 
    return destination_array; } 

 

