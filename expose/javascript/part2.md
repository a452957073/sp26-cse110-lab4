
# Part 2

## Question 1

Answer:

3

Explanation:

The variable i is declared using var inside the for loop. Since var has function scope, the variable i is accessible outside the loop. After the loop finishes, i becomes 3 (because the loop stops when i equals prices.length, which is 3). Therefore, line 12 prints 3.

---

## Question 2

Answer:

150

Explanation:

The variable discountedPrice is declared using var inside the for loop, which means it has function scope. Therefore, it can still be accessed outside the loop. After the loop finishes, discountedPrice holds the value from the last iteration, which is 300 * (1 - 0.5) = 150. So line 13 prints 150.

---

## Question 3

Answer:

150

Explanation:

The variable finalPrice is declared using var, so it has function scope and can be accessed outside the loop. During the loop, finalPrice is updated in each iteration. After the loop finishes, it holds the value from the last iteration, which is 300 * (1 - 0.5) = 150. Therefore, line 14 prints 150.

---

## Question 4

Answer:

[50, 100, 150]

Explanation:

The function loops through the prices array and applies the discount to each value. Each discounted price is rounded and added to the discounted array. For the input [100, 200, 300] with a discount of 0.5, the values become 50, 100, and 150. Therefore, the function returns [50, 100, 150].

---

## Question 5

Answer:

ReferenceError: i is not defined

Explanation:

The variable i is declared using let inside the for loop, which means it has block scope. Therefore, i only exists inside the loop block. Line 12 is outside the loop, so it cannot access i, resulting in a ReferenceError.

---

## Question 6

Answer:

ReferenceError: discountedPrice is not defined

Explanation:

The variable discountedPrice is declared using let inside the for loop, so it has block scope. It only exists inside the loop. Line 13 is outside the loop, so it cannot access discountedPrice, resulting in a ReferenceError.

---

## Question 7

Answer:

150

Explanation:

The variable finalPrice is declared using let outside the loop, so it has function scope and can be accessed after the loop. Inside the loop, finalPrice is updated in each iteration. After the loop finishes, it holds the value from the last iteration, which is 300 * (1 - 0.5) = 150. Therefore, line 14 prints 150.

---

## Question 8

Answer:

[50, 100, 150]

Explanation:

The function iterates through the prices array and calculates the discounted price for each value. Each result is rounded and pushed into the discounted array. Since all variables are properly scoped and used within their valid blocks, there is no error. For the input [100, 200, 300] with a discount of 0.5, the function returns [50, 100, 150].

---

## Question 9

Answer:

ReferenceError: i is not defined

Explanation:

The variable i is declared using let inside the for loop, which means it has block scope. Therefore, i only exists inside the loop block. Line 11 is outside the loop, so it cannot access i, resulting in a ReferenceError.

---

## Question 10

Answer:

3

Explanation:

The variable length is declared using const inside the function, so it has block scope within the function and is accessible after the loop. It is assigned the value of prices.length, which is 3. Therefore, line 12 prints 3.

---

## Question 11

Answer:

[50, 100, 150]

Explanation:

The function iterates through the prices array and calculates the discounted price for each element. Each result is stored in the discounted array using push(). Since all variables are properly scoped and no invalid reassignment occurs, the function runs without errors. For the input [100, 200, 300] with a discount of 0.5, the function returns [50, 100, 150].

---

## Question 12

### A

Answer:

student.name

### B

Answer:

student['Grad Year']

### C

Answer:

student.greeting()

### D

Answer:

student['Favorite Teacher'].name

### E

Answer:

student.courseLoad[0]

---

## Question 13: Arithmetic

### A. `'3' + 2`

Answer:

'3' + 2 → '32'

Explanation:

Explanation: string + number → number becomes string → concatenation

### B. `'3' - 2`

Answer:

'3' - 2 → 1

Explanation:

'-' converts string to number → 3 - 2 = 1

### C. `3 + null`

Answer:

3 + null → 3

Explanation:

null becomes 0 → 3 + 0 = 3

### D. `'3' + null`

Answer:

'3' + null → '3null'

Explanation:

string + null → null becomes 'null' → concatenation

### E. `true + 3`

Answer:

true + 3 → 4

Explanation:

true becomes 1 → 1 + 3 = 4

### F. `false + null`

Answer:

false + null → 0

Explanation:

false = 0, null = 0 → 0 + 0 = 0

### G. `'3' + undefined`

Answer:

'3' + undefined → '3undefined'

Explanation:

string + undefined → undefined becomes 'undefined'

### H. `'3' - undefined`

Answer:

'3' - undefined → NaN

Explanation:

undefined becomes NaN → result is NaN

---

## Question 14: Comparison

### A. `'2' > 1`

Answer:

'2' > 1 → true 

Explanation:

'2' becomes 2 → 2 > 1

### B. `'2' < '12'`

Answer:

'2' < '12' → false

Explanation:

string comparison → compares character by character ('2' > '1')

### C. `2 == '2'`

Answer:

2 == '2' → true

Explanation:

== converts types → 2 == 2

### D. `2 === '2'`

Answer:

2 === '2' → false

Explanation:

=== checks type → number ≠ string

### E. `true == 2`

Answer:

true == 2 → false

Explanation:

true = 1 → 1 ≠ 2

### F. `true === Boolean(2)`

Answer:

true === Boolean(2) → true

Explanation:

Boolean(2) = true → same type and value

---

## Question 15

Answer:

The == operator compares values after performing type conversion, while the === operator compares both value and type without conversion. Therefore, === is stricter and more predictable.

---

## Question 16

Answer:

This answer is in `part2-question16.js`.

---

## Question 17

Answer:

[2, 4, 6]

Explanation:

The function modifyArray loops through the array [1, 2, 3]. For each element, it calls the callback function doSomething, which multiplies the number by 2. So the values become 2, 4, and 6. These results are stored in a new array and returned.

---

## Question 18

Answer:

This answer is in `part2-question18.js`.

---

## Question 19

Answer:

1
4
3
2

Explanation:

The synchronous code runs first, so 1 and 4 are printed immediately. The setTimeout with 0 delay (printing 3) runs next, because it is placed in the event queue and executed after the current call stack. Finally, the setTimeout with 1000ms delay (printing 2) runs after 1 second.
