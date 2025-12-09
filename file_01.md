# 🚀 File 01: Your First C Program – "Hello, Ketan" 🌟

## 📘 Introduction

Aaj hum C ka sabse basic program likhne wale hain  
jo screen par `"Hello, Ketan"` print karega.  
Yeh har programmer ka **pehla kadam** hota hai.  
Is program ke saath hum **step-by-step code ko samjhenge bhi**. 🔥

---

## 🧑‍💻 Source Code – Hello World in C

```c
// First C Program - "Hello Ketan" 🚀

#include <stdio.h>  // Standard Input/Output header file

int main() {
    printf("Hello, Ketan\n");  // Screen par message print karega
    return 0;                  // Program successfully execute hua
}


📌 Step-by-Step Code Breakdown

1️⃣ #include <stdio.h>
🔹 Yeh ek preprocessor directive hai
🔹 stdio library include karta hai (Standard I/O)
🔹 Iske bina printf() kaam nahi karega


2️⃣ int main() { ... }
🔹 main() function har C program ka starting point hota hai
🔹 Program execution yahin se start hoti hai


3️⃣ printf("Hello, Ketan\n");
🔹 printf() ek output function hai
🔹 "Hello, Ketan" screen par print karega
🔹 \n – New Line Character (naye line me le jata hai)


4️⃣ return 0;
🔹 return 0; batata hai ki program successfully execute hua
🔹 Agar error hota toh koi aur value return karta


2️⃣ int main() me function calls
🔹 Humne alag-alag functions ko main() me call kiya
🔹 Yeh functions int return kar rahe hain, lekin humne return value store nahi ki (kyunki yeh sirf print kar rahe hain)


 
1️⃣ int hello1(); (Function Prototype)
🔹 Yeh compiler ko batata hai ki yeh function int return karega
🔹 Har function ka return type int hai, toh return statement likhna zaroori hai




✅ Recap (Memory Flash)

#include → tools laaye  
main() → entry gate  
printf() → bolne ka kaam  
\n → line todne ka kaam  
return 0 → kaam ho gaya bhai!
