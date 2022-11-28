# From
*From _ to _ in steps of _*  
From to repeats the following block of code from first value to second value, increasing in steps of third 
value, and the current number is accessible in the block of code using the variable “count”. If no steps are 
given, the step size is 1.

```
From 0 to 100 in steps of 1
Block
    Say count
    Rest for 0.1 seconds
End block
```

```
From 100 to 105 in  steps of 0.25
Block
    Say count
    Rest for 0.1 seconds
End block
```

```
From 0 to 10
Block
    Say “from count”
    Say count
    Repeat count times
    Block
        Say “repeat”
        Play note c4 for 0.1 seconds
    End block
End block
```