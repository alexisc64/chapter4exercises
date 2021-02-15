# *chapter4exercise*
##  The following will work on a UNIX machine, but will fail on a PC :
int zip; /* zip code for current address */
.........
zip = 92126;
/*********************************************************************
* the given number is greather than most pc can handle               *
**********************************************************************/
## What must be done to this program to fix it?

#include <stdio.h>
float answer; /* The result of our calculation */
int main()
{
answer = 1/3;
printf("The value of 1/3 is %f\n", answer);
return (0);
}
/**********************************************
* we need to introduce float values, changing *
* 1/3 for 1.0/3.0 in order to make it a float *
***********************************************/
## Why does 2 + 2 = 5928?

[File: two/two.c]
#include <stdio.h>
/* Variable for computation results */
int answer;
int main()
{
 answer = 2 + 2;
 printf("The answer is %d\n");
 return (0);
}
/***********************************************
* because you need to put the variable (answer)*
* because if not, C will give a weird numeric  *
* value to %d                                  *
************************************************/
## Why is an incorrect result printed? 
[File: div/div.c]
#include <stdio.h>
float result; /* Result of the divide */
int main()
{
 result = 7.0 / 22.0;
 printf("The result is %d\n", result);
 return (0);
}
/***********************************************
* with *float* we need to use %f\n instead of  *
* %d\n                                         *
************************************************/
## 

