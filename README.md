# Leap Year Challenge

## The Goal

We're going to write a program which will tell us whether or not a given year is a leap year. We'll do three versions of it - each one a little more complicated than the last.

To do this, you may want to use a <a href="https://www.accuracyproject.org/leapyears.html">list of which years are leap years</a>.

## The Lab

We'll separate our concerns by _defining_ our functions in the leap.py file, and _calling_ our functions in the testleap.py file.

Open up those two files, complete the challenges listed, and run your tests with the command `python testleap.py`

## Skills you may need

### Comparison operators

You've already used some comparison operators (greater than, less than, and equals) in our last lab. You may want <a href="https://www.tutorialspoint.com/python/python_basic_operators.htm">a few more</a>.

### Modulus and remainders

In Python, you can easily find the remainder of a division expression. For example, 10 divided by three is three, with a remainder of 1.

To jump straight to a remainder, you can write the expression using the modulus (%) operator.

` 10 % 3 `

This expression will return the remainder - it will evaluate to 1.

##### Modulus uses

The modulus is used more often in computer programming than you might use remainders in your everyday life. One of the most common uses of a modulus is to check if a number is even or odd. Since `10 % 2` evaluates to 0 (there's no remainder), you know it's even. Since `9 % 2` evaluates to 1 (since nine divided by 2 is 4 with a remainder of 1), a lot of programs will check whether an integer is even or odd using code that looks like this.

```python
if some_number % 2 == 0:
    print("This number is even!")
elif some_number % 2 == 1:
    print("This number is odd!")
```

### Boolean return data

The first function we will define will tell us whether a given year is a leap year. This is a really useful function, because there are only two possible answers. These two possible answers are called booleans which hold the value of either True or False.

```python
def is_leap_year(year)
    if # some code to check and see if the year is a leap year:
        return True
    else:
        return False
```

Notice that the words True and False are not in quotes. If we wrote them that way, they'd be strings. We want boolean values, not strings, so we're not using quotes. Also, notice that in Python they must start with capital letters.

### for-in loops

Loops, as you might imagine, let you repeat something on a scale that would be exhausting to do manually. We will cover many types later in the course, but here's a great first loop to run.

Let's write code that prints every number from 1-100:

```python
for x in range(1, 101):
  print(x)
```

In this loop, the letter x represents each number, one at a time. Generally it's called a local variable, and more specifically it will sometimes be referred to as an iterator.

The plain-words translation of that loop might read like this: `for every number from 1 up to (but not including) 101, print that number.`

This can become even cooler when we manipulate the code block inside the loop:

```python
for x in range(1, 101):
  print(x * 2)
```

The plain-words translation of that loop might read like this: `for every number from 1 up to (but not including) 101, print double the value of that number.`
