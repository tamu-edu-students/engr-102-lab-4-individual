# ENGR 102 Lab Topic 4 (individual)

## Activities

1. [Largest Number](#largest-number)
2. [How Many Gadgets](#how-many-gadgets)
3. [Calculate Roots](#calculate-roots)

## Largest Number

## How Many Gadgets

## Calculate Roots

## Frequently Asked Questions
1. **Activity 2 (how many gadgets) I want to use a loop. Can I use a loop?** No! You don't need to use a loop. That's why you can do this problem even though we haven't learned about loops. A loop is actually *inefficient* for solving this problem. **But how do I solve it without a loop?** Short answer: Write a mathematical equation for the number of gadgets produced for any given day. Long answer: Draw a graph with the gadgets/day on the y axis and days on the x axis. You have 3 parts to this graph: the square part for the first 10 days, the trapezoid part for days 11 to 50, and the rectangle part for days 51 to 100. How many gadgets have you made at the end of day 3? That's 10 gadgets/day times 3 days, so 30. Oh wait, that's the area under the curve from day 1 to day 3. Hmm... so if I want to know how many gadgets have been produced at the end of day 15, I can take the area under the curve for the first part (`10 * 10 = 100`) and add the area under the curve for days 11 through 15. The area of a trapezoid is $$\frac{1}{2}(b_1 + b_2)h$$. Think of it as a trapezoid on its side...

2. **Activity 2 (how many gadgets) are any gadgets produced on day 101?** Nope, day 100 is the last day it produces gadgets.

3. **Activity 3 (calculate roots) I have no idea what I'm doing. Help?** When you have a quadratic equation (`A != 0`) you can calculate the root(s) with the quadratic formula. Do you remember the name of the part under the square root? That's right, it's the discriminant. You have 3 possibilities for this number. It can be positive (2 real roots), zero (2 real identical roots), or negative (2 complex roots). You may want to use an `if-elif-else` statement to account for these possibilities.

4. **Activity 3 (calculate roots) how do I display a complex number?** You don't actually have to bother with python's complex numbers. Instead, use string formatting to display it correctly. Calculate the real `-b/(2a)` and imaginary `sqrt(|b^2-4ac|)/(2a)` parts of the number separately. Then use string concatenation to put the pieces together with an `i` attached to the imaginary part.

Have a question you don't see here? Email your instructor!

Based upon Dr. Keyser’s Original<br/>
Revised Summer 2025 SNR
