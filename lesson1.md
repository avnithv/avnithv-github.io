# Hello World
In your repl, add a new file and call it helloworld.py. In that file, write the code below:

`print('Hello, world!')`

Make sure that your code is exactly the same as the one shown above. If it isn't, the program will not run properly. This is a basic python program. Now run the program using the instructions in the introduction. The console on the right should show this:

`Hello, world!`

This happens because the `print()` function outputs the string `'Hello, world!'` onto the console. We will learn about basic datatypes, operations, control stuctures, and functions in this lesson.

# Basic Datatypes
There are different types of data that can be stored in variables. The basic ones are:
- String: Data which is a series of characters. It is defined using quotation marks such as `''` or `""`.
- Int - Data which is an integer, and can be negative. It is automatically defined whenever you assign an integer to a variable.
- Float - Data which is a number, and may or may not be an integer, but will alway have a decimal point. It is automatically defined whenever you assign a number with a decimal point to a variable.
- Boolean - Data which is either True or False. It is automatically defined whenever you assign a variable either `True` or `False`.

To assign a datatype to a variable, you just use the equal sign and put the variable on the left side and the datatype on the right side. Variables must not have spaces or start with a number. Some examples of assigning data to variables:
```
month = 'November'
year = 2020
pi = 3.14
MyBirthdayIsInAugust = False
```

Strings, ints, and floats can be converted into other datatypes, if it is possible. For example, you can convert the int `8` into a string of the character `‘8’`, but cannot convert `‘abcdef’`, a string, into an int. You can convert data types to strings, ints, and floats by using the `str()`, `int()`, and `float()` functions respectively. For example:
```
number_8 = 8
string_8 = str(number_8)
float_8 = float(string_8)
```
