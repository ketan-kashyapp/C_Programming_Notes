## 📌 Logical Operators in C 🚀

Logical operators **multiple conditions** ko check karne ke liye use hote hain.
Yeh hamesha **true (1)** ya **false (0)** return karte hain.

### 🔹 Types of Logical Operators

| Operator | Meaning                         | Result Condition                                    |
|----------|----------------------------------|-----------------------------------------------------|
| `&&`     | Logical AND                     | True **only if both** conditions are true           |
| `||`     | Logical OR                      | True if **at least one** condition is true          |
| `!`      | Logical NOT (Negation)          | **Inverts** the result (true → false, false → true) |

---



### ✅ 1️⃣ AND (`&&`) Operator → Dono conditions true honi chahiye

```c
#include <stdio.h>
int main() {
    int a = 20, b = 40;

    if(a > 12 && b > 35) {
        printf("\u2705 Both conditions are true!\n");
    } else {
        printf("\u274C One or both conditions are false!\n");
    }
    return 0;
}
```

**📝 Explanation:**
- `a > 12` → true
- `b > 35` → true
- ✔️ AND (&&) me dono true → output: **Both conditions are true!**

---



### ✅ 2️⃣ OR (`||`) Operator → Koi bhi ek condition true honi chahiye

```c
#include <stdio.h>
int main() {
    int x = 5, y = 10;

    if (x > 3 || y > 20) {
        printf("\n At least one condition is true!\n");
    } else {
        printf("\n Both conditions are false!\n");
    }
    return 0;
}
```

**📝 Explanation:**
- `x > 3` → true
- `y > 20` → false
- ✔️ OR (||) me koi bhi ek true ho → output: **At least one condition is true!**

---



### ✅ 3️⃣ NOT (`!`) Operator → Result ko ulta kar deta hai

```c
#include <stdio.h>
int main() {
    int x = 14, y = 16;

    if (!(x < y)) {
        printf("\u274C This condition is false (inverted)!\n");
    } else {
        printf("\u2705 This condition is true!\n");
    }
    return 0;
}
```

**📝 Explanation:**
- `x < y` → 14 < 16 → true
- `!true` → false → isliye `else` block chalega

```c

💡 Golden Rule:

| Value       | `!value`    | Meaning                  | Action              |
| ----------- | ----------- | ------------------------ | ------------------- |
| `0` (false) | `1` (true)  | Condition chalegi ✅      | IF block run hoga   |
| `1` (true)  | `0` (false) | Condition nahi chalegi ❌ | ELSE block run hoga |

🧠 Sochne ka Shortcut:

! matlab "ulta sochna" – agar 1 hai to 0, agar 0 hai to 1

IF me hamesha true (1) condition hi chalta hai

ELSE tab chalta hai jab IF false ho
```c


=========================================================================================================================================================================

Double NOT Operator (!!) :-


📘 Syntax:  int result = !!value;


💡 Kya hota hai !!value

| Step      | Logic                                                            | Result         |
| --------- | ---------------------------------------------------------------- | -------------- |
| `!value`  | Pehle value ko invert karta hai (0 → 1, non-zero → 0)            | ✅ Invert       |
| `!!value` | Phir dobara invert karta hai → Original boolean version deta hai | ✅ Boolean form |

🧠 Purpose:

🔸 Kisi bhi value ko explicit 0 ya 1 mein convert karna.
🔸 C language mein koi bhi non-zero value = true, aur 0 = false hota hai.


✅ Use Case in Real Code:

int age = 25;
int isValid = !!age;  // 25 → true (1)

int discount = 0;
int canApply = !!discount;  // 0 → false (0)


✅ !!value ka logic:

Koi bhi value agar non-zero (true) hai to !!value usse 1 (true) bana deta hai.
Aur agar value zero (false) hai to !!value usse 0 (false) bana deta hai.


🔍 Breakdown:

| Value | Meaning         | `!value` | `!!value` |
| ----- | --------------- | -------- | --------- |
| 0     | False           | 1        | 0         |
| 5     | True (non-zero) | 0        | 1         |
| -3    | True (non-zero) | 0        | 1         |
| 100   | True (non-zero) | 0        | 1         |



📌 Final Rule (yaad rakhne layak):

!!value sirf yeh check karta hai ki value truthy hai ya falsy — aur uska clean 0 ya 1 return karta hai.


=========================================================================================================================================================================

### 📊 Visual Summary Chart

```c
| Condition A | Condition B | A && B | A || B | !A |
|-------------|-------------|--------|--------|-----|
| true        | true        | true   | true   | false
| true        | false       | false  | true   | false
| false       | true        | false  | true   | true
| false       | false       | false  | false  | true
```

---

### 🔁 Summary / Recap:

- `&&` → Dono condition true ho → Tabhi true
- `||` → Koi bhi ek true ho → True
- `!` → Output ko ulta kar deta hai

👉 Logical operators ka use **if statements**, **loops**, aur **complex conditions** me hota hai.
