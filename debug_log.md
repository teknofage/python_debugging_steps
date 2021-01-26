# Debug Log

**Explain how you used the the techniques covered (Trace Forward, Trace Backward, Divide & Conquer) to uncover the bugs in each exercise. Be specific!**

In your explanations, you may want to answer:

- What is the expected vs. actual output?
- If there is a stack trace, what useful information does it contain?
- Which technique did you use, on which line numbers?
- What assumptions did you have about each line of code, and which ones were proven to be wrong?

_Example: I noticed that the program should show pizza orders once a new order is made, and that it wasn't showing any. So, I used the trace forward technique starting on line 13. I discovered the bug on line 27 was caused by a typo of 'pzza' instead of 'pizza'._

_Then I noticed another bug ..._

## Exercise 1

- What is the expected vs. actual output?
[[Actual Output 1: TypeError: 'topping' is an invalid keyword argument for PizzaTopping

Actual Output 2: werkzeug.routing.BuildError: Could not build url for endpoint '/'. Did you mean 'fulfill_order' instead?

Expected Output: Order submitted and returned to home page on click.]]

- If there is a stack trace, what useful information does it contain?
1. File "/Users/Funkhauser/dev/Courses/SPD-2.3/SPD-2.3-Debugging-Techniques-Lab/exercise-1/app.py", line 79, in pizza_order_submit
Open an interactive python shell in this framepizza.toppings.append(PizzaTopping(topping=topping_str))

2. File "/Users/Funkhauser/dev/Courses/SPD-2.3/SPD-2.3-Debugging-Techniques-Lab/exercise-1/app.py", line 84, in pizza_order_submit
Open an interactive python shell in this framereturn redirect(url_for('/'))
]]

- Which technique did you use, on which line numbers?
1. Trace Backwards from line 79, until I found the correct variable name that relates to the DB: topping_type on line 42.

2. Trace Backwards from line 84, until I found the name of the home page function that should replace the '/' route in the redirect.



- What assumptions did you have about each line of code, and which ones were proven to be wrong?
[[I had to assume that each variable relating to toppings could have been misnamed or mislabeled.]]

## Exercise 2

- What is the expected vs. actual output?
[[Your answer goes here!]]

- If there is a stack trace, what useful information does it contain?
[[Your answer goes here!]]

- Which technique did you use, on which line numbers?
[[Your answer goes here!]]

- What assumptions did you have about each line of code, and which ones were proven to be wrong?
[[Your answer goes here!]]

## Exercise 3

- What is the expected vs. actual output?
[[Your answer goes here!]]

- If there is a stack trace, what useful information does it contain?
[[Your answer goes here!]]

- Which technique did you use, on which line numbers?
[[Your answer goes here!]]

- What assumptions did you have about each line of code, and which ones were proven to be wrong?
[[Your answer goes here!]]
