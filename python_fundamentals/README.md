# Python FUNdamentals

![https://media.giphy.com/media/3oz8xwooUvMqNB1zEs/giphy.gif](https://media.giphy.com/media/3oz8xwooUvMqNB1zEs/giphy.gif)

- Python interpreter is great, but why might we not want to write all our code in the interpreter? What happens every time you quit?

SOLUTION:
1. Open Visual Studio Code
Visual Studio Code is a Code Editor, for writing code. (Think like Microsoft Office for writing...)

2. Open your directory in Visual Studio Code and create a new file

```sh
touch first_script.py
```

You should see this file in Visual Studio Code. We're going to write your first code script! Feel free to enter some of what you wrote for the Trick or Treat exercise, or copy this below:

```python
halloween_costumes = ['pizza', 'zombie', 'deer', 'student']
halloween_candies = {
    'chocolates': ['snickers'],
    'candies': ['skittles']
}
```

1. Now try running the file from your terminal
Make sure you are not in the python interpreter. Type:
```sh
python3 first_script.py
```
What happens?

![https://media.giphy.com/media/3KCOFfdqmptLi/giphy.gif](https://media.giphy.com/media/3KCOFfdqmptLi/giphy.gif)

Because we aren't in the interpreter any more, unless we tell the computer to output a value it won't show us any message (unless there's an error.)

One solution is the **print** method.

In first_script.py, add the line to the bottom of the script:
```python
print(halloween_costumes)
```
This time you should see the list of costumes. 

Now try moving that line to the top of first_script.py and running the script again.

![https://media.giphy.com/media/qQI16x8tgp7nW/giphy.gif](https://media.giphy.com/media/qQI16x8tgp7nW/giphy.gif)

We've hit a problem. Let's break down what happened here. If the print statement was at the bottom of the script it worked, but if it was at the top it didn't. 

That's because the print statement within it's parentheses references the variable `halloween costumes`, but we haven't defined that variable yet.

**Computers read code from top to bottom**


#### So what's the print statement about?

Print is a *built-in Python method*, which means it comes installed with Python and we can use it whenever we are writing Python.

Print is used to literally print out values to the terminal, and it's one of many ways to find out the output of a Python script.

#### Built-In Methods

Print is one of many methods. Let's take a look at a few more.

1. Len()
In first_script.py, move the print statement back to the bottom of the script. Then above the print statement type:
```python
costumes_numbers = len(halloween_costumes)
print('how many halloween costumes do we have?', costumes_numbers)
```
Then try running the code. You should first see our question followed by a number and then the list of halloween costumes. 

The **len** method can return the length of any list, dictionary, or string in Python.

1. Type()
You might also want to know the **type** of your variable, whether it's a data type or a data structure. In first_script.py, add to the bottom of the script:
```python
print(type(halloween_costumes), type(halloween_candines))
```
Once you run the script you should see that we have both a list and a dictionary. With print statements you can add multiple items as long as they are separated by commas, and you can use built-in methods inside the print statement, instead of assigning them to a variable first.

1. Input()
You can also get input from the terminal using the **input** method. In first_script.py, type the following at the bottom of the script:
```python
print('Enter your name:')
name = input()
print('Hello, ' + name)
```
![https://media.giphy.com/media/3o7buirYcmV5nSwIRW/giphy.gif](https://media.giphy.com/media/3o7buirYcmV5nSwIRW/giphy.gif)

*What did we just do?*
First we printed out a prompt. Then we assigned the input method to a variable, and then we printed out hello concatenated with the value of name. 

![https://media.giphy.com/media/vlYBYMFArzuOk/giphy.gif](https://media.giphy.com/media/vlYBYMFArzuOk/giphy.gif)


You've seen built-in methods before for both dictionaries and lists. But they exist for data types too.

#### Built-In Methods for Strings

1. Split()


1. Join()

1. Replace()

1. Upper() and Lower()

1. Reverse()
https://www.w3schools.com/python/python_ref_string.asp


### Third Group Assignment
[SPOOKY STORY SCRIPT](python_exercise_fundamentals.md)

![https://media.giphy.com/media/2vmgb8ZGaeBsuSeo5I/giphy.gif](https://media.giphy.com/media/2vmgb8ZGaeBsuSeo5I/giphy.gif)


