# Unit 2: Arithmetic Expressions and Precedence in C 

C supports various operators to perform operations on data. Understanding **operator precedence and associativity** is important to evaluate expressions correctly.

## ✅ Operators and Expressions

### 1️⃣ Numeric Operators

* **Arithmetic Operators:** `+`, `-`, `*`, `/`, `%`

```c
int a = 5, b = 2;
printf("%d", a + b); // 7
printf("%d", a % b); // 1
```

### 2️⃣ Relational Operators

* Compare values and return `1` (true) or `0` (false).
* Operators: `==`, `!=`, `<`, `>`, `<=`, `>=`

```c
int x = 5, y = 10;
printf("%d", x < y); // 1
```

### 3️⃣ Mixed Operands and Type Conversion

* When operands are of different types, C performs **type promotion**.

```c
int a = 5;
double b = 2.0;
double c = a + b; // int promoted to double
```

### 4️⃣ Logical Operators

* Used for logical conditions: `&&` (AND), `||` (OR), `!` (NOT)

```c
int a = 1, b = 0;
printf("%d", a && b); // 0
printf("%d", !a); // 0
```

### 5️⃣ Bitwise Operators

* Operate at the bit level: `&`, `|`, `^`, `~`, `<<`, `>>`

```c
int a = 5, b = 3;
printf("%d", a & b); // 1
printf("%d", a << 1); // 10
```

### 6️⃣ Assignment Operators

* Used to assign values: `=`, `+=`, `-=`, `*=`, `/=`, `%=`

```c
int x = 5;
x += 3; // x = 8
```

### 7️⃣ Operator Precedence and Associativity

* Determines the order of evaluation in expressions.
* Example:

```c
int a = 5 + 3 * 2; // Multiplication first, result 11
```

* **Important points:**

  * `()` has highest precedence
  * Multiplication/division/modulus `* / %` next
  * Addition/subtraction `+ -` next
  * Relational `< <= > >=`, then equality `== !=`
  * Logical `&&`, `||` next
  * Assignment `=` has lowest precedence

🧠 Explanation:
Understanding precedence ensures that expressions are evaluated correctly without unexpected

# Conditional Statements in C (Decision Making)

Conditional statements in C are used to make decisions.
Meaning:
👉 "If this condition is true, do this, otherwise do that"

Real-life example:

If it rains → take an umbrella
Else → go outside normally ✅

## ✅ Types of Conditional Statements in C

1️⃣ if
2️⃣ if-else
3️⃣ else-if ladder
4️⃣ nested if
5️⃣ switch-case

### 1️⃣ if Statement (Single Condition Check)

👉 Used when you need to check only one condition.

✅ Syntax:

```c
if(condition) {
    // statements
}
```

✅ Example:

```c
#include <stdio.h>
int main() {
    int age = 20;
    if(age >= 18) {
        printf("You are eligible to vote");
    }
    return 0;
}
```

🧠 Explanation:
If age is 18 or more → the message will be printed.

### 2️⃣ if-else Statement (True or False)

👉 Used when both cases (true & false) need to be handled.

✅ Syntax:

```c
if(condition) {
    // true block
} else {
    // false block
}
```

✅ Example:

```c
#include <stdio.h>
int main() {
    int num = 10;
    if(num % 2 == 0)
        printf("Even Number");
    else
        printf("Odd Number");
    return 0;
}
```

🧠 Explanation:
Even → if remainder is 0
Odd → if remainder is 1

### 3️⃣ else-if Ladder (Multiple Conditions)

👉 Used when multiple conditions need to be checked.

✅ Syntax:

```c
if(condition1) {
}
else if(condition2) {
}
else if(condition3) {
}
else {
}
```

✅ Example:

```c
#include <stdio.h>
int main() {
    int marks = 82;

    if(marks >= 90)
        printf("Grade A");
    else if(marks >= 75)
        printf("Grade B");
    else if(marks >= 50)
        printf("Grade C");
    else
        printf("Fail");

    return 0;
}
```

🧠 Explanation:
Grade is decided based on marks.

### 4️⃣ Nested if Statement (if inside if)

👉 Used when you need to check a condition inside another condition.

✅ Example:

```c
#include <stdio.h>
int main() {
    int a = 10, b = 20;

    if(a > 0) {
        if(b > 0) {
            printf("Both are positive numbers");
        }
    }
    return 0;
}
```

🧠 Explanation:
Both conditions must be true for the output to appear.

### 5️⃣ switch-case Statement (Menu Type Selection)

👉 Used when a variable has multiple fixed options. It is a faster version of if-else ladder ✅

✅ Syntax:

```c
switch(expression) {
    case value1:
        statements;
        break;
    case value2:
        statements;
        break;
    default:
        statements;
}
```

✅ Example:

```c
#include <stdio.h>
int main() {
    int day = 3;

    switch(day) {
        case 1: printf("Monday"); break;
        case 2: printf("Tuesday"); break;
        case 3: printf("Wednesday"); break;
        default: printf("Invalid Day");
    }
    return 0;
}
```

🧠 Explanation:
day = 3 → Output = Wednesday

### ✅ Difference: if-else vs switch

| Point               | if-else    | switch         |
| ------------------- | ---------- | -------------- |
| Multiple conditions | ✅ Yes      | ✅ Yes          |
| Range comparison    | ✅ Possible | ❌ Not possible |
| Only integer/char   | ❌          | ✅              |
| Speed               | Slow       | Faster         |

### ✅ Important Exam Points (Direct Theory Lines ✍️)

✔ if statement is used for single condition checking.
✔ if-else executes one block when condition is true and another when false.
✔ else-if ladder is used for checking multiple conditions.
✔ switch statement selects execution based on fixed constant values.
✔ break prevents fall-through in switch.
✔ default runs if no case matches.

----
----

# Iteration and Loops in C

Loops are used to execute a block of code repeatedly until a condition is met.

## ✅ Types of Loops in C

1️⃣ while loop
2️⃣ do-while loop
3️⃣ for loop

### 1️⃣ while Loop (Entry Controlled Loop)

👉 Executes a block of code as long as the condition is true.

✅ Syntax:

```c
while(condition) {
    // statements
}
```

✅ Example:

```c
#include <stdio.h>
int main() {
    int i = 1;
    while(i <= 5) {
        printf("%d\n", i);
        i++;
    }
    return 0;
}
```

🧠 Explanation: Prints numbers from 1 to 5.

### 2️⃣ do-while Loop (Exit Controlled Loop)

👉 Executes the block first and checks the condition later.

✅ Syntax:

```c
do {
    // statements
} while(condition);
```

✅ Example:

```c
#include <stdio.h>
int main() {
    int i = 1;
    do {
        printf("%d\n", i);
        i++;
    } while(i <= 5);
    return 0;
}
```

🧠 Explanation: Executes at least once even if the condition is false.

### 3️⃣ for Loop (Fixed Number of Iterations)

👉 Used when the number of iterations is known.

✅ Syntax:

```c
for(initialization; condition; increment/decrement) {
    // statements
}
```

✅ Example:

```c
#include <stdio.h>
int main() {
    for(int i = 1; i <= 5; i++) {
        printf("%d\n", i);
    }
    return 0;
}
```

🧠 Explanation: Prints numbers from 1 to 5.

### ✅ Multiple Loop Variables

👉 You can use multiple variables in a for loop.

```c
for(int i = 0, j = 10; i <= 5; i++, j--) {
    printf("i = %d, j = %d\n", i, j);
}
```

### ✅ Break, Continue, and Goto Statements

* **break:** Exits the loop immediately.
* **continue:** Skips the current iteration and moves to the next.
* **goto:** Jumps to a labeled statement in the program.

✅ Example:

```c
#include <stdio.h>
int main() {
    for(int i = 1; i <= 5; i++) {
        if(i == 3) continue; // skips 3
        if(i == 5) break;    // stops at 5
        printf("%d\n", i);
    }
    return 0;
}
```

🧠 Explanation: Loop prints 1, 2, 4 and stops before 5.
