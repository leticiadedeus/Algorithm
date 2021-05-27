# My annotations of algorithm
##### || This file is being written with some references to Python codes ||

## Computer components 

- CPU
- Memorie
- In/Out (entrance/exit)

## Algorithm

- A couple of instructions (finite)

## Languages

The computer can't understand the human language, so we could create the algorithm in binarie commands (the computer idiom), but it's more simple than this: we can learn programming languages, that can be transleted by the machine and then it can understand the commands (program)

## Data Representation

### | Intern representation

It can be made in bit, byte(8bits) or 'word'(16bits), that will be ready like **binarie code**

     binarie code = 1/yes 0/no          
     ...32, 16, 8, 4, 2
     if: 101
     then: 10
     reading from right to left

### | Primitive types

- Int:

     positive or negative numbers

- Float:

     decimal numbers

- String

     every character, being it number, letter, symbol or even the space (' ')

- Boolean

     - 1 or 0
     - True or False
     - On or Off
     - Opened or Closed

### | Constants and variables

- Constant: do not change while the code is running
- Variable: can suffer changes

### | Data manipulation

- Identification

     At first, we will need to take the data in a folder(identifier), that will be used to find and reference it later. It's important to give the folder a title that make us know what's saved in it.
     
     We also have some rules to follow: not using special characters, not even space (EXCEPITION: underline = '_')

     Ex =

          name = str(input())
          print(name)

     exit:

          Leticia de Deus
          
- Definition

     We need to define/declare the type of the content that will enter in the folder (identifier). 

     It can be converted, if you need. But it's important to know that each type has their own use. So if you try to make math with a string, it will output a ERROR.

- Assignment

     This moment is when the folder receives their value, no matter the type. It can be done for the own code. Ex:

          name = Leticia de Deus
          print(name)

     exit:

          Leticia de Deus

     Also, the assignment can be asked for the user. EX:

          name = str(input('Insert the name: '))
          print(name)

     exit:

          Insert the name: Pedro Henrique
          Pedro Henrique

When the folder receives a data, it just can keep that one data. If you insert another value, the last one will be forgotten.

## Expressions

### | Arithmetic expressions

Are that expressions that do a operation with numeric values (int and float). The fundamentaal arithmetic operations are: +, -, *, /, **, // and %.

### | Priority
When the code is running and there's a math operation, the processor will proritize the operators in a certain order, that is: 
          ();
          **; 
          *, /, //, %;
          +, -
So, when you're writing your code, make sure the expresssion is correctly written, and always check if all the parentheses are closed. PS: all the expression has to be in one unic line.

### | Tips to a better code:

* Math has exceptions sometimes, it have to be avoid.
* Always look for a simple way to do the expression (and all the functions too)

## Logic expressions

The only answers can be yes or not.

### | Operators

==, >, <, >=, <=, !=;

and, or, xor*, not**

*It's only true if JUST ONE of them is true

**Reverses the result (logic value)

## Exit commands 

When we're talking about the 'exit' in de code, it's a reference to what we show to the user, writing it on the screen.

          print('Hello World')

exit:

          Hello World

|

          message = 'Hello World'
          print(message)

exit: 

          Hellow World

|

The qm (quotation marks [' ', " "]) tell the print function if it will shows the user a folder(identifier) or a message (that's written with qm).

Also, we can use logic expressions to print TRUE or FALSE:

          print(9 > 10)

exit:

          TRUE

## Entrance commands

Most of the codes are made to have a high contact with the user, getting data of them. So we need to know how to receive these data. 

It's important to know that we can warn the user the type of data they can give to the algorithm, for this we use a message with the command of entrance.

          name = str(input('Insert your name: '))
          print(f'Welcome, {name}!)

exit:

          Insert your name: Leticia de Deus <ENTER>
          Welcome, Leticia de Deus!


## Conditions  

Logicly, the code starts running the commands from the first to the last line non-stopping, but, sometimes, we want it to just run a line IF we have a specific situation.

### | if and else

          if (logic expression):
               (command)

The expression have to returns a 'False or True' answer.

          if UserAge >= 18:
               print('The user is older/adult')
          else: 
               print('The user is minor')
          print('End of the algorithm')

'The user is older/adult' will only be printed if the age of the user is higher than or equal 18 years old.

'The user is minor' will only be printed if the age of the 'user is lower than 18 years old.

'End of the algorithm' will be printed anyways, because is out of the structure.

### | elif

          if UserAge >= 18:
               print('The user is adult')
          elif UserAge >= 14:
               print('The user is a teenager')
          else:
               print('The user is a child')

'The user is adult' will only be printed if the age of the user is higher than or equal 18 years old.

'The user is a teenager' will only be printed if the age of the user is higher or equal 14, but we already exclude that users who has 18yo or more.

'The user is a child' will only be printed if the age of the user lower than 14, but see we didn't have to write this logic expression, because we already exclude that users who has 14yo or more.

## Loops

Repeat a command till the code got the objective of that loop. For checking if this objective is achieved, we use a logic expression ('controll expression'). 

### | while (logic expression):

The logic expression will be in the loop command, so everytime before it starts to run the loop,  it will check the expression's value.

          while name != 'end':
               print('The name inserted: ', name)

### | 'do - while':

The logic expression will be on the end of the loop command, so it will me done at least one time without checking the expression's value.

          do:
               name = str(input())
               print(name)
          while:
               name != 'end'

### | 'do - for':

Not logic expression, the control expression is a counter, that will be declared in the beggin of the command. <b>It means we need to know how many times the loop has to run.<b>

          for c in range (0, 3):
               name = str(input('Insert the name: '))

| So the code will receive 3 names only.

## 