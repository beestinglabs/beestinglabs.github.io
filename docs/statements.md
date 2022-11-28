# Statements
Shorthand - Scorch has some shorthand forms of keywords and statements to enable quicker writing, however this comes at the cost of obfuscation of the code itself. The words or letters in the following which are in italics are not required for Scorch to understand the code.

## Say
Tell Scorch to say something in the console below the text editor.  
Scorch can say numbers, variables, notes, words.

`Say “hello”`  
`Say 1`  
`Say variable1` 

## Play
*Play note _ for _ beat*  
Play will play a given note for a given duration. If no duration is given, it will play that note for 1 beat.

`Play note C4 for 1 beat`  
`Play note 44 for 1 second`  
`Play note Cb5`  

## Repeat
*Repeat _ times*  
Repeats the following block of code a given number of times. The number of times can be a number or a variable defined earlier.

`Repeat 4 times`  
```
Block  
    Say “hello”  
End block
```

`Variable var1 is 30`

```
Repeat var1 times
Block
Say “30 times”
End block
```

## Rest
*Rest for _ beats*  
A rest for a given amount of time. Scorch will not read the next line of code until the time of rest has passed.

```
Play note C4 for 1 beat  
Rest for 1 
```

## Random Number
*Random Number between _ and _*  
A random number between 2 given values.  
If no values are given, this produces a random number between 0 and 1.

`Random number between 2 and 6`  
`Random number`

## Random Note
*Random Note between _ and _*
A random note between 2 given notes.  
If no notes given, produces a random note between minimum and maximum possible

`Random note between c4 and c7`  
`Random note`  

## Set CC
*Set CC _ to _*  
Set a given midi continuous control value to a given value between 0 and 127.

`Set CC 13 to 100`  
`Set CC 2 to random number between 0 and 127`  

## Set midi channel 
*Set midi channel to _*  
Set the midi output channel to given value.

`Set midi channel to 2`
