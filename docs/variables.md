# Variables

A variable is a stored value that can be changed. In Scorch, there a one key way to create and change variables.

## Assign a Variable
*Variable _ is _*  
Create or change a variable with a given name and value.  
The name must be a word that cannot be any other keyword, like a statement.  
If the name of the variable has already been assigned, the variable value will be changed. 

Creating Multiple Variables:
```
Variable var1 is 2
Variable var2 is var1 - 100
Variable var3 is “words, and a few of them!”

Repeat var2 times
Block
Say var3
Say var1
End block
```
Overwriting Variable:
```
Variable var1 is 2
Say var1 // this outputs 2

Variable var1 is 100000 //overwrite var1
Say var1 // this outputs 100000
```