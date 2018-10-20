# Pythonistas
![https://media.giphy.com/media/2vnId4IaAjIGZd2EWC/giphy.gif](https://media.giphy.com/media/2vnId4IaAjIGZd2EWC/giphy.gif)

- Officially conquered the fundamentals of Python
- Officially written your own script
- Officially pros at using the terminal

### What could be left to learn???

What if we wanted to take our spooky script and have multiple people input answers before outputting?

- We could just keep copying and pasting our code. 
- But our script would get long and difficult to read quickly.

### FINAL PIECES
![https://media.giphy.com/media/RnX4q6yYDoYCI/giphy.gif](https://media.giphy.com/media/RnX4q6yYDoYCI/giphy.gif)

#### For Loops
**For Loops** are one of the most common ways in python to loop over a sequence. But what does looping mean exactly?

Let's go back to our first_script.py, and find our list of halloween costumes. Add these lines to the script:
```python
for costume in halloween_costumes:
    print(costume)
```
![https://www.oreilly.com/library/view/head-first-python/9781449397524/httpatomoreillycomsourceoreillyimages1368346.png.jpg](https://www.oreilly.com/library/view/head-first-python/9781449397524/httpatomoreillycomsourceoreillyimages1368346.png.jpg)

We can also use For Loops on dictionaries.
```python
for candy in halloween_candies:
    print(candy)
```

#### Conditionals
Earlier we learned about *booleans* (`True or False`). In Python, we can test the truth value of code to decide how we want our code to run.

In our first_script.py, add the following lines:
```python
wizard = 'Harry'
if wizard == 'Harry':
    print('wer a wizard harry')
```
![https://automatetheboringstuff.com/images/000019.jpg](https://automatetheboringstuff.com/images/000019.jpg)

We can also test the equality of two variables in an if statement:
```python
witch = 'Hermione'
if wizard != witch:
    print('well done')
else:
    print('nice try')
```
In this example, we're getting a bit more tricky.
Let's break it down with a simpler example.
```python
test1 = True
test2 = False
print(test1 == test2)
print(test1 != test2)
three = 3
four = 4
print(three < four)
print(four > three)
```

#### Functions
We don't have time to go into depth about functions, but here's a great tutorial [https://www.datacamp.com/community/tutorials/functions-python-tutorial](https://www.datacamp.com/community/tutorials/functions-python-tutorial). Essentially functions are a way to wrap your code into blocks so that way you can call your code when you need it to run.

```python
def get_fundamentals():
    fundamentals = 'Having fun'
    print(fundamentals)
    return fundamentals

get_fundamentals()
```
![https://i0.wp.com/getmoreabout.com/wp-content/uploads/2017/12/1523299_orig-e1514470882262.png?fit=400%2C209&ssl=1](https://i0.wp.com/getmoreabout.com/wp-content/uploads/2017/12/1523299_orig-e1514470882262.png?fit=400%2C209&ssl=1)

Some more advanced examples:
```python
def new_costume(halloween_costumes):
    costumes = halloween_costumes + 'Black Panther'
    return costumes

updated_costumes = new_costume(halloween_costumes)
```

Combining everything together:
```python
def check_costumes(costumes):
    for costume in costumes:
        if costume == 'Black Panther':
            print("That's your costume " + costume)
        else:
            print("Back to the drawing board")
check_costumes(updated_costumes)
```

### Final Thoughts on Python
Open up your terminal and enter the python interpreter, type:
```python
import this
```