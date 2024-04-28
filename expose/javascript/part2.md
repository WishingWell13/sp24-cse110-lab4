### Part 2

1) Line 12 will print the value of `prices.length` (which is 3), because it occurs after the end of the for loop and the end condition is `prices.length`. Since the variable is a `var`, it has a function scope, so line 12 is still a valid place to call `i` (both line 6 and 12 are in the same function).

2) Line 13 will print the value of `150`, because it is overwritten until the last value of the array multipled by the discount (300 * (1-0.5)). Since the variable is a `var`, it has a function scope, so line 13 is still a valid place to call `discountedPrice` (both line 6 and 12 are in the same function).

3) Line 14 will print the value of `150`, because it is overwritten until the last iteration of the loop. Since the variable is a `var`, it has a function scope, so line 14 is still a valid place to call `discountedPrice` (both line 6 and 12 are in the same function).

4) This function will return `[50, 200, 300]`. The function goes through each value and multiplies it by `1-discountedPrice`. In this case, `discountedPrice` is 0.5, so we multiply by 0.5.

5) Line 12 will error. `i` is a block scope variable. The block `i` is defined in is the `for` loop. Line 12 is outside the for loop.

6) Line 13 will error. `discounted` is a block scope variable. The block `discounted` is defined in is the `for` loop. Line 13 is outside the for loop.

7) Line 14 will not cause an error because `finalPrice` is defined outside the for loop. Therefore, it is accessable in the entire function, because `let` means the variable is block scoped. `finalPrice` should be 150 at the console.log statement.

8) This function will return `[50, 200, 300]`. The function goes through each value and multiplies it by `1-discountedPrice`. In this case, `discountedPrice` is 0.5, so we multiply by 0.5.

9) Line 12 will error. `i` is a block scope variable. The block `i` is defined in is the `for` loop. Line 12 is outside the for loop.

10) The program will print `3` representing the length of the array `[100, 200, 300]` passed into the function. The program did not edit `length` after it was declared, so it will not cause errors. `const` means that `length` is block scoped. Both line 4 and 12 are in the same block.

11) This function will return `[50, 200, 300]`. The function goes through each value and multiplies it by `1-discountedPrice`. In this case, `discountedPrice` is 0.5, so we multiply by 0.5. We call functions on `discounted` and do not reassign it, so it will not throw an error.

#### Data Types

12:
a) `student.name`
b) `student["Grad Year"]`
c) `student.greeting()`
d) `student["Favorite Teacher"].name`
e) `student.courseLoad[0]`

#### Basic Operators and Type Conversion

13:
a) '3'+ 2 = '32'. The integer `2` was converted to a string. Then, the `+` symbol was treated as a concatination operator.
b) '3' - 2 = 1. The string `3` was converted to an integer. `3-2 = 1`
c) 3 + null = 3. `null` is converted to 0. Then, `3+0 = 0`
d) '3' + null = '3null'. The `+` is treated as string concatination, since it is after a string. Therefore, `null` is converted to `'null'`, and is appended after the string `'3'`
e) true + 3 = 4. `true` is converted to `1 ` for numeric addition. `1+3 = 4`
f) false + null = 0. `false` and `null` are both converted to 0. `0+0=0`
g) '3' + undefined = '3undefined'. The `+` is treated as string concatination, since it is after a string. `undefined` is converted to a string `'undefined'` and is appended after the string `'3'`.
h) '3' - undefined = NaN. `undefined` is converted to `NaN`. Since one of the terms of the subtraction is `NaN`, the result is `NaN`.

14:
a) '2' > 1 = true, string `'2'` becomes the number `2`, and `2>1 = true`
b) '2' < '12' = false. Since these are strings, we compare character by character. The string `'2'` is greater than the string `'1'`, so the expression is false.
c) 2=='2' = true. When comparing values of different types, javascript converts all values to numbers. Therefore, the right hand side of the expression is converted to the number `2`. `2==2` is a correct expression.
d) 2==='2' = false. `===` checks that both sides are the same type. The left hand side is a number, while the right hand side is a string, so the expression is false.
e) true == 2 = false. When comparing values of different types, javascript converts all values to numbers. `true` is converted to be `1`. 1 does not equal 2, so the expression is false
f) true === Boolean(2) = true. `Boolean(2)` converts `2` to `true` because it is non-zero. `true === true` is a true statment. 

15: The `==` operator uses type conversion before comparing the variables. Therefore, items of different types can be equal. The `===` operator does not use type conversion before comparing the variables. Therefore, items of different types cannot be equal under the `===` operator.


17) The result would be `[2,4,6]`. We pass in `doSomething` as the callback function. In `modifyArray`, we use the `doSomething` function on each element when we push it into the return value. `doSomething` multiplies each value by 2, hence the array `[1,2,3]` becomes `[2,4,6]`.

19) The output will be `1 4 3 2`. Line 4 is delayed less since the second parameter is 0. It will run after the non-delay statements. Line 3 will be last since it has a delay of 1000 ms.
 







 <!-- https://stackoverflow.com/questions/49331947/why-does-a-settimeout-delay-of-0-still-run-after-all-other-synchronous-code-in-a -->