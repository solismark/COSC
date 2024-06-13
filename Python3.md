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

## Splitting a email address

```

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

## .append()
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

## .input()

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


## Type casting using input()

```
var = int(input('Type something:\n'))
Type something:
1
1

var + 1
2

```
type casting allows you to set the input to a different type and perform different functions such as the example above with var + 1 because we typecasted it with int(input())


## Flow control
water can flow or crash just like code

## FOR Loop
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

## IF ELIF ELSE Loops

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



## WHILE Loops

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


## Pass, Break, Coninue

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

## Fizzbuzz activity

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

## Are you playing banjo? CodeWar

```
def are_you_playing_banjo(name):
    if name[0] == 'r' or name[0] == 'R':
        print(name + ' plays banjo')
    else:
        print(name + ' does not play banjo')
    return name


def are_you_playing_banjo(name):
    if name[0] == 'r' or name[0] == 'R':
        return name + ' plays banjo'
    else:
        return name + ' does not play banjo'
```

## School paperwork Codewar

```
def paperwork(n, m):
    if m<0 or n<0:
        return 0
    else:
        return n*m
```

## Rock paper scissors Codewars

```
def rps(p1, p2):
    if p1 == 'rock' and p2 == 'scissors':
        return 'Player 1 won!'
    elif p1 == 'rock' and p2 == 'paper':
        return 'Player 2 won!'
    elif p1 == 'scissors' and p2 == 'rock':
        return 'Player 2 won!'
    elif p1 == 'scissors' and p2 == 'paper':
        return 'Player 1 won!'
    elif p1 == 'paper' and p2 == 'rock':
        return 'Player 1 won!'
    elif p1 == 'paper' and p2 == 'scissors':
        return 'Player 2 won!'
    elif p1 == p2:
        return 'Draw!'
```

## Guest Boss  Codewars

```
def greet(name, owner):
    if name == owner:
        return 'Hello boss'
    else:
        return 'Hello guest'
```


# Day 3

## Review
int(input) will automatically typecast to a int to perform interger functions

```
lst = []
list.append('Wednesday')
lst
[Wednesday]

type(lst)
```

tuples are () and list are []

```
function

def name(argument1, argument 2)
```

For loops
	for x in list:
 
while loops
	while this is true continue to do this

if branching
elif
else does not need a condition it will perform if none of the if and elif perform


## Ord() and Chr()

Ord() allows you to get ordinal ACSII position of a letter

```
>>> ord('a')
97
>>> ord('z')
122
>>> ord('A')
65

```

same can be done but doing the opposite of Chr()

```
>>> chr(122)
'z'
>>> chr(123)
'{'
>>> chr(121)
'y'
>>> chr(120)
'x'

```

## Range()

will give you the start and end of whatever number that was placed 
```
>>> range(10)
range(0, 10)
```
## List(Range())

will allow you to list the numbers between the two numbers within the range ()

## range(START, STOP (and go back 1), STEP)
is the default operation

```
>>> list(range(0,10,2))
[0, 2, 4, 6, 8]


```

```
>>> for num in range(2,11,2):
...     print(num)
... 
2
4
6
8
10

```
the above example is showing how we are able to utilize the range() and for to iterate though the ranges (START, STOP, STEP) function outputting 
2
4
6
8
10

## Len() or length

len() can be used to help us with indexing number position


```
>>> hobbits = ['frodo', 'sam', 'bilbo']
>>> len(hobbits)
3
```
we can use range with len all together to be able to iterate through a list using undex positions

```
>>> hobbits = ['frodo', 'sam', 'bilbo']
>>> len(hobbits)
3


>>> range(len(hobbits))
range(0, 3)


>>> list(range(len(hobbits)))
[0, 1, 2]


>>> for hobbitmember in range(len(hobbits)):
...     print(hobbits[hobbitmember])
... 
frodo
sam
bilbo
```

## Codewar two_sun puzzle 
x + i = target

```
  1 def two_sun(number,target):
  2     length = range(len(number))
  3     for i in length:
  4         for x in length:
  5                 if x == 0:
  6                     pass
  7                 elif x == i:
  8                     pass
  9                 elif number[i] + number[x] == target:
 10                     print(i,x)
 11                     break
 12 two_sun([0,1,2,3], 4)
```
## output would be 

```
student@lin-ops:~$ python 005_practice.py 
(1, 3)
(3, 1)
```

## Slicing 
lst[start:stop:step]

```
>>> lst = list(range(0, 11, 1))
>>> lst
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
>>> lst[0]
0
>>> lst[1]
1
>>> lst[4]
4
```
another way to traverse a list

## Example of slicing
## lst[start:stop:step] is how to utilize
```
>>> lst
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
>>> lst[0:10:1]
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
>>> lst[0::1]
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
>>> lst[0:-1:1]
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

>>> lst[2::]
[2, 3, 4, 5, 6, 7, 8, 9, 10]
>>> lst[2::2]
[2, 4, 6, 8, 10]
>>> lst[2::3]
[2, 5, 8]
>>> lst[2::4]
[2, 6, 10]

```

moving backwords now

```
>>> lst
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
>>> lst[::-1]
[10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
>>> lst[::-2]
[10, 8, 6, 4, 2, 0]
>>> lst[::-3]
[10, 7, 4, 1]
>>> lst[::-4]
[10, 6, 2]
>>> lst[:2:-1]
[10, 9, 8, 7, 6, 5, 4, 3]


```
the -1 in the step allows is to walk backwords in the list


## Guess the number Exercise
See below for solution and product

```
  1 #!/usr/bin/env python3
  2 
  3 def guess_number(n):
  4     while True:
  5         n = int(input('Enter a number between 0 and 100:\n'))
  6         if n > 23:
  7             print('Too high! Guess again...')
  8             continue
  9         elif n < 23:
 10             print('Too low! Guess again...')
 11             continue
 12         elif n == 23:
 13             print('You guessed correct')
 14             break
 15             
 16 guess_number(23)
```

Another solution

```

  1 #!/usr/bin/env python3
  2 
  3 def guess_number(n):
  4     while True:
  5         x = int(input('Enter a number between 0 and 100:\n'))
  6         if x > n and x < 100:
  7             print('Too high! Guess again...')
  8             continue
  9         elif x < n and x < 100:
 10             print('Too low! Guess again...')
 11             continue
 12         elif x == n:
 13             print('You guessed correct')
 14             break
 15         else:
 16             print('Number entered is outside question.')
 17             continue
 18        
 19 guess_number(23)


```
Worked
Enter a number between 0 and 100:
100
Too high! Guess again...
Enter a number between 0 and 100:
20
Too low! Guess again...
Enter a number between 0 and 100:
23
You guessed correct


## Dictionary

romanNumerals = {'I':1, 'V':5, 'X':10, 'L':50}

## dictionary = {'KEY':VALUE}
example of structure

```

>>> roman = {'I':1, 'V':5, 'X':10, 'L':50}
>>> roman['I']
1
>>> roman['V']
5
>>> roman['X']
10
>>> roman['L']
50

```

you can also add and remove things from the dictionary

ADDING
```
>>> roman['C'] = 100
>>> roman
{'I': 1, 'V': 5, 'X': 10, 'L': 50, 'C': 100}
```

DELETING
```
>>> roman
{'I': 1, 'V': 5, 'X': 10, 'L': 50, 'C': 100}
>>> del roman['I']
>>> roman
{'V': 5, 'X': 10, 'L': 50, 'C': 100}
```

PRINTING out the values from a dictionary

```
>>> for key in roman:
...     print('{} = {}'.format(key, roman[key]))
... 
V = 5
X = 10
L = 50
C = 100
```

## Inventory Practice
Working with dictionaries

first we need a movies listing with prices

```
movies = {'Ironman':40.0 ,'Hulk':20.0 ,'Thor':10.0 ,'Hawkeye':5.0, 'Pokemon':45.0}

```
next we need a order and a total

```
order = [('Ironman', 4), ('Pokemon', 1)]
  3 total = 0

```

now we need to be able to index through the list to grab the movie that is in the order

```
>>> for i in order:
...     print(i[0])
... 
Ironman
Pokemon

```

now we can pull the movie we will want to grab the value we need to find the calculation

```	
>>>order
[('Ironman', 4), ('Pokemon', 1)]
>>> order[0]
('Ironman', 4)
>>> order[0][0]
'Ironman'

```
using order[][] we are able to pull the index position index and index position inside the list


 ```

 1 movies = {'Ironman':40.0 ,'Hulk':20.0 ,'Thor':10.0 ,'Hawkeye':5.0, 'Pokemon':45.0}
  2 order = [('Ironman', 4), ('Pokemon', 1)]
  3 total = 0
  4 for i in order:
  5     total += (movies[i[0]]*i[1])
  6 
  7 print(total)
  8 
~                                                                                          
~
```                                     
## for i in order:
is allowing us to retreive the ('Ironman', 4) and ('Pokemon', 1)

## movies[i[0]] 
movies = {'Ironman':40.0 ,'Hulk':20.0 ,'Thor':10.0 ,'Hawkeye':5.0, 'Pokemon':45.0}

is pulling the first index posistion value within the list that was pulled by [i]

## movies[i[0]] 
movies = {'Ironman':40.0 ,'Hulk':20.0 ,'Thor':10.0 ,'Hawkeye':5.0, 'Pokemon':45.0}

would be Ironman and movies[i[1]] would be Pokemon

Final product

```
  1 movies = {'Ironman':40.0 ,'Hulk':20.0 ,'Thor':10.0 ,'Hawkeye':5.0, 'Pokemon':45.0}
  2 order = [('Ironman', 4), ('Pokemon', 1)]
  3 total = 0
  4 for i in order:
  5     total += (movies[i[0]]*i[1])
  6 
  7 print(total)
  8 

```


## *args and **kwargs

ignore the args and utlize as a tuple and not a script


```
 1 def myFuns(*args):
  2     print(args)
  3     print(type(args))
  4 
  5 myFuns(1,2,3,4,5)
  6 

(1, 2, 3, 4, 5)
<class 'tuple'>

                            
```
the following will step through all the numbers and add all the numbers until the very end
```


  1 def myFuns(*args):
  2     total = 0
  3     for num in args:
  4         print(num)
  5         total += num
  6 
  7     print(total)
  8 
  9 
 10 myFuns(1,2,3,4,5)
 11                    
```

More information on *ARGS

When your function can have a variable number of arguments, you can use args to contain all the arguments in a single variable to allow unpacking in order.
```
def doSum(*args):
    type(args)
    sum = 0
    for addend in args:
        sum += addend
    print("Sum is {}".format(sum))
doSum(1,2,3,4)
Sum is 10


```


## File I/O

open and close file i/o

```
fp = open("test.txt")
fp.close()

>>> fp = open("test.txt")
>>> fp.close()

```
'r'
Read (default)
with open("test.txt", 'r') as outfile:

'w'
Write
with open("test.txt", 'w') as outfile:


This will allow you to automatically open and close the file

```
>>> with open("test.txt") as fp:
...     pass
... 
```

Writing to a file


```
with open("test.txt", 'w') as outfile:
     outfile.write('firstline\n')
     lines = ('Second line\n', 'Third line\n', 'Fourth line\n', 'Last line\n')
     outfile.writelines(lines)


resulting in

firstline
Second line
Third line
Fourth line
Last line

```

reading to a file

```
>>> with open("test.txt", 'r') as fp:
...     fp.read()
... 

'firstline\nSecond line\nThird line\nFourth line\nLast line\n'


```

reading a certain number of characters

```
>>> with open("test.txt", 'r') as fp:
...     fp.read(5)
... 
'first'


```
another example of reading from a file

```
>>> with open("test.txt", 'r') as fp:
...     for line in fp: 
...             print(line)
... 
firstline

Second line

Third line

Fourth line

Last line

>>>> with open("test.txt", 'r') as fp:
...     for line in fp: 
...             print(line, end='')
... 
firstline
Second line
Third line
Fourth line
Last line
>> with open("test.txt", 'r') as fp:
...     for line in fp: 
...             print(line, end='')
... 
firstline
Second line
Third line
Fourth line
Last line

```

## The textfile, travel_plans.txt, contains the summer travel plans for someone with some commentary. Find the total number of characters in the file and save to the variable num.

```
num = 0
file = 'travel_plans.txt'
with open (file) as fp:
    num = len(fp.read())

```

## We have provided a file called emotion_words.txt that contains lines of words that describe emotions. Find the total number of words in the file and assign this value to the variable num_words.

```
num_words = 0
file = 'emotion_words.txt'
with open (file) as fp:
    sentences = fp.read()
    words = sentences.split()
    num_words = len(words)

```

so first we declare num_words and file
then we utilize the open as fp 
sentences is equal to the string read from emotion.txt
we then split strings into words using words
from there we len(words) to grab the number of words within words

## Assign to the variable num_lines the number of lines in the file school_prompt.txt.

```
num_lines = 0
file = 'school_prompt.txt'
with open (file) as fp:
    for line in fp:
        num_lines += 1
```
with the code block above we declare the num_lines variable and file 
we then use with open and assign it to fp
we say for 'LINE' in fp that will +1 for each and add to num_lines

## Assign the first 30 characters of school_prompt.txt as a string to the variable beginning_chars.

```
file = 'school_prompt.txt'
beginning_chars = ""
with open (file) as fp:
    beginning_chars = fp.read(30)

```

## Assign the first 33 characters from the textfile, travel_plans.txt to the variable first_chars.

```
file = 'travel_plans.txt'
first_chars = ""
with open (file) as fp:
    first_chars = fp.read(33)
```

## Using the file school_prompt.txt, assign the third word of every line to a list called three.

```
three = []
file = 'school_prompt.txt'
with open (file) as fp:
    strings = fp.readlines()
    for line in strings:
        word = line.split()
        three.append(word[2])
    

```

## More File IO 

with open ('emotions_words.txt') as fp:
	num_words = len(fp.read().split())


## How to grab first word from every line in a text file

file = 'emotion_words.txt'
emotions = []
with open (file) as fp:
    for line in fp:
        emotions.append(line.split()[0])

 ## how to pull a word from a text file that contains a letter

Using the file school_prompt.txt, if the character ‘p’ is in a word, then add the word to a list called p_words.
```
p_words = []
file = 'school_prompt.txt'
with open (file) as fp:
    for line in fp:
        for word in line.split():
            if "p" in word:
                p_words.append(word)
```

we are able to evaluate if a letter is inside the a word

if 'z' in zebra
true

if 'k' in zebra
false


## Grade a specific question
python3 script {#} (question that you want)











# Day 4
## Practice Exam Questions


## Given the floatstr, which is a comma separated string of floats, return a list with each of the floats in the argument as elements in the list.
```
def q1(floatstr):
	lst = []
	for x in floatstr.split(','):
		lst.append(float(x))
	return(lst)
```
TLO: 112-SCRPY002, LSA 3,4
Given the floatstr, which is a comma separated string of
floats, return a list with each of the floats in the 
argument as elements in the list.
'''
pass

## Given the variable length argument list, return the average of all the arguments as a float
```
def q2(*args):
	total = sum(args)
	amount = len(args)
	avg = float(total/amount)
	return(avg)
```

'''
TLO: 112-SCRPY006, LSA 3
TLO: 112-SCRPY007, LSA 4
Given the variable length argument list, return the average
of all the arguments as a float
`''
pass


## Given an input string, return a list containing the ordinal numbers of each character in the string in the order found in the input string.

```
def q4(strng):
	lst = []
	num = []
	for i in strng:
		lst.append(i)
	for x in lst:
		sm = ord(x)
		num.append(sm)
	return(num)
```
'''
TLO: 112-SCRPY004, LSA 1,2
TLO: 112-SCRPY006, LSA 3
Given an input string, return a list containing the ordinal numbers of 
each character in the string in the order found in the input string.
'''
pass








