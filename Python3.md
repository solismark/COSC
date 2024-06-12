# Day 1
## Student Handbook
https://git.cybbh.space/programming/python/public


## SSH Command 
This is the command is to login to our Linux as student : `ssh student@10.0.0.0 -X` 

## FOR Loop
This will print each fruit in the list
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
```
## Information on stacks6 filetype indent on


windows_opstation_em90

192.168.65.10
10.50.21.242

lunix_opstation_em90 (password = password)

192.168.65.20
10.50.37.42

`ssh student@10.50.37.42 -X` and `terminator` 

## Console to VTA Instance
Project > Compute > Instances > Actions > Console to view GUI for each instance

## Creating Environment
vim $HOME/.vimrc

  ```
  1 syntax enable
  2 set tabstop=4
  3 set shiftwidth=4
  4 set expandtab
  5 set number
  6 filetype indent on
  7 set autoindent
```
turn numbers off on vim `set number` and `unset number`

nano $HOME/.nanorc

set tabsize 4
set tabstospaces
set linenumbers

## Basics
```
a = 1addition
	

+

subtraction
	

-

multiplication
	

*

division
	

/

integer division
	

//

modulus
	

%

exponent
	

**
print(type(a))
```

Caling for a script `python3 test.py` command
type()

float = 1.2

integer = 1

strings = "string" or 'string' can use single or double quotes

boolean = (True) or (False) 

    bool - boolean (True or False)

    int - integers

    float - floating point decimal

    str - string

    tuple - immutable sequence of items (not necessarily of the same type)

    list - mutable sequence of items (not necessarily of the same type)

 
 `git clone https://git.cybbh.space/programming/python/public.git`

addition
	

+

subtraction
	

-

multiplication
	

*

division
	

/

integer division
	

//

modulus
	

%

exponent
	

**

```
'hello' + string(1)
`hello1`

float(1)
1.0

int('1')
1

bool(0)
False

bool(1)
True

bool('0')
True

bool('')
False

'hello' * 5
'hellohellohellohellohello'

a = 'hello'
print( a + 'world')
helloworld

'hello /'world'
"hello 'world"

```

## Mutability

```
num = 0
a = 1
b = 2
num = a + b
num = 3
```
Tuples and Strings are immutable meaning they cannot change like above

a = 'string'

b = (tuple) 

c = [list]

Indexing to call individual elements out of strings 'Hello'[1] would be e
```
>>> a = 'Hello World'
>>> b = list(a)
>>> c = tuple(a)
>>> c
('H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd')
>>> a
'Hello World'
>>> b
['H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd']
```
Can use indexing to change something within the list
```
>>> b[0] = 'J'
>>> b
['J', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd']
```

## Split
split is a function and calling to it makes it a method function

first example is using the space as the delimeter
```
>>> 'hello world'.split()
['hello', 'world']
````
whatever you want to .split() you input the delimeter such as split(':') or split('-') and on that delimeter the function will split

```
'user:passwd'.split(':')
'user', 'passwd'
```
## Join
```
>>> b
['J', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd']
>>> ''.join(b)
'Jello World'

>>> b
['J', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd']
>>> 'O'.join(b)
'JOeOlOlOoO OWOoOrOlOd'
>>> 

```

## Format
Can pass values into curly brackets as placements and can be saved as a different variable
```
>>> hobbit = ['Frodo', 'Sam', 'Bilbo']
>>> hobbit
['Frodo', 'Sam', 'Bilbo']
>>> hobbit[1]
'Sam'
>>> hobbit[-1]
'Bilbo'


>>> print('{} {} {}'.format(hobbit[0], hobbit[1], hobbit[2]))
Frodo Sam Bilbo
>>> print('{} - {} - {}'.format(hobbit[0], hobbit[1], hobbit[2]))
Frodo - Sam - Bilbo
>>> print('{} , {} , {}'.format(hobbit[0], hobbit[1], hobbit[2]))
Frodo , Sam , Bilbo



```

## Email Splitter Activity

```
  1 email = input("Enter a email address:  ")
  2 result = input("Want to split email? Yes or No  ")
  3 true = "Yes"
  4 false = "No"
  5 if result == true:
  6     part1 = email.split('@')
  7     part2 = '.'.join(part1)
  8     part3 = part2.split('.')
  9     print(part1 and part2 and part3)
 10 else:
 11     print("Wrong option!!!!")
```





# Day 2
## Flow Control, Input, and CodeWars

# .append()
In order to output a list you need to have a empty list.

```
fellowship = []
fellowship.append('Froto')
fellowship
['Froto']

fellowship.append('Sam')
fellowship.append('Mary')
fellowship.append('Pip')
['Frodo', 'Sam', 'Mary', 'Pip']
```
.append() is used to add something to the list above "fellowship"
we are able to add things to the list with a .append()

# .input()

input is used to take user input and store it in a variable. you can also add a prompt for users to see
if you want to use the variable you need to set the variable then add input after the =
```
input()
something
'something'


input('Please type something:\n')
Please type something:
1
'1'


var = input('Type something:\n')
Type something:
1
'1'
print(type(var))
<class 'str'>
```


# Type casting using input()

```
var = int(input('Type something:\n'))
Type something:
1
1

var + 1
2

```
type casting allows you to set the input to a different type and perform different functions such as the example above with var + 1 because we typecasted it with int(input())


# Flow control
water can flow or crash just like code

# FOR Loop
from above the fellowship list is being evaluated with hobbit. for each hobbit (listing item) within fellowship it will print each object in the list and then add the 'is in the fellowship' string 

will allow you to walk through a list and perform some type of function

```
fellowship
for hobbit in fellowship:
	print(hobbit + 'is in the fellowship')


>>> for hobbit in fellowship:
...     print(hobbit + 'is in the fellowship')
... 
someis in the fellowship
moreis in the fellowship
itemsis in the fellowship
bcis in the fellowship

```

# IF ELIF ELSE Loops

```
if <condition>:
	<code block>
elif <condition>:
	<code block>
elif <condition>:
	<code block>
else:
```
now we can work off our for loop from the above fellowship example
using our hobbit to work through our list we can perform a if statement that says when hobbit is equal to Sam it will perform the print function

```
fellowship = ['Frodo', 'Sam', 'Mary', 'Pip']
for hobbit in fellowship:
	if hobbit == 'Sam':
		print(hobbit + 'is wise')

Sam is wise

```


adding to our if elif else loops 
with the following code it will perform both outputs because it is inside a for loop using hobbit to go through the list regardless if Sam or Pip is found and the print takes place

```
fellowship = ['Frodo', 'Sam', 'Mary', 'Pip']
for hobbit in fellowship:
	if hobbit == 'Sam':
		print(hobbit + 'is wise')
	elif hobbit == 'Pip'
		print(hobbit + 'is a Took')
Sam is wise
Pip is a Took

```

now using else it will run through each time and output in the following order

```
fellowship = ['Frodo', 'Sam', 'Mary', 'Pip']
for hobbit in fellowship:
	if hobbit == 'Sam':
		print(hobbit + 'is wise')
	elif hobbit == 'Pip':
		print(hobbit + 'is a Took')
	else:
		print(hobbit + 'is a hobbitses')
Frodo is a hobbitses
Sam is wise
Mary is a hobbitses
Pip is a Took

```



# WHILE Loops

while will perform an action until the desired response is provided to exit

```
while True:
	print('To infinity and beyond')
To infinity and beyond
To infinity and beyond
To infinity and beyond
To infinity and beyond
To infinity and beyond
To infinity and beyond
```
with this example since True will always be true then the print function will continue to print

```
while num <=5:
	print(num)
	num = num + 1 (or num +=1)

0
1
2
3
4
5


>>>num
6
```

this example will take num and see if its less than or greater than or equal to 5 then it will print the current number and then add 1 so it will continue until the num value is <= 5 therefore nothing happens


# Pass, Break, Coninue

pass will pass to the next line

continue will exit from its location and went back to the loop its in

break will break the code where ever it is located 

```
  1 while True:
  2     user = input('Type pass, break, or continue:\n')
  3     if user == 'pass':
  4             pass
  5             print('This is pass...')
  6 
  7     elif user == 'break':
  8             break
  9             print('This is break...')
 10 
 11     elif user == 'continue':
 12             continue
 13             print('This is continue...')
 14     else:
 15             print('Please choose a valid option:\n')



Type pass, break, or continue:
continue

Type pass, break, or continue:
continue

Type pass, break, or continue:
pass
This is pass...

Type pass, break, or continue:
break
.....
```

# Fizzbuzz activity

```
  1 #!/usr/bin/env python3
  2 num = int(input('Enter a number:\n')
  3 if num % 3 == 0:
  4     print(num + ' is fizzbuzz')
  5 elif num % 3 = 0:
  6     print(num + ' is fizz')
  7 elif num % 5 = 0:
  8     print(num + ' is buzz')
  9 else:
 10     print('The number you entered cannot be divided by 3, 5, or both')

```

