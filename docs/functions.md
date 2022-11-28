# Functions
A function must be created, then called. The process is as follows: 

## Create a function
*Function _ _*  
Create a function. The function needs to have a name, which must be a word, and can take variables after the name. These variables are then able to be used in the function itself, and the values of those variables can be different each time the function is called.

## Call a function 
*Call _ _*  
Call a function with the following variable values. When you call a function that has variables, you need to give it correct values in the same order. Check out examples to see what is meant by that.

```
Function func1
Block
    Say “function 1”
End block

Function func2 var1 var2 var3
Block
    Say var1
    Play note var2 for 1 beat
    Rest for var3 beats
End block

Call func1

Call func2 “function2” C4 2
```