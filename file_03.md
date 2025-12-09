# 🟢 C Program Structure and Syntax - Full Breakdown  

Agar C language ko achhe se samajhna hai, toh iska **structure aur syntax** samajhna zaroori hai.  
Yeh C ka skeleton hai, jo har program me follow hota hai.  

Toh chalo ekdum professional tareeke se samajhte hain! 💡🔥

---

## ✅ 1️⃣ Basic Structure of a C Program

Har C program ek basic structure follow karta hai, jo 3 major parts me divide hota hai:

1. 🧩 Header Files (`#include`)
2. 🧠 Main Function (`int main()`)
3. 🎯 Return Statement (`return 0;`)

---

## 🚀 Example Code – Basic Structure of a C Program

```c
#include <stdio.h>  // 1️⃣ Header file (Input/Output ke liye)

int main() {        // 2️⃣ Main function (C ka entry point)
    printf("hello world!\n");  // Output print karega
    return 0;       // 3️⃣ Program successful run hone par 0 return karega
}


📌 Breakdown (Structure)

1️⃣ #include <stdio.h>
🔹 Standard library ko include karta hai – printf(), scanf() jese functions ke liye zaroori hai.

2️⃣ int main()
🔹 C program ka entry point, yahan se execution start hoti hai.

3️⃣ { ... }
🔹 Curly brackets function ka body define karti hain

4️⃣ printf("Hello, World!\n");
🔹 Screen par output print karega

5️⃣ return 0;
🔹 Program successfully run hone par 0 return karega



✅ 2️⃣ Header Files – #include

C me predefined functions hoti hain jo header files me stored hoti hain.
Inko #include keyword se program me include karte hain.

## 🚀 Common Header Files

C language me header files predefined libraries ko include karne ke kaam aati hain.  
Yeh kuch commonly used header files aur unka use case:

| 📁 **Header File**       | ⚙️ **Use Case**                                                 |
|--------------------------|------------------------------------------------------------------|
| `#include <stdio.h>`     | Standard I/O (e.g., `printf()`, `scanf())
                      |
| `#include <math.h>`      | Math functions (e.g., `sqrt()`, `pow())`                        |
| `#include <string.h>`    | String handling (e.g., `strlen()`, `strcpy())`                  |
| `#include <stdlib.h>`    | Memory allocation & conversion (e.g., `malloc()`, atoi())
     


## ✅ 3️⃣ Main Function – `int main()`

C program ka execution **hamesha `main()`** se start hota hai.  

🔹 **2 tarike hote hain main() likhne ke:**

### 1️⃣ With Return Type (✅ Recommended)

int main() {
    return 0;
}

## 2️⃣ Without Return Type – ⚠️ Not Recommended

void main() {
    // Warning de sakta hai
}

🔹 void main() technically kaam karta hai, lekin modern C standards (C99 aur baad me) me ye recommended nahi hai.

🔹 Always use int main() for best practice. 🚀



✅ 4️⃣ Return Statement – return 0;

return 0; ka matlab hota hai ki program successfully execute hua.
Agar program me koi error hota toh return 1; ya return -1; likha jata.

🚀 Example Code:

int main() {
    printf("Program is running!\n");
    return 0;  // Success return karega
}




