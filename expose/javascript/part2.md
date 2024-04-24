### Part 2

1) Line 12 will print the value of `prices.length` (which is 3), because it occurs after the end of the for loop and the end condition is `prices.length`. Since the variable is a `var`, it has a function scope, so line 12 is still a valid place to call `i` (both line 6 and 12 are in the same function).

2) Line 13 will print the value of `150`, because it is overwritten until the last value of the array multipled by the discount (300 * (1-0.5)). Since the variable is a `var`, it has a function scope, so line 13 is still a valid place to call `discountedPrice` (both line 6 and 12 are in the same function).

3) Line 14 will print the value of `150`, because it is overwritten until the last iteration of the loop. Since the variable is a `var`, it has a function scope, so line 14 is still a valid place to call `discountedPrice` (both line 6 and 12 are in the same function).

4) This function will return `[50, 200, 300]`. The function goes through each value and multiplies it by `1-discountedPrice`. In this case, `discountedPrice` is 0.5, so we multiply by 0.5.

5) Line 12 will error. `i` is a block scope variable. The block `i` is defined in is the `for` loop. Line 12 is outside the for loop.

6) Line 13 will error. `discounted` is a block scope variable. The block `discounted` is defined in is the `for` loop. Line 13 is outside the for loop.

7) Line 14 will not cause an error because `finalPrice` is defined outside the for loop. Therefore, it is accessable in the entire function, because `let` means the variable is block scoped. `finalPrice` should be 150 at the console.log statement.

8) This function will return `[50, 200, 300]`. The function goes through each value and multiplies it by `1-discountedPrice`. In this case, `discountedPrice` is 0.5, so we multiply by 0.5.
