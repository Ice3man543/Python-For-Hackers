# Python For Hackers | Part. 1
#### Written By : @Ice3man (EthanTom)
#### Email : [ThomasEthan@protonmail.com](mailto:ThomasEthan@protonmail.com) 
#### Github : [https://github.com/Ice3man543/](https://github.com/Ice3man543/) 
###### File : Python For Hackers.md | Last Edited : October 6, 2017 4:25 PM

---

### Table of Contents 

- Introduction to the World of Python
- Beginning with the Interactive Console.
- Varibles - The Building blocks.
- Operators - The Elementary Concepts.
- Lists - oh the Beautiful Lists.
- Conditional Statements and Iteration.
- Dictionary - an advanced list.
- File IO - Expanding on basics
- Object Oriented Programming 
- Homework And Notes



- - -


### 0x00 | Introduction To The World of Python

Python is a modern language which was designed in the early 1990's by ==Guido van Rossum== at Stichting Mathematisch Center in the Netherlands as the successor of a language called ABC. This language has gained wide acceptance in the scientific and hacker communities as a language which is easy to program, easier to read and still easier to grasp. But do not let it's simplicity fool you, It is one of the most powerful programming lanugage. In fact, it's the most-used language by the Tech Giant Google who has used it for a variety of programs. From the Google Youtube Platform to the DeepMind Machine Learning Program, everyone at Google uses Python for tasks which are just mind-blowing.

Python is widely supported and runs on just about any platform imagined.
The power of Python comes from it's community mad and pre-built modules which are bundled with the language. In fact, there is a module for every one of your need in python.
Starting with Python is easy. If you've never programmed before, I suggest you start with this language. It will teach you the core and crux of programming before you dive in deeper.


- - -


### 0x01 | Beginning with Interactive Console

Just to remind you, there are two prominent versions of Python - Python2.7 and Python3. We are using Python2.7 here and it is recommended for you to use it because of many differences that exist between the two. If you are using a linux machine, then it is more convenient as I am also using a Debian Machine., for starters I assume you have Python 2.7 installed. If haven't then you can install it using you distro's package manager. For debian :-

```bash
sudo apt-get install python
```

If you are using Windows Or Mac, it is pretty easy for you to install Python. Just download the official point-and-click installers from Python website.

Now, assuming that you have successfully installed Python and are up and running. So let's get started in our journey to the magical kingdom of Python and it's modules.

Python has an interactive console which can be used to tinker around with code and view output of some statements or debug a certain piece of code. It can also be used as a starting platform to learn about the language.
To drop into the interactive mode, there is not much to do. Simply type in the command,

```bash
[~]$ python
```

So, here is the python interactive console.

![Interactive Window](img/Interactive_Python_Window.png)

Ok, So now let's begin with the traditional Hello World Approach.
Writing Hello World is very easy but it is a building block for you to learn the features of a language and evolve from the Hello World to some very complex programs. That's why most programming books start with a hello world example.

Type this line into interactive console and you are done.

```python
print "Hello World"
```

And gently press enter. There you go, you have created your first python program. If it prints ==Hello World== on the screen then give yourself a pat on the back. You are now a programmer and you have created your first computer program.

Let's break down the code line statement by statement 
- The first statement print is a built in python command which is used to print something to the standard output which is generally your monitor screen. 
- The Hello World Enclosed in "" is a string in terms of python. A String is just a group of characters. 

We call the **print** function with the string as it's argument. But, it's not the only way to call a function. There are many more methods.

```python
print "Hello World"
print("Hello World")
```

These are two different statements but they all print the same thing - Hello World.
Let's move on. There is not much left in printing.

### 0x02 | Variables - The Building Blocks

Variables are the building blocks of modern computer computer programming. In simplest terms, a variable is a named memory location which holds a certain piece of data. For example, let us consider a fridge. A fridge has different sections and places to keep different items. There are compartments for eggs, fruits, water bottles, etc. Each of this can be considered a variable because a variable is simply a holding place for some data. If it's still not clear, then we will make it clear later.

There are two types of computer programming languages.
- Dynamic Typed Language
- Static Typed Languages

Dynamicaly typed languages are like a fridge which has many sections of different sizes without a named usage and it's upto you decide what you want to put in each section. Speaking simply, it offers no specifier to define what kind of data a variable can hold. Every varaible can hold absolutely everyting.

On the other hand, static typed languages like C have different data types for different kinds of data. It can be considered as a fridge having named section of specific size for holding a specific item. One item cannot go inside a section for different item. For Example, In C Programming lanugage, an Integer can't hold a character value and a **character array** can't hold an integer.

So, how to declare a variable. It's easy - just choose a name for your variable and assign something to it.
If I want to create a variable holding my English marks - here is how I would do so.

```python
english_marks = 94
```
Code breakdown.
- **english_marks** is the variable name that we have decided.
- **=** is the assignment operator. It is used to assign something to something. In simple english, it means put value of 94 into english_marks.

Ok, it was the most simple discription of the variables.
A variable can hold any value you intend. Here is use of different variables types.

```python
my_name = "@Ice3man"
my_class = 12
my_section = 'B'
my_precent_marks = 97.5
```

Code Breakdown -
- The Variable **my_name** is a string which holds @Ice3man as my name. I told you about strings earlier. String are just an array (group) of characters.
- The Variable **my_class** is an integer type. You must be knowing Integers from your schoool. Every number is an integer.
- The Variable **my_section** is a character type which holds a single character. For now, it holds B which is my section.
- The Variable **my_precent_marks** is a floating type variable or in simpler terms, decimal variable. It holds marks which are in decimal.

We now know how to declare variables. There are some special variables types which we will take a look later.
Let's look at how to access variables.

Accessing a variable is very easy if you know it's name. Just type it's name and you can acess it.
```python
precent_water_on_earth = 71
print precent_water_on_earth
```
In the above code, we first declare a variable **precent_water_on_earth**. Then we use a print statement with the variable name as argument to print it on the screen. But this method is not much efficient.

The user does not knows what 71 refers to. It could mean anything. So, it is advised to use string cocantenation to create a nice output. Strings can be cocatenated using + operator. Here is a better example.

```python
precent_water_on_earth = 71
print "Precentage Of Water On Earth : " + precent_water_on_earth
```
Let's run it. The above code will give you a nasty error complaining about that **it cannot cocatenate str and int objects.**

The reason is embedded in the last paragraph where I defined Static Typed languages. Actually, python is a dynamically typed language does not means that python doesn't maintain the distinction between different types of data types. It simply means that Python provides an abstraction layer to us programmers so we can simply do our job without having to worry about variable type to choose. But, Internally it maintains a record of our variables, their types, the values they hold and it also restricts us to use two different types of variables together. 

In the code of printing precent of water of earth, the second statement is simply cocatenation of string "Precentage Of Water On Earth : " and **Integer** precent_water_on_earth. Thus, the operation is not allowed by Python. The way we can overcome this is by changing it into string object using str method. This should work. 

```python
precent_water_on_earth = 71
print "Precentage Of Water On Earth : " + str(precent_water_on_earth)
```
I hope you will remember this distinction of different data types from this example. It will surely come in handy.

Let's take a more complex example.
For Example, if i want to print my details from the last example in a nice format we can do that using this code.

```python
my_name = "@Ice3man"
my_class = 12
my_section = 'B'
my_precent_marks = 97.5

print "My Name : " + my_name
print "My Class : " + str(my_class)
print "My Section : " + my_section
print "My Precentage Marks : " + str(my_precent_marks)

```

Here is the output from my Interactive window.

![Output_marks](img/Output_My_Marks.png)

This method is good but suppose we have four or five arguments we want to print on a single line. Or maybe we just want to print all info in a single line. So, in that scenario we are rendered somewhat limited by simple string cocantenation. Thus, format strings to the rescue.

If you have ever programmed in C, you must be remembering *printf*. If not, then let me tell you.

Format Strings are special wildcards in the string which when encountered by *print* or *printf* function halts the execution, gets the next argument passed to the function and displays it uses the kind of format string given.

Some common format string 

| Format String | Type to print |
|--------|----------------------|
|  %s    | String    			|
|  %c	 | Character 			|
|  %f    | Float (decimal)		|
|  %i    | Integer   			|
|  %x    | Hexadecimal			|

There are many more, but these are more than enough for us.

Let's rewrite the info printing code using our newly acquired knowledge of format strings.

To specify a format string, we use print method with a string and our format arguments inside it. After closing the " we put a precentage sign % followed by brackets () and put all format strings argument variable names inside it.

```python
my_name = "@Ice3man"
my_class = 12
my_section = 'B'
my_precent_marks = 97.5

print "My Name : %s My Class : %i My Section : %c My Marks precent : %f" % (my_name, my_class, my_section, my_precent_marks)

```

As you can see our code has improved a lot. Also, we don't need to convert anything to string as our format string %s already does it. Isn't it better.

### 0x03 | Operators - The Elementary Concepts

Operators are very useful in Computer programming. You can think of an operator in terms of your mathematics operators. You have used many of them like Add, Subtract, Multiply. These are the Fundamental things that make computers such a powerful tool. 

Python has a number of operators which are used for different tasks. We will begin with Arithmetic operators.

Arithmetic operators are the most basic operators and are used to perform simple mathematical computations. A combination of these simple operators can be used to solve infinitely complex problem. Some arithmetic operators are -


| Operator | Task 	 |	Example	|
|----------|---------|----------|
|   +      |   Adds two numbers    | 5 + 5 = 10 |
|   -      |Subtracts two numbers | 5 - 5 = 10  |
|   *      |Multiplies two numbers| 5 * 5 = 25
|   /      |Divides two number    | 5 / 5 = 1   |
|   ****     |Power of (exponential) | 5 **** 5 = 3125 |
|   %      |Modulus (Returns remainder) | 5 % 5 = 0 |

We could easily write a program to perform all these operations on different numbers. But, I am tired of typing in interactive console. So, let's learn how to code a python program in a file and run it from there.

Python script file usually have an extension of .py . There are many IDE's for Python development but We are gonna use a text editor to write our code. Now comes the choice of editors. If you are using windows, you have got Notepad++ which is awesome, Sublime Text but it costs money for Full Version. If you are using linux, you can use nano, vi, Sublime Text :-), etc. I will use sublime text to write the code in linux. So open up your respective text editors. 

Let's begin typing our code.

```python
#!/usr/bin/python

num1 = 5 
num2 = 3

add = num1 + num2
sub = num1 - num2
mul = num1 * num2
div = num1 / num2
exp = num1 **** num2
mod = num1 % num2

print "Addition : %d Subtraction : %d Multiplication : %d Divison : %d Raised To (exp) : %d Modulus : %d" % (add, sub, mul, div, exp, mod)

```

Code breakdown -
- The First line *#!/usr/bin/python* is the standard Python shebang line which allows your computer to interpret the file as a python script.
- The other lines are easy to understand and I hope there is not need to explain them.
- Finally, we print the output in a single line.

Now comes the question of running our script. On windows it is easy. Just navigate to directory and run the script by typing the name of script by passing it as an argument to python.exe. On linux it is a bit more complicated.

First things first. You need to give execute permission to the file. To do this, navigate to the directory where you created the script. Now, type the following command.

```bash
chmod +x arithmetic.py
./arithmetic.py
```
- In the first line, we set execute permission on our file which is **arithmetic.py**.
- Next we execute it using **./arithmetic.py** statement.

Here is output from my sample run.
![Sample_File_run](img/sample_file_run.png)

The script runs well. Now, we know some things about how arithmetic operators work.

The next type of operator we are going to learn are called Conditional Operators. These are used to perform comparison between different values and return a boolean value. Boolean values are special values which state only two type of conditions, either True or False.

A Conditional Operator is mostly used in combination with a conditional statement such as an if statement. A Computer which can only perform arithmetic operations is of no use if it cannot perform logical tasks. For Example, if you are taught only what numbers are and how many numbers are there. Then you cannot know if 1 is greater than 5 or 5 and 5 are equal because you have been taught only the one side of the matter.

A computers needs to be able to compare things and perform branching which simply means jumping to another line in code.

There are many conditional operators and some of them we will have a look here. Maybe you know them from your maths class.

| Operator | Task | Example |
|--------|--------|---------|
| >      |  Is greater than | 1 > 2 = False |
| <		 | Is less than | 1 < 2 = True |
| == 	 | Is equal to  | 2 == 2 = True |
| >=     | Is greater than or equal to | 3 >= 2 = True |
| <=     | Is less than or equal to | 2 <= 3 = True |
| !=     | Is not equal to | 3 != 3 = True |

You must note that **==** is different than **=** operator. **=** means assignment operator. It used to assign a value to the operand.

You can write a program to check all these conditions. Or simply dive into the interactive console to execute them and check the result on the fly. Here's my terminal.

```python
>>> a = 10
>>> b = 5
>>> 
>>> a > b
True
>>> a < b
False
>>> a == b
False
>>> a >= b
True
>>> a <= b
False
>>> a != b
True
```

> Interactive Console is one of the biggest advantage of using Python in my opinion.   _@Ice3man

If you've had enough experiment with conditional statement, we can move forward to Assignment operators.

Asssignment Operators are basically used to assign something to a variable, most probably a value to the variable. There is not much to know about assignment operators except that they can be combined with arithmetic operator to create a short form for an statement.

| Operator | Task  | Example |
|--------|--------|----------|
|   =     | Assign value of right operands to left operand. | c = a + b |
|  +=     | Adds right operand to left and assign it to left.| b+=a (b=b+a) |
| -=  | Subtracts right operand to left and assign it to left.| b-=a (b=b-a) |
| *=  | Multiplies right operand to left and assign it to left.| b*=a (b=b*a) | 

And so on. These are called Compound Assignment Operator. There is not much to check about them. So there is no code for this part.

Next come bitwise operator. Data at the lowest level in the computers consists of Bits. 8 bits make a byte. Almost all programming languages provide the functionality to work with bits including python.
