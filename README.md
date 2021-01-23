# python3_basics

Python is a general-purpose coding language.
Unlike HTML, CSS, and JavaScript, it can be used for other types of programming and software development besides web development. It is a cross platform,object-oriented programming language, comparable to Perl, Ruby, Scheme, or Java.

#### Let's check installed python version.

``python --version
``

If python is not installed, download it for free from the following website: https://www.python.org/

#### Interpreted programming language

Developer can write Python (.py) files in a text editor and then put those files into the python interpreter to be executed.

### First Coding experience

create ``helloworld.py`` file and put following line in it.

``print("Hello, World!")``

Open a cmd inside the folder where the ``'helloworld.py'`` is in and run following command.

``python helloworld.py``

#### Run python code within the cmd it self.

Type ``python`` or ``py`` in the cmd
This convert the cmd to python command line.

Then print("Hello, World!") can be run with there it self, no need of a file.

Use ``exit()`` to exit from python command line. 

### Python Indentation

Indentation is used to indicate a block of code.

````
Correct
if 6 > 4:
  print("Six is greater than four!")
````
````
Syntax Error
if 6 > 4:
print("Six is greater than four!")
````
The number of spaces is up to you as a programmer, but it has to be at least one.
````
Correct
if 6 > 4:
 print("Six is greater than four!") 
if 6 > 4:
        print("Six is greater than four!") 
````
````
Syntax Error
if 6 > 4:
 print("Six is greater than four!")
        print("Six is greater than four!")
````
### Python Comments

Used to explain Python code, make the code more readable or to prevent execution of code.

python comments starts with a ``#``

````
#This is a comment
print("Hello, World!")
````

### Multi Line Comments

Python does not really have a syntax for multi line comments. To add a multiline comment need to insert a # for each line.

````
#This is a 
#multi line 
#comment
print("Hello, World!")
````

Since Python will ignore string literals that are not assigned to a variable, multiline string (triple quotes) can be used to place multi line comment inside it.

````
"""
This is a 
multitline
comment
"""
print("Hello, World!")
````
### Variables

Variables are containers for storing data values. Python has no command for declaring a variable.A variable is created the moment a value is assigned to it.

````
x = 6
y = "Mike"
print(x)
print(y)
````
Variables do not need to be declared with any particular type, and can even change type after they have been set. Though it is not recomend to do so.

````
x = 6      # x is of type int
x = "Mike" # x is now of type str
print(x)

--output--
  Mike
````
### String Variables

String variables can be declared either by using single or double quotes.

````
x = "Mike"
# is the same as
x = 'Mike'

--output--
  Mike
````

### Case-Sensitive

Variable names are case-sensitive.

````
a = 4
A = "Mike"
#A will not overwrite a
````

### Casting

If you want to specify the data type of a variable, this can be done with casting.
````
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
````

### Get the Type

You can get the data type of a variable with the ``type()`` function.

````
x = 5
y = "Mike"
print(type(x))
print(type(y))

--output--
<class 'int'>
<class 'str'>
````

### If ... Else
Simple ``if`` example
```
a = 3
b = 20
if b > a:
  print("b is greater than a")
```

### Elif
Python way of telling if the previous condition is not true check this condition
````
a = 3
b = 3
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
````

### Else
The ``else`` keyword catches anything which isn't caught by the preceding conditions.
````
a = 3
b = 3
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
````
### Python Loops
Python has two primitive loop commands

while loop and
for loop

``while`` loop executes a set of statements as long as a condition is true
````
i = 1
while i < 5:
  print(i)
  i += 1
  
--output--
1
2
3
4
````

### break Statement
``break`` statement stops the loop even if the while condition is true
````
i = 1
while i < 5:
  print(i)
  i += 1
  if i == 3:
    break
  
--output--
1
2
````

### continue Statement
``continue`` statement stops the current iteration, and continue with the next
````
i = 0
while i < 5:
    i += 1
    if i == 3:
        continue
    print(i)
  
--output--
1
2
4
5
````

### else Statement
``else`` statement runs a block of code once when the condition no longer is true
````
i = 1
while i < 5:
  print(i)
  i += 1
else:
  print("i is no longer less than 5")
  
--output--
1
2
3
4
i is no longer less than 5
````

### List
Lists are used to store multiple items in a single variable.
Lists are created using square brackets,
```
samplelist = ["item1", "item2", "item3"]
```

### List Length
len() function determines how many items a list has
```
samplelist = ["item1", "item2", "item3"]
print(len(samplelist))

--output--
  3
```

List items can be of any data type or types

```
samplelist1 = ["item1", "item2", "item3"]
samplelist2 = [1, 2, 3, 4, 5]
samplelist3 = [ True, False, False, True ]
samplelist4 = [ True, "item1", False, 5 ]
```

### Access Items
List items are indexed so the index number can be used to access them
```
samplelist1 = ["item1", "item2", "item3"]
print(samplelist1[0])

--output--
  item1

Note: The first item has index 0.
```

### Negative Indexing
Negative indexing used to access items from the reverse or from the end, -1 refers to the last item, -2 refers to the second last item etc.
```
samplelist1 = ["item1", "item2", "item3"]
print(samplelist1[-1])

--output--
  item3
```

### Range of Indexes
Specify a range of indexes by specifying where to start and where to end the range. This will return a new list with specified items.
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
print(samplelist1[1:3])

--output--
['item2', 'item3']

Note: The search will start at index 1 (included) and end at index 3 (not included).
```
Folliwing will return the items from the beginning to, but NOT including, ``"item4"``
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
print(samplelist1[:3])

--output--
['item1', 'item2', 'item3']
```
This will return the items from the ``"item3"`` to end
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
print(samplelist1[2:])

--output--
['item3', 'item4', 'item5']
```

### Check if Item Exists
Use the ``in`` keyword to determine if the specified item present in the list
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
if "item2" in samplelist1:
  print("Yes, 'item2' is in the list")

--output--
Yes, 'item2' is in the list
```

### Change Item Value
Refer to the index number to change the value of a specific item
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1[1] = "updatedItem2"
print(samplelist1)

--output--
['item1', 'updatedItem2', 'item3', 'item4', 'item5']
```
### Change a Range of Item Values
Define a list with the new values, and refer to the range of index numbers to insert the new values

```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1[1:3] = ["uptatedItem2", "updatedItem3"]
print(samplelist1)

--output--
['item1', 'uptatedItem2', 'updatedItem3', "item4", 'item5'] 
```
Replace 3 items with 2 items
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1[1:4] = ["uptatedItem2", "updatedItem3"]
print(samplelist1)

--output--
['item1', 'uptatedItem2', 'updatedItem3', 'item5']

Note: Here 3 items replaced by the new list of 2 items 
```

Replace 1 items with 2 items
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1[1:2] = ["uptatedItem2", "updatedItem3"]
print(samplelist1)

--output--
['item1', 'uptatedItem2', 'updatedItem3', 'item3', 'item4', 'item5']

Note: Here 1 items replaced by the new list of 2 items 
```
### Append Items
Use the `append()` method to add item to the end of the list
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1.append("item6")
print(samplelist1)

--output--
['item1', 'item2', 'item3', 'item4', 'item5', 'item6']
```

### Insert Items
Use the `insert()` method to insert an item at a specified index
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1.insert(1, "insertedItem")
print(samplelist1)

--output--
['item1', 'insertedItem', 'item2', 'item3', 'item4', 'item5']
```

### Extend List
Use the `extend()` method to append elements from another list to the current list
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist2 = ["item6", "item7", "item8"]
samplelist1.extend(samplelist2)
print(samplelist1)

--output--
['item1', 'item2', 'item3', 'item4', 'item5', 'item6', 'item7', 'item8']
```

### Remove Specified Item
The `remove()` method removes the specified item
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1.remove("item4")
print(samplelist1)

--output--
['item1', 'item2', 'item3', 'item5']
```

### Remove Specified Index
The `pop()` method removes the specified index, It removes the last item if the index is not specified
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1.pop()
print(samplelist1)

--output--
['item1', 'item2', 'item3', 'item4']

Note: Last item is removed
```
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1.pop(1)
print(samplelist1)

--output--
['item1', 'item3', 'item4', 'item5']

Note: Item at index 1 is removed
```
### del Key Word
The `del` keyword also removes the specified index

```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
del samplelist1[1]
print(samplelist1)

--output--
['item1', 'item3', 'item4', 'item5']
```
### Clear the List
Use ``clear()`` to remove all the items in the list
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
samplelist1.clear()
print(samplelist1)

--output--
[]
```
