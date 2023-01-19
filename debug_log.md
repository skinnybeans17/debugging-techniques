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

First, the problem I noticed with the main home and base pages, is that the style sheets weren't showing. That's because it wasn't linked correctly. I changed it from '/static/style.css' to '../static/style.css', and now the styles show up. This is the technique of Trace Backward. Next, I noticed that in 'app.py', the 'toppings_list' wasn't defined. I then noticed that 'topping_str' had something to do with this. This is also a Trace Backward technique. The server also wasn't starting up, so I added port=8000. This was a trace forward technique. Once I got that running, I saw an internal server coming up. I fixed that by changing some of the variables, and the orders are saving now! Also a trace forward technique.

## Exercise 2

I saw that send_file wasn't defined, so I removed that. I also saw a typo where it was http instead of https, so I fixed that. Other than that, nothing much else needed to be changed. This was also a Trace Backward technique. I got the app running the same way for the first exercise. I fixed the internal server error by changing city to q to better match up the code, and same with temperature to temp. Trace Forward technique this is.

## Exercise 3

For this one, the list index was out of range on line 37 in the utils.py file. I fixed that by changing the i to j, ad also adding in 'k += 1' for both letters. Then on line 53, it said it needed to be slices or integers for lists, and not floats. So I fixed that by adding mid for both of the high and low elem problems. Finally, I added a second slash for the mid divided by two, and the problems are solved! Once again a Trace Backward technique.
