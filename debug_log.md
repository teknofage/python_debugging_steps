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
TypeError: 'topping' is an invalid keyword argument for PizzaTopping
[[Your answer goes here!]]
changet he html and app.py key values
## Exercise 2
line 53, in results
    'city': result_json['name'],
KeyError: 'name'
[[Your answer goes here!]]
Had to change api params to correct names.
## Exercise 3
File "main.py", line 8, in <module>
    merge_sort(list_of_nums)
  line 38, in merge_sort
    arr[k] = right_side[j]
IndexError: list assignment index out of range
line 53, in binary_search
    if arr[mid] < elem: 
TypeError: list indices must be integers or slices, not float
[[Your answer goes here!]]
interger division was neede isntead of floating point division