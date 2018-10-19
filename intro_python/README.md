# Introduction to Python and Coding
![https://media.giphy.com/media/9xaryfkdWqqiK6QHKf/giphy.gif](https://media.giphy.com/media/9xaryfkdWqqiK6QHKf/giphy.gif)

### What is Python?
- Programming language, created in 1991 by Guido van Rossum
- Named after Monty Python
- Used for a wide range of programming, from making web apps to data analysis

**Why Python?**
'Python is almost always the second best language for any prblem'

### Open your terminal and check your python version
Type:
```sh
python --version
python3 --version
```

### Let's start coding
In your terminal, type `python3`. This will open the interactive python interpreter where you can write your python code and have the computer execute it. 

1. Type `'Hello world'`
Congrats you've just typed your first bit of python and had the computer execute it 🎉!

Let's breakdown what just happened.
1. You entered data into the interpreter
2. That data had a certain format, in this case variable, and the interpreter automatically showed that data again.

What if we wanted to save our data?

### Variables
We can save our hello world data into a *variable* and keep using it again and again. 

```python
var = 'Hello world'
```
Now try typing `var` again. What happens?

The `var` variable now has 'Hello world' stored inside. Python understands that our variable contains a *string*. You can type any string and store it into a variable.
```python
one = 'one'
two = 'two'
three = 'three'
```

### Data Structures
Strings are just one type of data structure accepted in Python. 

There's also *numbers*. We can take our variables that we assigned before and assign them their actual numbers.
```python
one = 1
two = 2
```
Once we do this though, our strings that were stored in these variables will be erased!

What happens if you try and use a number for your variable?
```python
1 = 1
```
You'll get a syntax error 😅! That's because Python has rules for how to name variables.

- A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume) | 
- A variable name must start with a letter or the underscore character |
- A variable name cannot start with a number |
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ ) |
- Variable names are case-sensitive (age, Age and AGE are three different variables)| 


So our previous example could work if we changed the variable name to:
```python
one_1 = 1
```

Python also has a special name for decimal numbers called *floats*
```python
one = 1.0
```

What if we decided that we wanted to combine variable one and two? We could use a Python *method* for manipulating variables and data.

1. To join variables together use the `+` symbol, this is called concatenation.
```python
one + two
```
You should see `3.0` as your answer. We just added the data in variable one and two together. 
What would happend if we added variables `var` and `three` togther?
```python
var + three
```

2. Other methods that you can use on numbers and floats:
division:
```python
one / two
```

multiplication:
```python
one * two
```

We can also assign a truth value to a variable, called a *boolean*.
```python
var_true = True
var_false = False
```
We can then check if these two variables contain the same truth value.
```python
var_true == var_false
```

In Python `=` is used to assign values to a variable, and `==` is used to check if two variables contain the same value.

### Quick Assignment
```
1. Turn to the people next to you and ask them their first name and age. 
2. Assign those values to variables and input your own first name and age in separate variables. 
3. Try testing if your names or ages are equal.
4. Try joining your names together.
5. Try adding/multiply/dividing your ages.
6. Try joining your ages and names together.
```





SMALL ASSIGNMENT

HOw to store variables: structures
- lists
- dictionaries
- tuples
- sets

How to access variables
append

SMALL ASSIGNMENT

- how to look for help

Group assignment
trick or treat
