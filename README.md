# python3_basics

General-purpose coding language
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
if 5 > 2:
  print("Five is greater than two!")
````
````
Syntax Error
if 5 > 2:
print("Five is greater than two!")
````
The number of spaces is up to you as a programmer, but it has to be at least one.
````
Correct
if 5 > 2:
 print("Five is greater than two!") 
if 5 > 2:
        print("Five is greater than two!") 
````
````
Syntax Error
if 5 > 2:
 print("Five is greater than two!")
        print("Five is greater than two!")
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
#This is a comment
#written in
#more than just one line
print("Hello, World!")
````

Since Python will ignore string literals that are not assigned to a variable, multiline string (triple quotes) can be used to place multi line comment inside it.

````
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
````
### Variables

Variables are containers for storing data values. Python has no command for declaring a variable.A variable is created the moment you first assign a value to it.

````
x = 5
y = "John"
print(x)
print(y)
````
Variables do not need to be declared with any particular type, and can even change type after they have been set. Though it is not recomend to do so.

````
x = 4       # x is of type int
x = "Sally" # x is now of type str
print(x)
````

### Casting

If you want to specify the data type of a variable, this can be done with casting.
````
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
````
