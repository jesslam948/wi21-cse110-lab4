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

14.
    a. 32. This is because '3' is a string so it reads the + sign as a concatenation symbol. Thus, it converted 2 to a string and concatenated '3' + '2' = '32'.

    b. 1. This is because the - sign can only mean subtraction, thus '3' is converted from a string to a number and then 3 - 2 = 1 was computed.

    c. 3. This is because 3 is a number so the + sign will be read as addition. Then, null becomes 0 based on javascript number conversion rules. Thus it computes 3 + 0 = 3.

    d. 3null. This is because '3' is a string so it reads the + sign as a concatenation symbol. Then, null becomes 'null' based on string conversion rules. Thus it concatenated '3' + 'null' = '3null'.

    e. 4. This is because, when converted to a number, true = 1. Thus, this computes 1 + 3 = 4.

    f. 0. This is because, when converted to a number, false = 0 and null = 0. Thus, this computes 0 + 0 = 0.

    g. 3undefined. This is because "3" is a string so it reads the + sign as a concatenation symbol. undefined converted to a string is "undefined" so it concatenates "3" + "undefined" = "3undefined".

    h. NaN. This is because the - sign can only mean subtraction, thus "3" is converted from a string to number, so is undefined but undefined = NaN when converted to a number (based on the conversion rules). Thus, it computes 3 - NaN = NaN.

15.
    a. true. When comparing values of different types, JS converts the values to numbers. Thus, it evalutes 2 > 1, which is true.

    b. false. These are the same type so they will compared as strings and will be compared character by character. '2' comes after '1' in lexicographic order so this will evaluate to false.

    c. true. These are different types so they are converted to numbers. Thus it evaluates 2 == 2, which is true.

    d. false. This is a strict equality operator so it sees that 2 and '2' are different types and immediately returns false before attempting to convert.

    e. false. These are different types so they are converted numbers. true is converted to 1 (due to the conversion rules) so it attempts to evaluate 1 == 2, which is false.

    f. true. Boolean(2) gets evaulated to true by the conversion rule (2 is not a value that is intuitively "empty" unlike 0). Thus, this evaulates true === true. The types match and the values match so this is true.

16. == is a regular equality operator while === is a strict equality operator. This means that == will check for equality in value and will convert types to match if they don't. On the otherhand, === cares about the types matching and so if the types don't match it will automatically evaluate to false.

17. 'How are you?' will be printed. This is because 2 == true will be evaluted to false (the reasoning is explained in 15e). Then, it will evaulate the else if (2). Since JS will convert conditional statements to boolean values, it is essentially evaulating Boolean(2). Since Boolean(2) gets evaulated to true by the conversion rule, we enter this else if block. Thus, 'How are you?' is printed.