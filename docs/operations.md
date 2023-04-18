# Operations

## -
*Subtraction*  
Subtract value on right from value on left.  
`10 - 1`

## + 
*Addition*  
Sum values together.  
`1 + 1`

## *
*Multiplication*  
Multiply values together.  
`100 * 10`

## /
*Division*  
Divide value on left by value on right.
`100 / 10`

## ( )
*Brackets*  
Place an operation in brackets to be completed first.  

These can be used together. The order of operations is as follows: Brackets, Division and Multiplication, Addition and Subtraction, or BDMS for short.

**Example:**  
`100 * -2 - 15 + (20 + 2) / 2`

*Brackets:* `100 * -2 + 15 + 22 / 2`

*Division and Multiplication:* `-200 + 15 + 11`

*Addition and Subtraction:* `-174`

*Answer:* `-174`


# Code in Context

```
variable note1 is d4
variable note2 is e5
variable note3 is g5
variable length1 is 1/6
variable length2 is 1/4
variable length3 is 8
variable length4 is 4

repeat length3 times
block
    play note c4 for length1 + length2 / length3 beats
    rest for length2 beats
    play note note2 for length1 beats
    rest for length2 beats
end block

repeat length4 times
block
    play note note2 for length1 / 3 beats
    rest length2 + length1 / 2 beats
    play note note3 for length1 beats
    play note f5 for length1 beats
    rest length2 beats
end block
```