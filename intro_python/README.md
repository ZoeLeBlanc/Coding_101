# Introduction to Python and Coding
![https://media.giphy.com/media/9xaryfkdWqqiK6QHKf/giphy.gif](https://media.giphy.com/media/9xaryfkdWqqiK6QHKf/giphy.gif)

### What is Python?
- Programming language, created in 1991 by Guido van Rossum
- Named after Monty Python
- Used for a wide range of programming, from making web apps to data analysis

**Why Python?**

'Python is almost always the second best language for any problem'

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

### Data Types
Strings are just one of many data types accepted in Python. 

There's also numbers, called *integers*. We can take our variables that we assigned before and assign them their actual numbers.
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

Python also has a special name for decimal numbers, called *floats*.
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

2. Other methods that you can use on integers and floats:
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

### Data Structures
Typing the information of two or three students is doable, but what if we wanted to do everyone in the workshop? Typing a new variable each time to assign their value is really tedious!

That's where data structures come in! In Python, we can store data types in various data structures that are optimized for different problems.

#### Lists
If we wanted to take the first names of everyone in the workshop, we could store them in a data structure called a *list*.
```python
names = ['Hermione', 'Harry', 'Ron']
```
A list is an unordered, comma-separated collection of any values. So we can store any combination of values in our list.
```python
names = ['Hermione', 'Harry', 'Ron', 42]
```
We can also store a list inside of another list.
```python
names = ['Hermione', 'Harry', 'Ron', 42, ['UVA', 'W&L']]
```
What if you want to just print out 'Hermione' from the list? We can do that by *indexing* the list. 
```python3
names[0]
```
Each list in Python is a sequence, and we can access the position of an item in that sequence through indexing. **In Python, indexes always start at zero!**

We can use indexing in all sorts of ways.
1. We can take the final item by using negative one, which tells python to get the last item from the list
```python3
names[-1]
```
1. We can take a range of items by using a colon to specify when we want to start and stop
```python3
names[1:3]
```
1. If we try to index longer than the list, we'll get an error that tells us we're out of range of the list
```python3
names[8]
```

Now what if we wanted to add a Hogwarts classes to our list? We could create a new list that contained the classes and then use concatenation to join them.
```python3
classes = ['Defense Against The Dark Arts', 'Potions']
names + classes
```
We can see in the interpreter that we now have a list containing both lists, but what happens if you type names again?
![https://media.giphy.com/media/80TEu4wOBdPLG/giphy.gif](https://media.giphy.com/media/80TEu4wOBdPLG/giphy.gif)

Remember to store values, we need to *assign* them to variables.
```python3
classes = ['Defense Against The Dark Arts', 'Potions']
new_list =names + classes
```

We can also add items and remove them from the list. Let's take a look at some of these methods [https://www.w3schools.com/python/python_ref_list.asp](https://www.w3schools.com/python/python_ref_list.asp). You can read more about them in the python documentation [https://docs.python.org/3/tutorial/datastructures.html](https://docs.python.org/3/tutorial/datastructures.html)

#### Quick Assignment
```
Try out the methods in the documentation for manipulating lists
1. Find a way to add 'Dumbledore' to the end of our `new_list` (hint: there's multiple ways to do this)
2. Try reversing and sorting our `new_list`, what happens? Try doing the same on `classes`
```

Lists are great. But what if we wanted to store information not just in a sequence, but in a way that let's us keep certain values together?

#### Dictionaries
We can use a *dictionary*, which is a collection of key/value pairs to store this information. Keys and values are always separated by a colon.

```python3
witch = { 'name': 'Hermione', 'age': 18}
```
To access our values in dictionaries, we don't use indexing. Instead, we use the keys of dictionary. Keys are always the values that come before the colon.
```python3
witch['name']
```
We write the key inside of brackets and quotations, called *bracket notation*. 

What happens if we add another name to the dictionary?
```python
witch = { 'name': 'Hermione', 'age': 18, 'name': 'Harry'}
```
Where's hermione??

![https://media.giphy.com/media/OUwzqE4ZOk5Bm/giphy.gif](https://media.giphy.com/media/OUwzqE4ZOk5Bm/giphy.gif)

Hermione was overwritten in our dictionary because our new value shared the same key. In a dictionary, keys must be unique!

Just like lists though we can store a dictionary inside of a dictionary
```python
hogwarts = {
    'student_1': {
        'name':'Hermione'
    },
    'student_2': {
        'name':'Harry',
        'age':19
    },
}
```
Now we can get Hermione's name if we type `hogwarts['student_1']['name']`. What's happening here is that we're using the keys to find our value that's nested inside a dictionary within a dictionary.

We can add Hermione's age by using a similar notation:
```python3
hogwarts['student_1']['age'] = 18
```
Just like lists there are many ways to manipulate dictionaries
[https://www.w3schools.com/python/python_ref_dictionary.asp](https://www.w3schools.com/python/python_ref_dictionary.asp)

#### Quick Assignment
```
Try out the methods for manipulating dictionaries.
1. Remove Harry's age from the `student_2` dictionary
2. Get all the keys for the `hogwarts` dictionary
3. Get all the values for the `student_1` dictionary
```

[https://media.giphy.com/media/F6MFG8PHtQ2qs/giphy.gif](https://media.giphy.com/media/F6MFG8PHtQ2qs/giphy.gif)

You can also get even crazier and store lists in dictionaries:
```python
hogwarts = {
    'student_1': {
        'name':'Hermione',
        'classes':['Defense Against The Dark Arts', 'Potions']
    },
    'student_2': {
        'name':'Harry',
        'age':19
    },
}
```
Notice that the list is a value of a key, in this case `classes`. You can only insert a list into a dictionary as a value.

You can also put dictionaries inside of lists:
```python
students_hogwarts = [
    {
        'name':'Hermione',
        'classes':['Defense Against The Dark Arts', 'Potions']
    },{
        'name':'Harry',
        'age':19
    }
]
```
Notice that we now don't have keys for our top-most dictionaries. In lists, items don't have keys so each of your dictionaries is without an explicit key.

Python defaults to indexing each dictionary with numbers, just like in our list of strings. So to get the first value, you would type:
```python
students_hogwarts[0]
```
### Any questions?

### Second Group Exercise
[TRICK OR TREAT PYTHON](python_exercise.md)

![https://media.giphy.com/media/uoPf8Z0vGcTOE/giphy.gif](https://media.giphy.com/media/uoPf8Z0vGcTOE/giphy.gif)