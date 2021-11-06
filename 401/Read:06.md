# Game of Greed 1
## Random Module :
What is **`Random Module`** :
* The *`Random Module`* provides access to functions that support many operations.

Perhaps the most important thing is that it allows you to generate random numbers.

The Random module contains some very useful functions :
1. **`Randint`** :
   * Return a random intege by using *`random.randint(a, b)`*.

example :

```
import random
print(random.randint(0, 5))

# This will output either 1, 2, 3, 4 or 5.
```

2. **`Random`** :
   * Return the next random floating point number in the range [0.0, 1.0).
   * If you want a larger number, you can multiply it.

example :

```
import random

random.random()
# This will return random float number between 0 and 1

random.random() * 100
# This will output random number between 0 and 100
```

3. **`Choice`** :
   * Return a random element from the non-empty sequence seq. If seq is empty, raises IndexError.

example :

```
import random

random.choice( ['red', 'black', 'green'] ).

# This will return a random element from a list.
```
4. **`Shuffle`** :
   * The shuffle function, shuffles the elements in list in place, so they are in a random order.

example :

```
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)

# This will shuffle the list of x
```

5. **`Randrange`** :
   * Generate a randomly selected element from range(start, stop, step).

example :

```
import random
for i in range(3):
    print random.randrange(0, 101, 5)

# This will generate a random number between 0 and 101 with step of 5.
```
And their is more built-in functions...

![Random Module](https://i1.wp.com/techvidvan.com/tutorials/wp-content/uploads/sites/2/2020/07/Built-in-functions-for-generating-random-numbers-in-python-Copy.jpg?w=644&ssl=1)

## Risk Analysis :
**`Risk Analysis`** is the process of identifying the risks in applications or software that you built and prioritizing them to test.

In any software, using *`risk analysis`* at the beginning of a project highlights the potential *`problem areas`*. After knowing about the *`risk areas`*, it helps the developers and managers to mitigate the *`risks`*.

### Risk Identification :
There are different sets of risks included in the risk identification process :
1. **`Business Risks`** :
   * It is the risk that may come from your company or your customer, not from your project.
2. **`Testing Risks`** :
   * You should be well acquainted with the platform you are working on, along with the software testing tools being used.
3. **`Premature Release Risk`** :
   * a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required.
4. **`Software Risks`** :
   * You should be well versed with the risks associated with the software development process.

### The perspective of Risk Assessment :
There are three perspectives of Risk Assessment:
1. **`Effect`** :
   * To assess risk by Effect.
2. **`Cause`** :
   * To assess risk by Cause is opposite of by Effect.
3. **`Likelihood`** :
   * To assess risk by Likelihood is to say that there is a probability that a requirement won’t be satisfied.

### How actually shall we perform risk analysis?
There are three steps :
1. **`Searching the risk`**
2. **`Analyzing the impact of each individual risk`**
3. **`Measures for the risk identified`**

## Test Coverage :

![Test Coverage](https://files.realpython.com/media/Intermediate-Advanced-PyTest-Features_Watermarked.2d8ace6b71be.jpg)

**`Test coverage`** is a useful tool for finding untested parts of a codebase, it's of little use as a numeric statement of how good your tests are.

Like most aspects of programming, testing requires thoughtfulness. TDD is a very useful, but certainly not sufficient, tool to help you get good tests.

The reason, of course, why people focus on coverage numbers is because they want to know if they are testing enough.

Sufficiency of testing is much more complicated attribute than coverage can answer, you are doing enough testing if the following is true:

* You rarely get bugs that escape into production.
* You are rarely hesitant to change some code for fear it will cause production bugs.