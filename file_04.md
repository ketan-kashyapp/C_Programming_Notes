# 🟢 Keywords, Identifiers, and Naming Conventions 🎯

---

## 🔹 Keywords (Reserved Words)

- Keywords woh words hote hain jo **C language me pehle se reserve** hote hain.
- Inko **variable ya function name** ke liye use **nahi** kiya ja sakta.

### ❌ Wrong Usage:
int return = 10;  // ERROR! 'return' ek keyword hai.

✅ Correct Usage:
int myReturn = 10;  // Sahi tarika hai.


## 📖 Total 32 Reserved Keywords in C 🎯

🔹 Data Type Keywords:
int, float, double, char, void

🔹 Control Flow Keywords:
if, else, switch, case, default

🔹 Looping Keywords:
for, while, do, break, continue

🔹 Storage Class Keywords:
auto, static, extern, register, volatile

🔹 Return & Jump Keywords:
return, goto

🔹 Modifiers (Type Qualifiers):
const, signed, unsigned, short, long

🔹 Structure & Memory Management:
struct, union, enum, sizeof, typedef


## 📝 Important Notes:

✅ Keywords case-sensitive hote hain (int ≠ Int)
✅ Yeh system ke predefined functions hote hain
✅ Inko variable/function name ke roop me use nahi kar sakte


## 📌 Naming Conventions for Variables and Functions

🔹 **Rules for Naming Identifiers:**

✅ Allowed: Alphabets (a-z, A-Z), Digits (0-9), Underscore (_)

❌ Not Allowed: Special characters (@, $, %, etc.), Spaces

🚫 Identifier kabhi bhi digit se start nahi ho sakta

⚠️ C is case-sensitive → Age and age are different


## ✅ Valid Examples:

int myAge  = 18;    // Correct
int _count =  5;    // Correct
int 2count = 10;    // ❌ ERROR – cannot start with digit


## 👉 Function Naming Conventions 🎯

🎯 Convention	  🎯 Example	          🎯 Use Case
camelCase	     calculateSum()	      Function names
snake_case	     calculate_sum	      Variables & constants
PascalCase	     CalculateSum	      Structs & Classes


## 🚀 Example Code: Naming Best Practices 🎯

```c
#include <stdio.h>

// CamelCase function name
int calculateSum(int a, int b) {
    return a + b;
}

int main() {
    int total_sum = calculateSum(5, 10);  // Snake_case for variable
    printf("Sum: %d\n", total_sum);
    return 0;
}