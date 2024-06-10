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








