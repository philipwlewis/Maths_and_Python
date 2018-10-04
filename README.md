# First Steps with Python

To run Python code on a computer it must have the Python "interpreter" software installed.

To start we’ll take a shortcut and use a website which lets you code by connecting you to a computer on the internet that runs Python.

Open up a new browser window and go to:

[https://www.pythonanywhere.com/embedded3/](https://www.pythonanywhere.com/embedded3/)

The site should look like this:

![PythonAnywhere Web Console](https://photos.app.goo.gl/dE88THxp6TjnkwfF8)

The black part of the screen is a Python *terminal* or *console*. This is a place where you can enter *input* (the text which makes up your code) and which displays *output* (the results of your code).

You should see the following prompt:
 ```In [1]:``` 

This is the command line (a line where you can enter commands). `In[ ]` means it's a line which takes input. 

The number here initially set to `[1]` is a counter indicating the number of commands you have entered since starting the terminal.

Click your cursor anywhere in the *terminal* screen. Anything you type should now appear on the command line.

Type the following into the terminal:

```
print("hello world")
```

Then press enter. 

Be careful to use the right type of brackets, and note that we need to use speech marks or double quotes `""` when defining some text that we want Python to display.

You should see the following:

```
In [1]: print("hello world")
hello world

In [2]:
```
If so _Congratulations!_ You're a computer programmer and just run your first piece of code.

If you see an error message _Congratulations!_ You’re a computer programmer because you’ve just made your first coding mistake!

Inventor Thomas Edison was quoted as saying his work was involved 1% inspiration and 99% perspiration. The same might be said of computer programming. In my experience the majority of time spent computer programming is receiving errors and trying to solve them rather than seeing code run successfully.


**Exercise** 
_Write a command to get the computer to display your name._

There are numerous ways in which you can make mistakes when computer programming, and you shouldn’t feel put off if you make them. As you work through programming tasks you'll become familiar with more common errors, and develop approaches to investigate and solve errors that you haven't seen before.

In order to solve any problem you may sometimes find it useful to be able to take a snapshot of your screen which you can email or post in a help forum. If you are not sure how to do this you can find instructions here:

[http://www.take-a-screenshot.org/](http://www.take-a-screenshot.org/)

#### Exercise. Take a screenshot of the Python terminal screen.


# Installing Python on your computer

There are many different ways to install Python and work with code on your computer. In this module we will use [Anaconda](https://www.anaconda.com/download/) that includes a copy of the Python libraries and some tools that allow us to program with it. There are versions for Windows, MacOS and Linux, and it is installed on the UCL cluster room machines. 

To find and launch Anaconda on a UCL desktop, open the Windows menu and look for Anaconda3 (64bit) or type Anaconda in the search box. Click on "Anaconda Navigator".

To install Anaconda on your own machine perform the following steps:

- Go to	https://www.anaconda.com/download/. 
- Select and download installer for Python version 3.6.
- Run the installer program. (You will have an option to also install vscode, but can leave this unchecked as we will not be using it).

When Anaconda has installed find Anaconda Navigator in your application menu and start it.

**If you have problems using Anaconda or Spyder on the UCL computers or your own computers you can instead complete the exercises below using the online Python console at [https://www.pythonanywhere.com/embedded3/](https://www.pythonanywhere.com/embedded3/)**

### Spyder
Spyder is an application that lets us work with Python code files and run Python code. You should be able to launch it from the Anaconda Navigator menu.

When Spyder starts up you should see the following:

![Spyder Application](https://photos.app.goo.gl/bkFSPAWrjYfXwL8X6)

Panel 1 is the **Editor** panel. Any files you open will be seen as a "tab" in this panel. If you have no files open Spyder will create a code file `untitled.py` for you to work in.

Panel 2 displays some useful information. Here you can view one of three tabs:
- _Help._ This allows you to view the Python documentation. To open up the help page on a particular command, select it with your mouse and press *ctrl-i* (Windows) or *cmd-i* (MacOS).
- _Variable Explorer._ This shows information on the objects that Python has stored in the computer's memory. 
- _File Explorer._ This shows the current working directory. Double clicking on a file will open it in in the **Editor** panel. The directory shown will be the default location that Python searches when opening files.

Panel 3 is a **Python console**. When you run Python code any messages or output will be shown in this panel. The `In  []:` prompt is called the *command line* where you can  enter Python commands directly, or you can also run code that you are working on in the *Editor* panel. 


## Getting Started with Python

Let’s begin exploring how we can use Python to do calculations. You can complete these exercises either in Spyder, by typing into the Python console (lower right hand panel), or alternatively using the browser based version of Python we used earlier.


As we’ll be running short commands we’ll use the command line so click inside the Python terminal window to select it.

Type the following (it should appear after the `In[2]:` command line prompt), then press *Enter*.

`1+1`

You should see the following (depending on how many commands you’ve run the line count number might be different from 1):
```
In [1]: 1+1
Out[1]: 2

In [2]:
```

So far so good! The symbols used by Python for maths are:

   `+` add
   `-` subtract
   `*` multiply
   `/` divide

**Exercise** 
_Perform the following calculations on the Python command line._
  i. 78 plus 41
  ii. 391 minus 23
  iii. 23 multiplied by 26
  iv. 1250 divided by 5

Python also allows us to work with powers using the `**` operator. For example the following code calculates $5^2$:
```
In [1]: 5**2
Out[1]: 25
```

### Ordering of mathematical operations
Try out the following commands using Python.
```In[]: 9 + 2*7```
```In[]: 9+2 * 7```
```In[]: 9 + 2 * 7```
```In[]: 9+2*7```

You should find the same answer in each case (`23`). Python ignores white spaces which separate numbers and symbols, and adding spaces into a calculation make no difference to how the result is worked out.

If Python receives a calculation that contains a mixture of `+` `-` `*` `/`  `**` operations it will calculate any powers first, then multiplications and divisions, then additions and subtractions.

For example the calculation:
```
In[1] : 10*4**2+7*4-1
```

is resolved as:

`10*4**2 + 7*4 - 1` = `10*16 + 7*4 - 1` = `160 + 28 - 1` = `187`  

If you want to tell Python to perform the calculation in a different order you can use brackets `(` and`)`. 

Anything within brackets is calculated first, so `(10*4)**2` would produce the result  `1600`.

Note. You can only use the round brackets `(` and`)` to group the order of a calculation.  Other backet symbols can not be used e.g. on a keyboard we can also find _square brackets_ `[` and `]`, _curly brackets_ `{` `}`, and triangular brackets `<` and `>`  (the less and greater than symbols).

#### Exercises.

i) What is the result of the command
```In[]: 6+9/3+2```

ii) What is the result of the command
```In[]: (6+9)/3+2```

iii) What is the result of the command
```In[]: (6+9)/(3+2)```

iv) What command is needed to calculate `3` plus `4` all multiplied by `8`.

v) What command is needed to add `3` to the result of `4` multiplied by `8`.

More complicated calculations may require nested brackets (where one bracket contains another). In this case the innermost brackets will be calculated first, followed progressively by the outer ones. For example:

`(10+(2*3))/8` = `(10+6)/8` = `16/8` = `2`.

### Variables: a way to store and reuse values

In a computer program we use *variables* to store values so that we can access and update them as our program runs.

Here are some examples of how we can set up variables in Python:

```In [1]: x=2```

```In [2]: a=8.5```

```In [3]: b=4.1```

```In [4]: measurement1=34.92```

Setting up a _variable_ in a computer program means assigning a name that acts as a label for a number or other data object stored by the computer (e.g. a piece of text).

You'll notice that when a calculation or value is assigned into a variable Python does not display its value using an `Out []:` line. 
 
This is because the result of the command is being stored into a variable and Python only displays results and values after a command entry when the output is not stored.

In order to see a value in the command line we can type its name or alternatively  use the `print` command:

```
In [1]: a=8.5

In [2]: a
Out[2]: 8.5

In [3]: print(a)
8.5
```
We might read the commands above as

_1: Let variable `a` be equal to 8.5_

_2: Evaluate the current value of variable  `a`._

_3: Display the value of `a` on the screen._

When we want to access the stored information we can refer to our variables in calculations or other code.  For example:
```
In[1]: a=8.1

In[2]: b=4.1

In[3]: a+b
Out[3]: 12.2
```

Note that here the equals sign `=` acts as a variable assignment command. In programming the variable name always comes first and its value second i.e. _variable name_ = _value_.

As a program runs the values of the variables might change - this is why they are called variables! Let’s change the value of a.
```
In [4]: a=1.2

In [5]: a+b
Out[5]: 5.3
```

We can create new variables that store the result of a calculation using existing variables:
```
In [6]: c=a+b

In [7]: c
Out[7]: 5.3

In[8]:print(c)
12.6
```

An interesting question here is what will happen to variable `c` if we change the value of `a` or `b`?

```
In [1]: a=1.2

In [2]: b=4.1

In [3]: c=a+b

In [4]: c
Out[4]: 5.3

In [5]: a=3.1

In [6]: c
Out[6]: 5.3
```

We see that in this case once `c` has been calculated it does not change when we update `a`. If we wanted to update it we can recalculate it after changing `a`.

```
In[7]: c=a+b

In [8]: c
Out[8]: 7.2
```

You are free to choose the variable names. It's a good idea to try to use a name associated with the data that is stored (but not something too long-winded). For instance a variable containing the height measurement of a plant might be called `h` or  `height`.

The underscore character `_` can be used to break up a long variable name and make it easier to read e.g. `leaf_width_cm`, `total_population`. You can usually find the underscore on the same key as the minus sign, if you hold down shift. 

However note that variable names:
- cannot contain spaces. (`big_num=1000` is allowed but `big num=1000` is not.)
- cannot start with a number. (`val1=42` is allowed but `1st_val=42` is not.)
- cannot contain a dash, as this represents the minus operation. (`my_val=12` is allowed but `my-val=12` is not).
- should not be a word that is already used by Python (we will meet these later, but some of these are: `int`, `float`, `str`, `for`, `if`, `while`, `sum`, `len`).

### Reseting the terminal

Sometimes we might want to clear all the values of the variables we created. In the IPython you can do this by typing:

`%reset`

You’ll need to press the `y` key to confirm you want to delete all your variables in the computer's memory.

For example:

```
In [1]: a=1.0

In [2]: print(a)
1.0

In [3]: %reset
Once deleted, variables cannot be recovered. Proceed (y/[n])? y

In [4]: print(a)
---------------------------------------------
NameError   Traceback (most recent call last)
<ipython-input-39-c5a4f3535135> in <module>()
----> 1 print(a)
NameError: name 'a' is not defined
```

### Types of number

Look at the following code:

```
In [1]: a=2

In [2]: b=2.0
```
Mathematically both `a` and `b` have been assigned the same value. However because of the way we created the variables Python stores the two values with different data types. We can examine the type of data stored in a variable using the `type` command:


 ```
In [1]: a=2

In [2]: b=2.0

In [3]: type(a)
Out[3]: int

In [4]: type(b)
Out[4]: float
```

An `int` (short for integer) is the Python data type used to store a whole number values, e.g. `1, 7, 43, -12, 10234894,`. 

We might use `int` variables when:
- we deal with quantities that take whole number values. (population numbers, copy numbers)
- we make use of a counter in our computer program (e.g. repeat this 10 times) 
- we need to look up a value stored in a set (e.g. find the forth number in this list). 

A `float` (short for floating point number) is a Python data type used to store decimal numbers (e.g. `10.9`, `3.1459`, `-202341.5`).

We use this type of number in cases where a variable value might take a non-whole number value (e.g. when dealing with measurements.) In this case the computer needs to keep track of the decimal places in calculations.

When you type in a number Python will automatically treat it as an integer or floating point number, dependant on whether you include a decimal point. For example:
```
In [8]: type(999)
Out[8]: int

In [9]: type(999.9)
Out[9]: float

In [10]: type(999.)
Out[10]: float
```
Note. We see here that Python also allows you to specify a float type number by adding a decimal point only (i.e. 999. instead of 999.0)

The results of calculations also take either `int` or `float` values. This will depend on the type of numbers used in the calculation and the mathematical operations used:
```
In [12]: type(4.0+2.0)
Out[12]: float

In [12]: type(4+2)
Out[12]: int

In [12]: type(4.0+2)
Out[12]: float

In [13]: type(4*2)
Out[13]: int

In [14]: type(4/2)
Out[14]: float
```
Note here that:
- combinations involving both `int` and `float` types produce a `float` result.
- _addition_ / _subtraction_ / _multiplication_ using `int` values only, produce `int` results, but _division_ of an integers produces a `float` result (to avoid rounding issues when a result is not a whole number). 

For the most part Python is designed to automatically convert between `int` and `float` values so we do not have to. However in some cases we will need to explicitly specify the number type, or convert an existing variable to use a specific type:
```
In [1]: a = int(4.1)

In [2]: a
Out[2]: 4

In [3]: b = float(2)

In [3]: b
Out[3]: 2.0

In [4]: c = 5.9

In [5]: d = int(a)

In [6]: d
Out[6]: 5
```
Note that if when a decimal number is converted into an integer the value is always rounded down to the nearest whole number. 

#### Scientific Numbers

We can also use Python to work with scientific numbers (like $2 \times 10^{10}$ and $3.56 \times 10^{-4}$). To do this we use `e` or exponent notation.

```
In [1]: a=2e10

In [2]: a
Out[2]: 20000000000.0

In [3]: b = 3.56e-4

In [3]: b
Out[3]: 0.000356

In [4]: c = 4e100

In [4]: c
Out[4]: 4e+100
```

#### Exercises.

1. In the Python terminal create the following variables:
      - Variable `h1` with a value of `12.2`
      - Variable `h2` with a value of `10.2`
      - Variable `h3` with a value of `13.9`
  
    Now without typing in the numbers (`12.4` and `10.3`) again.
   - Find the value of `h1` _minus_ `h2`.
   - Find the value of `h2` _times_ `h3`.
   - Set up a new variable called total which has a value equal to the sum of  `h1`, `h2`, and `h3`.
   - Find the value of total divided by 3.
   
   What have you calculated? Store the final value into a suitably named variable.


2. An experiment records the mass of the tomatoes grown inside and outside a greenhouse.

   Inside greenhouse:
   4 tomatoes with masses 43g, 29g, 61g, 50g.

   Outside greenhouse:
   5 tomatoes with masses 38g, 42g, 20g, 34g, 72g.

   Use Python to calculate the total mass of tomatoes grown in each condition, and the average weight of the tomatoes. Store the resulting averages into variables and print out your results.

   _Note that Python cannot deal with units when entering numbers. When performing calculations you'll have to keep track of the units yourself, and remember to add them if necessary when displaying a result._

  

