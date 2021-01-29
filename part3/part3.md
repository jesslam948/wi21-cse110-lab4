Breakpoint at result in calculate sum:
![breakpoint screenshot](p3_breakpoint.jpg)

Watch expressions for num1, num2, and the data type of result:
![watch exp screenshot](p3_watchexp.jpg)

The bug was that num1 and num2 were read as strings so result was a string that consisted of concatenating num1 and num2 together.

I fixed it by converting num1 and num2 to Numbers:
![bug fix](p3_fix.jpg)