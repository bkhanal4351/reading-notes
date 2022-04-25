## How to use Random Module
-  The random module provides access to functions that support many operations. Perhaps the most important thing is that it allows you to generate random numbers.

When to use it?
- We want the computer to pick a random number in a given range Pick a random element from a list, pick a random card from a deck, flip a coin etc. When making your password database more secure or powering a random page feature of your website.

Random functions

1. Randint
- If we wanted a random integer, we can use the randint function Randint accepts two parameters: a lowest and a highest number. Generate integers between 1,5. The first value should be less than the second.

    `import random
    print random.randint(0, 5)`
This will output either 1, 2, 3, 4 or 5.

Random
If you want a larger number, you can multiply it.

For example, a random number between 0 and 100:

`import random
random.random() * 100`
Choice
Generate a random value from the sequence sequence.

random.choice( ['red', 'black', 'green'] ).
The choice function can often be used for choosing a random element from a list.

`import random
myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
random.choice(myList)`
Shuffle
The shuffle function, shuffles the elements in list in place, so they are in a random order.

random.shuffle(list) Example taken from this post on Stackoverflow

`from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)`
Output:
# print x  gives  [[9], [2], [7], [0], [4], [5], [3], [1], [8], [6]]
# of course your results will vary
Randrange
Generate a randomly selected element from range(start, stop, step)

`random.randrange(start, stop[, step])
import random
for i in range(3):
    print random.randrange(0, 101, 5)`


## What is Risk Analysis
- In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks. When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.

Risk Identification

1. Business Riska
2. testing Risks
3. Premature release Risk
4. Software Risks

How to perform Risk Analysis?
There are three steps:

1. Searching the risk

2. Analyzing the impact of each individual risk

3. Measures for the risk identified

Notes taken from (https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
(https://www.edureka.co/blog/risk-analysis-in-software-testing/)






