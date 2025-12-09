# ⚙️ File 02: Functions in C – Understanding `int` Return Type 🔄

## 📘 Introduction

Is program me hum `int` return type ke functions use karke "Hello, World!" style ka modular code likh rahe hain.  
Saath hi `void` vs `int` functions ka breakdown bhi dekhenge — real-life relatable tarike se. 🧠

---

## 🧾 Source Code – `int` Return Type with Function

```c
// "Hello, World!" using int return type in functions

#include <stdio.h>

// Function Prototypes (Yeh batate hain ki neeche yeh functions define honge)
int hello1();   // Function prototype

int main() {
    printf("Hello, I am Ketan Kashyap\n");  // Main function ka message

    // Calling other function
    hello1();  // Function call

    return 0;  // Program successfully executed
}

// Function Definition
int hello1() {
    printf("I am a b.tech student\n");  // Function ka output
    return 0;  // Returning integer value
}


## 🔍 Code Breakdown


### 1️⃣ `int hello1();` – Function Prototype  

⚙️ Compiler ko batata hai ki yeh ek function hai jo `int` return karega  
⚠️ Agar return type define nahi kiya, to error ya warning aa sakti hai  

---

### 2️⃣ Function Call in `main()`  

✨ Hum `main()` function ke andar `hello1()` ko call karte hain  
⚠️ Return value use nahi ki, kyunki hum sirf print kar rahe hain  

---

### 3️⃣ Function ke andar Return

🔁 Har function `int` return karta hai  

📌 Abhi return value ka use nahi kiya, but sikha ki yeh kaise kaam karta hai 



⚔️ Comparison – void vs int Functions

☑️ void Functions

🔹 Koi return value nahi dete
🔹 Sirf kaam karte hain (like print karna)
🔹 Return likhne ki zaroorat nahi, likha to error


☑️ int Functions

🔹 Integer value return karte hain
🔹 return likhna mandatory hai
🔹 Return value ko store karke use bhi kiya ja sakta hai

