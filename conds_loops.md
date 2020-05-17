# loops & conditionals
***
### A loop is used for executing a block of statements repeatedly until a given condition returns false.



## macros
In a C program, all lines that start with # are processed by preprocessor which is a special program invoked by the compiler. In a very basic term, preprocessor takes a C program and produces another C program without any #.

```tcc
#include<stdio.h> 
#define tax 100 
int main() 
{ 
    printf("tax is %d", max); 
    return 0; 
} 
```
output: tax is 100

When we use define for a constant, the preprocessor produces a C program where the defined constant is searched and matching tokens are replaced with the given expression. For example in the following program max is defined as 100.

***
## operator ternary (?)
The conditional operator is kind of similar to the if-else statement as it does follow the same algorithm as of if-else statement but the conditional operator takes less space and helps to write the if-else statements in the shortest way possible.


<img src="https://media.geeksforgeeks.org/wp-content/uploads/20190920110229/Conditional-or-Ternary-Operator-__-in-C_C.jpg" width="200">

Syntax: variable = Expression1 ? Expression2 : Expression3

examples: 
```tcc
#include <stdio.h> 
int main() 
{ 
    // variable declaration 
    int n1 = 5, n2 = 10, max; 
  
    // Largest among n1 and n2 
    max = (n1 > n2) ? n1 : n2; 
  
    // Print the largest number 
    printf("Largest number between"
           " %d and %d is %d. ", 
           n1, n2, max); 
    return 0; 
} 
```
Output:
Largest number between 5 and 10 is 10.
***
## if else

Decision Making in C helps to write decision driven statements and execute a particular set of code based on certain conditions.

The if statement alone tells us that if a condition is true it will execute a block of statements and if the condition is false it won’t. But what if we want to do something else if the condition is false. Here comes the C else statement. We can use the else statement with if statement to execute a block of code when the condition is false.

if (condition)
{
    // Executes this block if
    // condition is true
}
else
{
    // Executes this block if
    // condition is false
}

### Example
```tcc
#include <stdio.h> 
int main() 
{ 
    int i = 25; 
  
    if (i > 15) 
        printf("i is greater than 15"); 
    else
        printf("i is smaller than 15"); 
  
    return 0; 
} 
```
output: i is greater than 15

flowchart: 
<img src="https://media.geeksforgeeks.org/wp-content/uploads/20191119183412/C-Cpp-if-else.png" width="200">
***
## for 
This is one of the most frequently used loop in C programming.
Syntax of for loop:

 
 For (initialization; condition test; increment or decrement)
{
       //Statements to be executed repeatedly
} 

###lets see a example

```tcc
#include <stdio.h>
int main()
{
   int i;
   for (i=1; i<=5; i++)
   {
       printf("%d\n", i);
   }
   return 0;
}

```
output:
1,2,3,4,5

#### Nested For Loop

for ( initialization; condition; increment ) {
   for ( initialization; condition; increment ) 
      // statement of inside loop
   }
   // statement of outer loop
}

### Example
```tcc
#include <stdio.h>
int main(){
   for (int i=0; i<2; i++)
   {
	for (int j=0; j<4; j++)
	{
	   printf("%d, %d\n",i ,j);
	}
   }
   return 0;
}
```



flowchart: 
<img src="https://beginnersbook.com/wp-content/uploads/2017/09/for_loop_C.jpg" width="200">
***
## break statement

The break in C is a loop control statement which is used to terminate the loop. As soon as the break statement is encountered from within a loop, the loop iterations stops there and control returns from the loop immediately to the first statement after the loop.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/break.png" width="200">


Basically break statements are used in the situations when we are not sure about the actual number of iterations for the loop or we want to terminate the loop based on some condition.

Syntax:
```tcc
break;
```

break can used in 3 diferents loops
#### 1.Simple loops
```tcc
#include <stdio.h>
int main()}
int i;
for (int i = 0; i < 10; i++) {
  if (i == 4) {
    break;
  }
  printf(" %i\n");
  return 0;
}
```


 #### 2.Nested loops
```tcc
#include <stdio.h> 
  
int main() { 
    // nested for loops with break statement 
    // at inner loop 
    for (int i = 0; i < 5; i++) { 
        for (int j = 1; j <= 10; j++) { 
            if (j > 3) 
                break; 
            else
                printf("*"); 
        } 
        printf("\n"); 
    } 
   
    return 0; 
} 

```

#### 3.Infinite loops
```tcc
#include <stdio.h> 
  
int main() { 
    // loop initialization expression 
    int i = 0; 
   
    // infinite while loop 
    while (1) { 
        printf("%d ", i); 
        i++; 
    } 
   
    return 0; 
} //warning: dont forget to put "break" in this type of loop
```
***
## continue statement
Continue is also a loop control statement just like the break statement. continue statement is opposite to that of break statement, instead of terminating the loop, it forces to execute the next iteration of the loop.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/continue.png" width="200">




```tcc
#include <stdio.h> 
int main() { 
    // loop from 1 to 10  
    for (int i = 1; i <= 10; i++) {  
        // If i is equals to 6,  
        // continue to next iteration  
        // without printing  
        if (i == 6)  
            continue;  
        else
            // otherwise print the value of i  
            printf("%d ", i);  
    }  
    return 0;  
}
```
Output:
1 2 3 4 5 7 8 9 10 

The continue statement can be used with any other loop also like while or do while in a similar way as it is used with for loop above.


***
Reference:
https://www.geeksforgeeks.org/
