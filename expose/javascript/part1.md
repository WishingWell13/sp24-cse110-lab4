### Part 1 

Question `var`:
1) `values added: 20` is printed by line 9. 

2) Line 13 will never print, because the return statement will trigger first. However, it will not cause a compile error since `result` is global

Question `let`
1) `values added: 20` is printed by line 9.
2) Line 13 will error. `let` means that `result` is block scoped, and since line 13 is outside the if statement, `result` is no longer accessible.

Question `const`
1) There should be an error on line 7. We try to reassign a variable `result` that is a const.
2) There should be an error on line 7. We try to reassign a variable `result` that is a const. Additionally, const is block scoped, so it is not accessible on line 13.

### Part 2:
