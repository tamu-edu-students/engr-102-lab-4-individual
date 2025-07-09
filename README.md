# ENGR 102 Lab Topic 4 (individual)

## Activities
This lab consists of three individual activities, and an optional bonus activity. Please submit the following files to Gradescope. Check out the [Frequently Asked Questions](#frequently-asked-questions) below. **Please include the individual header in your ~.py files.**

1. [Largest Number](#largest-number)
2. [How Many Gadgets](#how-many-gadgets)
3. [Calculate Roots](#calculate-roots)

## Largest Number
Using conditional statements (i.e. statements like `if-elif-else`) write a program named `largest_number.py` that takes as input from the user three (3) numbers from the keyboard and prints the value of the largest number. Your code should output in the format shown below.

Example output (using inputs `1`, `2`, `3`):
```
Enter number 1: 1
Enter number 2: 2
Enter number 3: 3
The largest number is 3.0
```


## How Many Gadgets
Assume a machine during its initial testing phase produces 10 gadgets a day. After 10 days of testing (starting on day 11), it begins to ramp up, producing 1 more gadget per day (11 gadgets on day 11, 12 on day 12, etc). On day 50 it reaches full speed, where it continues to run until on day 101 it stops producing gadgets. Write a program named `how_many_gadgets.py` that reads in a day (as a number) from the keyboard and reports the total number of gadgets produced from the initial testing phase up to and including the day entered. For example, entering 3 would report 30 gadgets.

Your code should also...
- Check for inappropriate day numbers and message the user accordingly
- Echo the input in the output when you report the number of gadgets
- Use the output format shown below

**Note**: Do **NOT** use a loop. Part of the challenge in this program is for YOU to work out the model for how to compute gadgets produced in total, given the above information. **Hint**: Solve this problem by hand on paper first, then translate your solution to Python. **A graph or diagram is extremely helpful.** This approach is much easier than debugging some lousy Python code written before you understand the problem.

Example output (using input `3`):
```
Please enter a positive value for day: 3
The sum total number of gadgets produced on day 3 is 30
```

Example output (using input `-1`):
```
Please enter a positive value for day: -1
You entered an invalid number!
```


## Calculate Roots

## Frequently Asked Questions
1. **Activity 2 (how many gadgets) I want to use a loop. Can I use a loop?** No! You don't need to use a loop. That's why you can do this problem even though we haven't learned about loops. A loop is actually *inefficient* for solving this problem. **But how do I solve it without a loop?** Short answer: Write a mathematical equation for the number of gadgets produced for any given day. Long answer: Draw a graph with the gadgets/day on the y axis and days on the x axis. You have 3 parts to this graph: the square part for the first 10 days, the trapezoid part for days 11 to 50, and the rectangle part for days 51 to 100. How many gadgets have you made at the end of day 3? That's 10 gadgets/day times 3 days, so 30. Oh wait, that's the area under the curve from day 1 to day 3. Hmm... so if I want to know how many gadgets have been produced at the end of day 15, I can take the area under the curve for the first part (`10 * 10 = 100`) and add the area under the curve for days 11 through 15. The area of a trapezoid is $$\frac{1}{2}(b_1 + b_2)h$$. Think of it as a trapezoid on its side...

2. **Activity 2 (how many gadgets) are any gadgets produced on day 101?** Nope, day 100 is the last day it produces gadgets.

3. **Activity 3 (calculate roots) I have no idea what I'm doing. Help?** When you have a quadratic equation (`A != 0`) you can calculate the root(s) with the quadratic formula. Do you remember the name of the part under the square root? That's right, it's the discriminant. You have 3 possibilities for this number. It can be positive (2 real roots), zero (2 real identical roots), or negative (2 complex roots). You may want to use an `if-elif-else` statement to account for these possibilities.

4. **Activity 3 (calculate roots) how do I display a complex number?** You don't actually have to bother with python's complex numbers. Instead, use string formatting to display it correctly. Calculate the real `-b/(2a)` and imaginary `sqrt(|b^2-4ac|)/(2a)` parts of the number separately. Then use string concatenation to put the pieces together with an `i` attached to the imaginary part.

Have a question you don't see here? Email your instructor!

Based upon Dr. Keyser’s Original<br/>
Revised Summer 2025 SNR
