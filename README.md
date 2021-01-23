# python3_basics

Python is a general-purpose coding language.
Unlike HTML, CSS, and JavaScript, it can be used for other types of programming and software development besides web development. It is a cross platform,object-oriented programming language, comparable to Perl, Ruby, Scheme, or Java.

#### Let'scheck installed python version.

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
````
### String Variables

String variables can be declared either by using single or double quotes.

````
x = "Mike"
# is the same as
x = 'Mike'
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

output
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

output
item1

Note: The first item has index 0.
```

### Negative Indexing
Negative indexing used to access items from the reverse or from the end, -1 refers to the last item, -2 refers to the second last item etc.
```
samplelist1 = ["item1", "item2", "item3"]
print(samplelist1[-1])

output
item3
```

### Range of Indexes
Specify a range of indexes by specifying where to start and where to end the range. This will return a new list with specified items.
```
samplelist1 = ["item1", "item2", "item3", "item4", "item5"]
print(samplelist1[1:3])

output
['item2', 'item3']

Note: The search will start at index 1 (included) and end at index 3 (not included).
```


