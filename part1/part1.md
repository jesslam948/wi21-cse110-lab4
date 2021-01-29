1. The value of i at the end of the for loop (prices.length) will be printed to the console. There isn't an error because we used 'var', which is not block/loop-local.
2. The last discountedPrice will be printed to the console. Again, because discountedPrice will be visible even after the for loop because it was declared using 'var' instead of 'let'.
3. The last finalPrice will be printed to the console. The finalPrice variable is declared using 'var' and is declared before the for loop so there won't be any errors.
4. The call discountedPrices([100, 200, 300], .5) will return [50, 100, 150]. The for loop goes through each of the prices (100, 200, 300) and then discounts them using the rate (.5 in this case), rounds it, and then adds it to the new discounted array. Since the discount is 50%, the returned array has each of the prices at half-price.

5. This will give an error because i was declared using 'let' and is part of the for-loop block so it's not visible outside of the for-loop block.
6. This will also give an error because discountedPrice was declared using 'let' and was declared inside the for-loop code block so it isn't visible outside of that block.
7. This will print out the last value of finalPrice. This is because finalPrice was declared outside of the for-loop so it will still be visible after the for-loop and will even retain the last value it was assigned within the for-loop.
8. discountPrices([100, 200, 300], .5) will return [50, 100, 150] because the for loop discounts each price (100, 200, 300) by the rate (50%) and puts the discounted prices into a new discounted array that it eventually returns.

9. An error will be thrown because i is declared using 'let' and is part of the for-loop block so it's not visible outside of the for-loop block
10. An error will be thrown because discountedPrice was declared using 'const' and was declared within the for-loop block. Thus, it is not visible outside of the for-loop block.
11. Assuming that errors are not thrown while attempting to re-assign finalPrice within the for-loop, this line should output 0, since it was declared using 'const' and is assumed to never change value.
12. Assuming that errors are not thown while attempting to update the discounted array within the for-loop, this function will return an empty array []. This is because it was declared using 'const' and is assumed that its value won't change.

13. 
a. `student.name`
b. `student['Grad Year']`
c. `student.greeting()`
d. `student['Favorite Teacher'].name`
e. `student.courseLoad[1]` (I'm assuming we're asking for the index 1 and not the first element which would be at index 0, otherwise we would just replace the 1 with a 0)