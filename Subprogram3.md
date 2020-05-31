<h1> Chapter 3<h1>

***
subprograms are the fundamental building block of programs and are therefore among the most important concepts in programing languages design

 ## Characteristics of Subprogram

A Subprogram is a program inside any larger program that can be reused any number of times.

Characteristics of a Subprogram:


Subprograms include the following characteristics:

<h3>-Each subprogram has a single entry point</h3>
<h3>-There is only one subprogram execution at any given time</h3>

<h3>-Control always returns to the caller when the subprogram execution terminates.</h3>


(1) A Subprogram is implemented using the Call & Return instructions in Assembly Language.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/Untitled-drawing-5-2.jpg" width="700">

(2) The Call Instruction is present in the Main Program and the Return(Ret) Instruction is present in the subprogram itself.

(5) The Main advantage of Subprogram is that it avoids repetition of Code and allows us to reuse the same code again and again.

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

<h3>parameter profile</h3>
The parameter profile of a subprogram is the container of the number, order, and types of its formal parameters. While a subprogram protocol is subprogram’s parameter profile as well as its return type if it’s a function.

<h3>Formal parameter</h3>
Formal parameters are parameters in the subprogram header, sometimes thought as dummy variables because they are not variables in the usual sense, mostly because they are bound to storage only when the subprogram is called while binding is often through some other program variables.


<h3>parameter-passing method of Python<<7h3>
The parameter-passing method of Python  is called passing-by-assignment. Because all data values are objects, every variable is a reference to an object. So, the actual parameter value is assigned to the formal parameter

***

<h1>recursion</h1>

<img src="https://cdn.programiz.com/sites/tutorial2program/files/how-recursion-works-c_0.jpg" width="200">




