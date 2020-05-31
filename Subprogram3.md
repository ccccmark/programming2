<h1> Chapter 3</h1>

***
<h3>Subprograms are the fundamental building block of programs and are therefore among the most important concepts in programing languages design.</h3>

***

 ## Characteristics of Subprogram

A Subprogram is a program inside any larger program that can be reused any number of times.

Characteristics of a Subprogram:
<img src="https://image.slidesharecdn.com/namesbinding-141110164824-conversion-gate01/95/subprogram-32-638.jpg?cb=1415638216" width="400">


Subprograms include the following characteristics:

<h3>-Each subprogram has a single entry point</h3>
<h3>-There is only one subprogram execution at any given time</h3>

<h3>-Control always returns to the caller when the subprogram execution terminates.</h3>


(1) A Subprogram is implemented using the Call & Return instructions in Assembly Language.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/Untitled-drawing-5-2.jpg" width="700">

- The Call Instruction is present in the Main Program and the Return(Ret) Instruction is present in the subprogram itself.

- The Main advantage of Subprogram is that it avoids repetition of Code and allows us to reuse the same code again and again.

***
Two fundamental abstractions
- process abstraction 
- data abstraction.

```tcc
int swap(int& a, int& b) {
int c = a;
a = b;
b = c;
}
```
Charateristics of process abstractions
-Memory space efficiency.
-I Less development and maintenance time,
-I Increase readability, and etc.






***

<h1>Parameters</h1>
subprogram are used to perform some specified task. they can gain access to the data by two ways

1.through direct access to non local variables
2.through parameters passing



<h2>types of parameters</h2>

<h3>parameter profile</h3>
The parameter profile of a subprogram is the container of the number, order, and types of its formal parameters. While a subprogram protocol is subprogram’s parameter profile as well as its return type if it’s a function.

<h3>Formal parameter</h3>
Formal parameters are parameters in the subprogram header, sometimes thought as dummy variables because they are not variables in the usual sense, mostly because they are bound to storage only when the subprogram is called while binding is often through some other program variables.

<h3>Keyboard parameter</h3>
when parameters lists are long there may be mistakes in the order of parameter in the list

<h3>Positional parameter</h3>
in nearly all languages the blinding of the actual parameter to the formal parameter is done by simple position. the first actual parameter is bound to the first formal parameter and so forth

<h3>parameter-passing method of Python</h3>

The parameter-passing method of Python  is called passing-by-assignment. Because all data values are objects, every variable is a reference to an object. So, the actual parameter value is assigned to the formal parameter

***

<h1>recursive processes</h1>
Recursion means subprogram call itself.recursive subprogram calls. is one of the most sequence-control structure in programing.

<img src="https://cdn.programiz.com/sites/tutorial2program/files/how-recursion-works-c_0.jpg" width="200">

<h3>Direct</h3>
When in the body of a method there is a call to the same method, we say that the method is directly recursive. That means Direct recursion occurs when a method invokes itself.

-direct recursion makes overhead.

-The direct recursion called by the same function

-In direct function, when function called next time, value of local variable will stored

-Direct function engaged memory location	
```tcc
int num()
{
	...
	...
	int num();

}
```



<h3>Indirect</h3>
In indirect recursion more than one function are by the other function and number of times.

-The indirect recursion does not make any overhead as direct recursion

-While the indirect function called by the other function

-but in indirect recursion, value will automatically lost when any other function is called local variable

-while local variable of indirect function not engaged it
```tcc
int num()
{
	...
	...
	int sum();

}
int sum()
{
	...
	...
	int num();

}
```


***
References
https://www.geeksforgeeks.org/subprogram-and-its-characteristics/

