## Food Rating

In a five-star restaurant review system (⭐️⭐️⭐️⭐️⭐️), the star represent different levels of satisfaction. But what does each star rating actually mean?

Start by creating a `rating` variable and assign it a decimal number between 0 and 5.

Next, make a rating system with and `if` / `elif` / `else`:

- `rating` greater than 4.5, print `'Perfection'`
- `rating` greater than 4, print `'Excellent'`
- `rating` greater than 3, print `'Good'`
- `rating` greater than 2, print `'Fair'`
- Otherwise, print `'Poor'`

```py
rating = float(input("Restaurant review: "))

if rating > 4.5:
  print('Perfection')
elif rating > 4:
  print('Excellent')
elif rating > 3:
  print('Good')
elif rating > 2:
  print('Fair')
else:
  print('Poor')

```

## High School Grades

U.S high schools typically last for four years, from freshman year to senior year

First, ask the user to enter their grade as an integer

Create a four-year high school grade system using an `if`/`elif`/`else` statement:

- `grade` is 9, print `Freshman`
- `grade` is 10, print `Sophomore`
- `grade` is 11, print `Junior`
- `grade` is 12, print `Senior`
- Everythign else is `TBD`

```py
grade = int(input("What's your grade? "))

if grade == 9:
  print('Freshman')
elif grade == 10:
  print('Sophomore')
elif grade == 11:
  print('Junior')
elif grade == 12:
  print('Senior')
else:
  print('TBD')

```

## Snapple Facts

**Snapple** is a famous tea brand born in Brooklyn, NY. Every bottle cap hides a quirky, fun fact

Use the random module to generate a number between 1 and 6

Then, use an if/elif/else statement to print out one of these **Snapple* facts

```py
import random

snapple = random.randint(1, 6)

if snapple == 1:
  print('Flamingos turn pink by eating shrimp.')
elif snapple == 2:
  print('Honey never goes bad.')
elif snapple == 3:
  print('Shrimp can only swim backwards.')
elif snapple == 4:
  print('A taste bud\'s life is about 10 days.')
elif snapple == 5:
  print('You can\'t sneeze while sleeping.')
else:
   print('Tiny pocket in jeans was for watches.')
```

## Seasons of the year

Ah, the four seasons of the year - winter, spring, summer of fall; all you have to do is call

Ask the user the month number using `input`

Check for the four seasons using an `if`/`elif`/`else`

- `month` is 1, 2, 3, print `'Winter 🌨️'`
- `month` is 4, 5, 6, print `'Spring 🌱'`
- `month` is 7, 8, 9, print `'Summer 🌻'`
- `month` is 10, 11, 12, print `'Autumn 🍂'`
- Everything else is `Invalid`

## Planet Wights

The year is 2199... Humanity is now an interplanetary epecies, freely traveling across the solar system!

Create a weight conversion program that:

- Asks the user for their Earth weight (as a **float**)
- Asks the user for planet number (as an **int**)

Then, use an `if`/`elif`/`else` statement to calculate the user's weight on the destination planet.

To calculate the user's weight:
*destination weight=Earth weight × relative gravity*

```py
weight = float(input("Earh weight: "))
planetNum = int(input("User for a planet number: "))


if planetNum == 1:
  rg = 0.38
  destinationWeight = weight * rg
  print('Your weight in Mercury is: ', destinationWeight)

elif planetNum == 2:
  rg = 0.91
  destinationWeight = weight * rg
  print('Your weight in Venus is: ', destinationWeight)

elif planetNum == 3:
  rg = 0.38
  destinationWeight = weight * rg
  print('Your weight in Mars is: ', destinationWeight)

elif planetNum == 4:
  rg = 2.53
  destinationWeight = weight * rg
  print('Your weight in Jupiter is: ', destinationWeight)

elif planetNum == 5:
  rg = 1.07
  destinationWeight = weight * rg
  print('Your weight in Saturn is: ', destinationWeight)

elif planetNum == 6:
  rg = 0.89
  destinationWeight = weight * rg
  print('Your weight in Uranus is: ', destinationWeight)

elif planetNum == 7:
  rg = 1.14
  destinationWeight = weight * rg
  print('Your weight in Neptune is: ', destinationWeight)

else:
  print('Invalid number')
```
