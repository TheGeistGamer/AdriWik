# Example Loops

## Are we there yet?

First, ask the user "Are we there yet?" using the `input()` function and store it is an answer variable.

Then, create a `while` loop that asks the user "Are we there yet?" again. Keep asking them this over andd over until they respond with "Yes"

```py
# Primera pregunta
answer = input("Are we there yet? ")

# Repetir mientras la respuesta no sea "Yes"
while answer != "Yes":
    answer = input("Are we there yet? ")
```

## New Year Countdown

Ring in the New Year! A new Year's Eve party doesn't feel complete without a countdown form 10 to 1

Use a `for` loop that counts down by using the "step" value in `range()`

Inside the loop, print the numbers from 10 to 1, each on tis own line.

When the loop finishes the countdown, print this exact string `Happy New Year! 🥳`

```py
for i in range(10, 0, -1):
  print(i)

print('Happy New Year! 🥳')
```

## Snake Eyes

Suppose we have a pair of dice. 🎲 🎲

In dice games, "snake eyes" means rolling two 1s.
Why is it called that? Because two small dots look like a pair of snake eyes

It's the lowest possible roll and is seen as bad luck.

Lets keep rerolling two dice until we get snake eyes

First, use the `random` module to "roll" the two dice.

Each die (named die1 and die2) should have an integer value form 1 to 6

Store the sum of the two random values in vaiable named `total`

Using a `while` loop, check if `total` is 2. If isn't print the string `Nope` and keep "rerolling" the dice.

Let the loop run until the `total` is 2 then print `snake eyes`

```py
import random

total = 0

while total != 2:
  die1 = random.randint(1, 6)
  die2 = random.randint(1, 6)

  total = die1 + die2

  if total == 2:
    print('Snake eyes!')
  else:
    print('Nope')

```

## Asterisks

Use only a `for` loop with `range()` and `print()` to display a staircase of asterisks

Be sure you start with a single `*` in the first line and end with 24 total asteriks on the last line.

Each should have a space after it so they're spread out.

```py
for i in range(1, 25):
  render = '* ' * i
  print(render)
```

## Sum of Squares

A number is "squared" when it is either multiplied by itself or taken to the second power

First, ask the user for an integer with `int(input())` and store it in a `number` variable.
Then define a `total` with an initial value of 0.

You can pass a string propt to `int(input())`

Next, use a `for` loop and `range()` function to calculate the `total` of the squares of all integers from 1 to that `number`

Last, pritn the output as an integer value

If `number` is 5, the `total` should be 55 because:
