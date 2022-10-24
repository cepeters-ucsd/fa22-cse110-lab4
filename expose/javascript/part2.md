1. 
It should log 3.

i is within the scope of the function and it will stop once it reaches prices.length which is 3.

2. 
It should log 150.

discountedPrice is updated through every loop of the for loop. The last loop is for i = 2, which means it's set to prices[2] * (1 - discount) = 300 * (1 - 0.5) = 150. Because it's a var it's in the function scope so it is accessible.

3. 
It should log 150.

The final price will be updated on the same loop as discountedPrice for the previous question, which means it'll be set to Math.round(150 * 100) / 100. This is just the same, so it'll be 150. It's also in the scope because it's a var, so it's accessible in the full function.

4. 
[50, 100, 150]

The loop just finds the discounted prices rounded to the hundredths place. The discount is 50% and the original prices are [100, 200, 300] so these prices are just halved and pushed into discounted which is then returned.

5. 
Error.

Line 12 is outside the block scope of i. Because it's a let variable, it can't be accessed from outside its block scope.

6. 
Error

Line 13 is outside the block scope of discountedPrice, which is also a let variable and thus is unaccessible.

7. 
It should log 150.

finalPrice is declared in the same block scope as Line 14 so it's accessible, and the finalPrice should just be the price of the final discounted price, which is 300 * 0.5 = 150.

8. 
[50, 100, 150]

This is functionally identical to the same question from earlier. i and discountedPrice aren't accessible from line 16, but they're not accessed either. discounted, the variable in question, is created in the same scope as line 16. Therefore, the result is the same as question 4 and no errors are produced.

9. 
Error.

i isn't accessible for the same reasons as in question 5 so it will produce an error at line 11.

10. 
It should log 3.

length is set to prices.length which is 3. It's a constant so it doesn't change, and it's in the same block scope as line 12 so no errors are produced.

11. 
[50, 100, 150]

Functionally the only difference between this function and its other iterations is there's no rounding which doesn't matter with these inputs. The const keyword on discounted only means it can't be reassigned, but const arrays can have elements added so that isn't a problem here. This results in the same result as before.

12. 
A. student.nanme
B. student["Grad Year"]
C. student.greeting()
D. student["Favorite Teacher"].name
E. student.courseLoad[0]

13. 
A. "32" (2 is concatenated as a string onto '3')
B. 1 ('3' is treated as an int, 3 - 2 = 1)
C. 3 + null (null is treated as 0, 3 + 0 = 3)
D. '3' + null (null is treated as "null", '3' + "null" = "3null")
E. 4 (true is treated as 1, 1 + 3 = 4)
F. 0 (false & null are both treated as 0, 0 + 0 = 0)
G. "3undefined" (undefined is treated as "undefined", '3' + "undefined" = "3undefined")
H. NaN (subtracting undefined just makes the expression undefined)

14. 
A. true (because they're different types they're treated as numbers and, 2 > 1)
B. false (alphabetically, "2" is not less than "12")
C. true (2 and '2' are treated as numbers where they're equal)
D. false (using strict equality the types are different and the values are thus unequal)
E. false (the two types are treated as numbers, 1 != 2)
F. true (all nonzero booleans are true, true === true)

15. 
=== requires that two values are strictly identical while == is looser and will convert types to make them comparable.

16. 
See file.

17. 
[2,4,6]

The function applies the callback function to each element of the array and adds the result to a new array. The callback function being used doubles the number, so this is done to every element of [1,2,3] resulting in [2,4,6].

18. 
See file.

19. 
1
4
3
2