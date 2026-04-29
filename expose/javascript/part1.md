# Part 1

## Question 1

Answer: 

values added: 20

Explanation: When add is true, the code inside the if block runs. The variable result is set to num1 + num2, which is 10 + 10 = 20. So line 9 prints "values added: 20".

## Question 2

Answer:

final result: 20

Explanation:The variable result is declared using var, which has function scope. This means it can be accessed outside the if block. Therefore, line 13 can still access result and prints "final result: 20".

## Question 3

Answer:

We should not use var because it has function scope instead of block scope, which can cause unexpected behavior. Variables declared with var can be accessed outside the block where they are defined, leading to bugs and confusion. It is better to use let or const because they have block scope and are safer.

## Question 4

Answer:

values added: 20

Explanation:When add is true, the if block runs. Inside the block, result is set to num1 + num2, which is 10 + 10 = 20. So line 9 prints "values added: 20".

## Question 5

Answer:

ReferenceError: result is not defined

Explanation: result is declared with let inside the if block. let has block scope, so result only exists inside the if block. Line 13 is outside the if block, so it cannot access result.

## Question 6

Answer:

TypeError: Assignment to constant variable.

Explanation: The variable result is declared with const, which means it cannot be reassigned. On line 7, the code tries to assign a new value to result (num1 + num2), which causes an error. Therefore, line 9 is never executed.

## Question 7

Answer:

TypeError: Assignment to constant variable.

Explanation: Because the code throws an error on line 7 when trying to reassign a const variable, the function stops executing. As a result, line 13 is never reached and nothing is printed.
