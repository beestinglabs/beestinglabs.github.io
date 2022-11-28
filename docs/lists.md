# Lists
Lists are just a collection of values, which can be manipulated and changed. For example, this can be useful for storing a collection of notes or numbers.

Create a list by typing a sequence of numbers. For example:  
`1 2 3 4 `  
`C4 B2 Db5`  

The lists we created above are valid lists, and can be used in other statements, for example to play a chord:  
`Play note c4 c5 Eb5 for 1 beat`

Use lists in the same way as you would any other value, like creating a variable with a list as a value:  
`Variable mylist is 0 1 2 3 4 5`

To interact with the values in a list, there are 4 main statements:

*Add value \_value\_ to position \_position\_ of \_list\_*  
*Swap value \_value\_ to position \_position\_ of \_list\_*  
*Remove value from position \_position\_ of \_list\_*  
*Get value from position \_position\_ of \_list\_*  

**value**: the value to add or swap to the list.  
**position**: the position within the list to alter.  
**list**: the list to interact with.  

Important: Lists are a collection of values, and Scorch will treat them as such. They can be used in place of a value, even in statements used to interact with lists! This will become more clear later on.


## Add value to list
*Add value \_value\_ to position \_position\_ of \_list\_*  
Add a value to the list at a given position.

*Add value \_value\_ to end of \_list\_*  
Add a value to the end of the list.

*Add value \_value\_ to start of \_list\_*  
Add a value to the start of the list.

## Remove values from list
*Remove value \_value\_ from \_position\_ of \_list\_*  
Remove a value from a given position in a list

*Remove value \_value\_ from start of \_list\_*  
Remove a value from the start of a list

*Remove value \_value\_ from end of \_list\_*  
Remove a value from the end of a list

## Swap values of list
*Swap value \_value\_ to position \_position\_ of \_list\_*  
Swap a new value for an existing value at a given position in a list. 

*Swap value \_value\_ to end of \_list\_*  
Swap a new value for the last value of a given list.

*Swap value \_value\_ to start of \_list\_*  
Swap a value for the first value of a given list.

## Get values from a list
*Get value from position \_position\_ of \_list\_*  
Get the value at a given position in a list

*Get value from end of \_list\_*  
Get a value at the end of a list

*Get value from start of \_list\_*  
Get the value at the start of a list

### List examples:

create a list and store it, then play then add a value at the end of the list:
```
Variable my_list is 0 1 2 3 4
Say “original list:”
Say my_list
Add value 2 to end of my_list
Say “altered list:”
Say my_list
```
Create a list of notes and velocities and store them, then use a certain value of these lists:
```
Variable my_notes is c4 c5 d2 e3
Variable my_velocities is 0.1 1 0.6
Play(get first value from my_notes) for 1 beat with velocity (get first value from my_velocities)
```
Create some lists and store them, then interact with the lists and use their values:
```
Variable my_notes is c4 c5 c2 c6
Variable my_velocities is 0.2 1 0.3 0.4
Repeat 8 times
Block
    From 0 to 3
    Block
        Play (get value from position count of my_notes) with velocity (get value from position count of my_velocities) for 1 beat
    End block
    Swap value (random note between c4 and c5) to position (random number between 0 and 3) of my_notes
    Swap value (random number) to position (random number between 0 and 3) of my_velocities
End block
```