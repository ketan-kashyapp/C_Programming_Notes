# 📘 C Programming: Variables, `printf()` and `scanf()` Mastery 🚀

---

## 🟢 1. Variable Declaration & Initialization

### 🔹 1. Normal Declaration (Without Initialization)

```c
#include <stdio.h>
int main() {
    int a;
    float b;
    char c;
    double d;
    return 0;
}

👉 Isme sirf variables ko declare kiya gaya hai, initialize nahi kiya gaya.



🔹 2.  Declaration + Initialization Together

#include <stdio.h>
int main() {
    int a = 10;
    float b = 5.5;
    char c = 'A';
    double d = 12.3456;
    return 0;
}

👉 Yeh recommended tarika hai agar value already pata ho.



🔹 3. Multiple Variable Declaration on One Line

int a = 10, b = 20, c = 30;
float x = 1.2, y = 2.3, z = 3.4;

👉 Ek hi type ke multiple variables ek saath declare/initialize karne ke liye.



🔹 4. Without Initialization (but using later)

#include <stdio.h>
int main() {
    int a;
    a = 50;  // Value later assign ki
    printf("Value of a: %d", a);
    return 0;
}

👉 Variable ko pehle declare karke baad me value assign kar sakte hain.



🔹 5. Constant Variable (Value Change Not Allowed)

const int a = 100;
a = 200;  // ❌ ERROR! Const variable ki value change nahi hoti

👉 const ka use fix value ke liye hota hai.



--------------------------------------------------------------------------------------------------------------------------------------

# 🖨️ C Programming: printf() Function Examples

`printf()` function C programming me output display karne ke liye use hota hai. Neeche kuch commonly used examples diye gaye hain jo beginners ke liye helpful honge. 👇

---

## 📌 1. Normal printf() (Direct Output)

```c
printf("Hello, World!");
```

✅ Jab simple text output print karna ho bina kisi variable ke.

---

## 📌 2. Variable ke Saath printf()

```c
int age = 18;
printf("Your age is %d", age);
```

✅ Jab kisi variable ka value print karna ho.

---

## 📌 3. Multiple Variables ek saath printf()

```c
int a = 10, b = 20;
printf("A = %d, B = %d", a, b);
```

✅ Jab ek se zyada variables ko ek hi line me print karna ho.

---

## 📌 4. printf() me Formatting (Integer, Float, Character, etc.)

```c
int x = 5;
float y = 5.6789;
char c = 'A';

printf("Integer: %d\n", x);
printf("Float: %.2f\n", y);
printf("Character: %c\n", c);
```

✅ Jab alag-alag data types ko format karke print karna ho.

---

## 🔁 Format Specifiers Quick Reference

| Format | Data Type | Example Output   |
|--------|-----------|----------------  |
| `%d`   | int       | 42               |
| `%f`   | float     | 3.14          c  |
| `%.2f` | float     | 3.14 (2 decimal) |
| `%c`   | char      | A                |
| `%s`   | string    | Hello            |

---

📢 **Note:** `\n` ka use new line ke liye hota hai. 

---

> 💡 Tip: Aap `\t` (tab), `\n` (newline), aur `%%` (percentage print) bhi use kar sakte ho.



-------------------------------------------------------------------
-------------------------------------------------------------------

# 🟢 scanf() Function Examples in C 📥

## 📌 1. Simple `scanf()` (User se Input lena)

```c
int num;
scanf("%d", &num);
```

✅ Jab user se ek integer input lena ho.

---

## 📌 2. Multiple Input ek saath `scanf()`

```c
int a, b;
scanf("%d %d", &a, &b);
```

✅ Jab ek line me user se multiple values leni ho.

---

## 📌 3. Different Data Types ke saath `scanf()`

```c
int age;
float height;
char gender;

printf("Enter age, height, and gender: ");
scanf("%d %f %c", &age, &height, &gender);
```

✅ Jab user se alag-alag type ke inputs lene ho.

---

📌 **Note:** 
- `%d` → Integer ke liye
- `%f` → Float ke liye
- `%c` → Character ke liye
- `&` → Variable ka address dena zaroori hai `scanf()` ke liye


