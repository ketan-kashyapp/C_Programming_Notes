## 🔢 Operators in C (With Simple Desi Explanation)

Operators C language me values aur variables par operations perform karne ke liye use hote hain.

Aaj hum important **Arithmetic Operators** ko examples ke saath dekhenge! 🚀

---

## ✨ Arithmetic Operators in C

Arithmetic operators mathematical calculations ke liye use hote hain.
Ye numbers par basic operations perform karte hain:

### 🔹 1️⃣ Addition (`+`)

Dono numbers ko jodta hai. Simple math! ➕

```c
#include <stdio.h>
int main() {
    int a = 10;
    int b = 20;
    int sum = a + b; // Addition
    printf("Addition of %d and %d is: %d\n", a, b, sum);
    return 0;
}
```

🧠 **Explanation:** 10 + 20 = 30. Jo `sum` me store ho raha hai.

---

### 🔹 2️⃣ Subtraction (`-`)

Dono numbers me se ek ko doosre se ghatata hai ➖

```c
#include <stdio.h>
int main() {
    int a = 20;
    int b = 14;
    int sub = a - b;
    printf("Subtraction of %d and %d is: %d\n", a, b, sub);
    return 0;
}
```

🧠 **Explanation:** 20 - 14 = 6

---

### 🔹 3️⃣ Multiplication (`*`)

Dono numbers ka guna karta hai ✖️

```c
#include <stdio.h>
int main() {
    int a = 20;
    int b = 10;
    int product = a * b;
    printf("Product of %d and %d is: %d\n", a, b, product);
    return 0;
}
```

🧠 **Explanation:** 20 * 10 = 200

---

### 🔹 4️⃣ Division (`/`)

Ek number ko doosre se bhaag karta hai. Lekin dhyan rahe:
**Agar dono integer hain to output bhi sirf integer part hota hai.** ➗

```c
#include <stdio.h>
int main() {
    int a = 15;
    int b = 4;
    int divide = a / b;
    printf("Division of %d and %d is: %d\n", a, b, divide);
    return 0;
}
```

🧠 **Explanation:** 15 / 4 = 3.75 hota, but C sirf `3` dikhata kyunki dono integers hain.

---


### 🔹 5️⃣ Modulus (`%`)

Division ke baad jo remainder (sheshfal) bacha usko dikhata hai ➰

```c
#include <stdio.h>
int main() {
    int a = 13;
    int b = 2;
    int remainder = a % b;
    printf("Remainder of %d and %d is: %d\n", a, b, remainder);
    return 0;
}
```

🧠 **Explanation:** 13 % 2 = 1 (kyunki 13 divide by 2 me 6 \* 2 = 12 and 1 remainder bacha)

---

## 🔍 Summary Table

| Operator | Symbol | Use Case         | Example (a = 10, b = 3) | Output |
| -------- | ------ | ---------------- | ----------------------- | ------ |
| Add      | `+`    | Addition         | a + b                   | 13     |
| Subtract | `-`    | Subtraction      | a - b                   | 7      |
| Multiply | `*`    | Multiplication   | a \* b                  | 30     |
| Divide   | `/`    | Integer Division | a / b                   | 3      |
| Modulus  | `%`    | Remainder (Mod)  | a % b                   | 1      |

📚 Bas itna yaad rakho, aur practice karte raho.🧠💪

✅ Properly Aligned Markdown Table: Operator Precedence in C

| **Priority (High → Low)** | **Operators**                     | **Category**   | **Associativity** |            |               |
| ------------------------- | --------------------------------- | -------------- | ----------------- | ---------- | ------------- |
| 1                         | `()` `[]` `.` `->`                | Postfix        | Left to Right     |            |               |
| 2                         | `++` `--` (prefix/postfix)        | Unary          | Right to Left     |            |               |
| 3                         | `+` `-` (unary), `!` `~`          | Unary          | Right to Left     |            |               |
| 4                         | `*` `/` `%`                       | Multiplicative | Left to Right     |            |               |
| 5                         | `+` `-`                           | Additive       | Left to Right     |            |               |
| 6                         | `<` `<=` `>` `>=`                 | Relational     | Left to Right     |            |               |
| 7                         | `==` `!=`                         | Equality       | Left to Right     |            |               |
| 8                         | `&&`                              | Logical AND    | Left to Right     |            |               |
| 9                         | \`                                |                | \`                | Logical OR | Left to Right |
| 10                        | `=` `+=` `-=` `*=` `/=` `%=` etc. | Assignment     | Right to Left     |            |               |
| 11                        | `,`                               | Comma          | Left to Right     |            |               |

🔍 Explanation in Simple Words (Desi Style):

👉 Precedence:
Jaise class mein monitor ki baat sabse pehle maani jaati hai, waise hi high precedence waale operator ki value pehle nikaali jaati hai.

Example: 2 + 3 * 4
Here * has higher precedence than +, so 3 * 4 = 12 first, then 2 + 12 = 14.

👉 Associativity:
Jab ek jaise priority ke operator ho, toh kaun pehle chalega—yeh decide hota hai associativity se.

🧠 Most operators have Left to Right associativity.
But kuch operators (like = and ++ in prefix form) have Right to Left associativity.

                                                   📌 Chhote Examples for Clear Understanding:

1️⃣ Multiplicative vs Additive (Priority check)

    int x = 2 + 3 * 4;  // x = 2 + 12 = 14 (Multiplication first)

2️⃣ Same precedence → Associativity check

    int x = 10 - 5 - 2;  // Left to Right: (10 - 5) = 5, then 5 - 2 = 3

3️⃣ Assignment (Right to Left Associativity)

    int a, b, c;
    a = b = c = 5;  // Interpreted as: a = (b = (c = 5))  

4️⃣ Comma Operator (Lowest Precedence)

    int x = (1 + 2, 3 + 4);  // x = 7 (because comma returns last value)      


💡 Tips to Remember:

Brackets () have highest priority. Use them to control expression flow manually.
Assignment and Unary (++, --, =, etc.) are usually Right to Left.
When in doubt, use brackets to avoid confusion.    


— ye tumhare har expression ko samajhne me madad karega, especially jab multiple operators ek hi line me use hote hain.


✅ 📘 Modulus Operator (%) – Visual Use Case Chart

| 🔍 Use-Case                                   | 💡 Logic Example (`x % y`) | 🎯 Real-World Application Example                                 |
| --------------------------------------------- | -------------------------- | ----------------------------------------------------------------- |
| 🔢 **Last Digit Nikalna**                     | `number % 10`              | `253 % 10 = 3` → Last digit of 253 is 3                           |
| 👬 **Even/Odd Check**                         | `number % 2`               | `5 % 2 = 1 → Odd`, `8 % 2 = 0 → Even`                             |
| 🕒 **Clock Time Wraparound**                  | `hours % 12`               | `14 % 12 = 2` → 14:00 = 2:00 PM (12-hour clock format)            |
| 🔁 **Repeating Patterns (e.g. colors, days)** | `index % n`                | `index % 7` → Days of week, `index % 3` → Red, Green, Blue repeat |
| 🎯 **Circular Buffer Logic**                  | `i = (i + 1) % size`       | Used in queues, circular arrays, rotating banners, etc.           |
| 🎲 **Game Turns / Player Switching**          | `turn % numPlayers`        | `turn % 2` → Switch between Player 1 & 2                          |
| 📦 **Group Distribution / Batching**          | `itemNumber % groupSize`   | Distribute students into 3 groups → `rollNo % 3`                  |


🔁 Visual Understanding:

```c
Number = 253
253 % 10 = 3   → Last Digit = 3

Number = 18
18 % 2 = 0     → Even Number

Clock: 14:00
14 % 12 = 2    → Time = 2:00 PM

Index: 9
9 % 3 = 0      → 0th color in [Red, Green, Blue] → Red again


🧠 Tip for Interviews & Coding:

Modulus operator is used whenever there's cyclical, repeating, or remainder-based logic.

It’s extremely important in game logic, array indexing, and number analysis.