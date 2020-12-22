# Risk assesment, and the Random Package

Risk assesment is a key part of software development, relating to the impact it could have on a company if a given part of the application or software where to fail in some way. Un-related is the use of the random package with makes a number of opertations much simpler much like the built-in Math.Random methods of Javascript but much simpler and more versitile. 

# key methods of Random pkg

import the random package with the code below:
`import random`

- `random.randint(lowest, highest)` takes a range and selects a random number from it. 
- `random.choice([]: list of any length) -> value from list` selects a random element from a list
- `random.shuffle([]: list of any lenght) -> mutated list with its input values shuffled` 
- `random.randrange(start, stop[, step])` like randint but allows for setting of a multiple as step. 
  example `random.randrange(0, 100, 5)` would return a number between 0 and 100 that was a multiple of 5

# Risk assessment: what to look at and how to evaluate

The risk associated with an application or piece of software can be summed up in the question: 
"How much time and money will this cost the company if the software fails" everything else is about Identifying:
  - What parts could fail, external/internal
  - what could make them fail
  - how expensive in time/money/customers will it be if it fails
  - how can that expense be minimized
  - how likely is it to fail

after that it's the devil in the details, when developing software, being cognizant of these things and taking pre-cautions to minimize the damage of failure in its design from the beginning, can save everyone stress/time/money. some risks are unavoidable but being aware of them can help form a plan to deal with them and minimize the impact. 


[Return to Main index of Notes](./README.md)

