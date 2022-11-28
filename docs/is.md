## Is
*Is _ less than/more than/equal to _ ?*  
Is allows the comparison of two values, and if found to be correct, Scorch will read the block which follows, otherwise it will skip the block. The comparisons can be written out or can be the symbolic equivalents:  
<, >, =, !=.

```
Is 2 more than 1?
block 
    Say “yes”
End block
```
```
Is random number equal to 1
Block
    Say “ yes”
End block
```
```
Variable var1 is 200
Is var1 < 2
Block
    Say “no, it is 200”
End block
```


## Or is?
*Or is _ less than/more than/equal to _ ?*  

When an is statement is false, and does not execute the code block below it, Scorch will move to the next 
statement. Having `Or is _ less than/more than/equal to _ ?` below an `is` statement will only be read by 
Scorch if the is before it is false. You can chain as many of these together as you like, and the first to 
come true will be the only one that Scorch executes.

## Otherwise
*Otherwise*  

Otherwise can be used after an is statement or an is statement followed by or is statements. If all the is/or 
is  statements are false, Scorch will always execute the block below otherwise. If one of the is/or is 
statements before is correct, the otherwise will be ignored by Scorch.

```
Is 3 less than 2?
Block
    Say “no it’s not!”
End block
Or is 4 more than 5?
Block
    Say “nope!”
End block
Otherwise
Block
Say ”last 2 were false. So this will be read!”
End block
```