## 📌 C Programming - Fundamentals & Operators

### 🎯 Variables & Data Types in C 🔥

C me variables aur data types bina chai ke biscuit jaise hain! 🍪☕
Agar yeh nahi samjhe toh code likhna mushkil ho jayega. Chalo samajhte hain! 🚀

---

### 🏆 1️⃣ What are Variables? ⬇️

Variables ek container ki tarah hote hain jo memory me data store karte hain.
Jaise ghar me alag-alag dibbe me cheezein rakhi hoti hain, waise hi C me variables alag-alag type ke data rakhte hain! 😎

```c
int age = 18;  // Ek variable jo "age" store karega
```

👉 Yaha `age` ek variable hai jo `18` store kar raha hai.

---

### 🏆 2️⃣ Variable Declaration & Initialization ⬇️

🔹 **Declaration**: Batata hai ki konse type ka data store hoga.
🔹 **Initialization**: Variable me value assign karta hai.

```c
int number;     // Declaration
number = 25;    // Initialization

// Ek hi line me bhi kar sakte hain:
int number = 25;  // Declaration + Initialization
```

---

### 🏆 3️⃣ Data Types in C ⬇️

C me har variable ka ek data type hota hai, jo batata hai ki konse type ka data store hoga. 🔻

| Data Type | Size    | Example           |
| --------- | ------- | ----------------- |
| int       | 4 bytes | 100               |
| float     | 4 bytes | -3.2              |
| double    | 8 bytes | 15.789456         |
| char      | 1 byte  | 'A', 'z'          |
| void      | 0 bytes | Functions ke liye |

```c
int age = 20;
float price = 99.99;
char grade = 'A';
double pi = 3.14159;
```

---

### 🏆 4️⃣ sizeof() Operator ⬇️

Agar kisi data type ka size check karna ho toh `sizeof()` ka use hota hai:

```c
#include <stdio.h>

int main() {
    printf("Size of int: %lu bytes\n", sizeof(int));
    printf("Size of float: %lu bytes\n", sizeof(float));
    printf("Size of double: %lu bytes\n", sizeof(double));
    printf("Size of char: %lu bytes\n", sizeof(char));
    return 0;
}
```

👉 `sizeof()` batata hai ki koi bhi data type memory me kitni space leta hai! 🚀

---

### 🏆 5️⃣ printf() aur scanf() ⬇️

✅ `printf()` → Output dikhane ke liye
✅ `scanf()` → User se input lene ke liye

```c
#include <stdio.h>

int main() {
    int age;
    printf("Bhai apni umar batao: ");
    scanf("%d", &age);
    printf("Wah bhai! Tum %d saal ke ho! \n", age);
    return 0;
}
```

👉 `%d` integer ke liye, `%f` float ke liye, `%c` character ke liye use hota hai!

---

### ✅ Summary ⬇️

* **Variables** - Data store karne ke liye use hote hain
* **Declaration & Initialization** - Variable declare aur initialize karna zaroori hai
* **Data Types** - `int`, `float`, `char`, `double`, etc.
* **sizeof()** - Kisi bhi data type ka size check karne ke liye
* **printf() & scanf()** - Output aur user input ke liye

📢 Agar samajhne me dikkat ho, toh **KetanGPT** available hai! 😆💡
📞 Bas ek message maar, pura concept **tadka lagake** samjha denge! 🚀

---

### ✅ Coming Up Next:Practice karenge code ke sath! Let's go! 🚀
