# 📌 Assignment Operators in C

Assignment Operators C language me variables ko value assign karne ke liye use hote hain. Yeh operators left-hand side ke variable me right-hand side ki value ko store kar dete hain.

---

## 🔹 Types of Assignment Operators

| Operator | Description               | Example                          |
| -------- | ------------------------- | -------------------------------- |
| =        | Simple assignment         | `a = 10;` (assigns 10 to a)      |
| +=       | Addition assignment       | `a += 5;` (same as `a = a + 5;`) |
| -=       | Subtraction assignment    | `a -= 3;` (same as `a = a - 3;`) |
| \*=      | Multiplication assignment | `a *= 2;` (same as `a = a * 2;`) |
| /=       | Division assignment       | `a /= 2;` (same as `a = a / 2;`) |
| %=       | Modulus assignment        | `a %= 3;` (same as `a = a % 3;`) |

---

## ✅ Example Flow:

Agar `a = 10` hai, to step-by-step result:

```c
 a += 5;   // a = 15
 a -= 3;   // a = 12
 a *= 2;   // a = 24
 a /= 4;   // a = 6
 a %= 5;   // a = 1
```

---

## 🧠 Short Explanation:

* **=** : Directly kisi variable ko value assign karta hai.
* \**+=, -=, *=, /=, %=** : Shortcut operators hain jo existing value ko modify kar dete hain.

---

## 💼 Real-Life Use Cases of Assignment Operators:

### 1️⃣ ATM Machine (Balance Update)

➡️ Jab paisa withdraw hota hai:

```c
 balance -= amount;
```

### 2️⃣ Shopping Cart (Total Price Calculation)

➡️ Jab naya item add hota hai:

```c
 totalPrice += itemPrice;
```

### 3️⃣ Student Marks Calculation

➡️ Jab alag subjects ke marks add hote hain:

```c
 totalMarks += subjectMark;
```

### 4️⃣ Salary Calculation with Bonus

➡️ Jab salary me bonus add hota hai:

```c
 salary += bonus;
```

### 5️⃣ Battery Percentage Update

➡️ Jab phone charge/discharge hota hai:

```c
 batteryPercent += charge; // charging
batteryPercent -= usage;   // discharging
```

---

## 📊 Visual Table - Summary

| Assignment Operator | Use Case Examples                       |
| ------------------- | --------------------------------------- |
| =                   | Balance set karna, marks assign karna   |
| +=                  | Salary increment, total price add karna |
| -=                  | Money withdraw, battery usage update    |
| \*=                 | Discounts, salary hike calculation      |
| /=                  | EMI divide karna, tax deductions        |
| %=                  | Time ya remainder calculations          |

---

## 📌 Summary:

* Assignment operators help in assigning and updating values efficiently.
* Real-life applications me yeh bahut important role play karte hain.
* Yeh operators programming ko clean aur easy-to-read banate hain.

🎯 Next Step: Practice in small code snippets to get comfortable with each operator!
