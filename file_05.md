# 🔥 C Program Structure + Function + Variable + Output Breakdown in C

---

## ✅ Full Example Code

```c
// Function prototype
int sum(int a, int b);

int main() {
    // Variables declaration and initialization
    int num1 = 10;
    float num2 = 20.5;
    char letter = 'A';

    // Printing program structure
    printf("🔥 C Program Structure 🔥\n");
    printf("-------------------------\n");
    printf("1️⃣ #include <stdio.h>\n");
    printf("2️⃣ int main() {\n");
    printf("3️⃣    // Variables\n");
    printf("4️⃣    // Function Call\n");
    printf("5️⃣    return 0;\n");
    printf("6️⃣ }\n\n");

    // Printing variables
    printf("Integer Variable: %d\n", num1);
    printf("Float Variable: %.2f\n", num2);
    printf("Character Variable: %c\n", letter);

    // Function call
    int result = sum(num1, (int)num2);
    printf("Sum of %d and %d is: %d\n", num1, (int)num2, result);

    return 0;
}

// Function definition
int sum(int a, int b) 
{
    return a + b;
}


📌 Code Breakdown 🚀

🛠️ Step 1: Header File

#include <stdio.h>
✅ Standard I/O library ko include karta hai.

✅ printf() aur scanf() jaise functions use karne ke liye zaroori hota hai.


🛠️ Step 2: Function Prototype

int sum(int a, int b);
✅ Batata hai ki sum() function exist karta hai.

✅ 2 integers leta hai aur ek integer return karta hai.


🛠️ Step 3: main() Function Start

int main()
✅ C program ka entry point.

✅ Yahan se execution start hota hai.


### 🛠️ Step 4: Variables Declaration

```c
int num1 = 10;
float num2 = 20.5;
char letter = 'A';

### 📦 Variable Details Chart
+---------+--------+--------+------------------+
| Variable| Type | Value | Description |
+---------+--------+--------+------------------+
| num1 | int | 10 | Integer value |
| num2 | float | 20.5 | Decimal value |
| letter | char | 'A' | Character value |
+---------+--------+--------+------------------+


🛠️ Step 5: Print Program Structure

printf("🔥 C Program Structure 🔥\n");
printf("-------------------------\n");
printf("1️⃣ #include <stdio.h>\n");
printf("2️⃣ int main() {\n");
printf("3️⃣    // Variables\n");
printf("4️⃣    // Function Call\n");
printf("5️⃣    return 0;\n");
printf("6️⃣ }\n\n");

✅ Ye structure sirf samajhne ke liye print hota hai.
✅ Help karta hai visualise karne me C program ka structure.

🖥️ Output:

🔥 C Program Structure 🔥
-------------------------
1️⃣ #include <stdio.h>
2️⃣ int main() {
3️⃣    // Variables
4️⃣    // Function Call
5️⃣    return 0;
6️⃣ }


🛠️ Step 6: Print Variables

printf("Integer Variable: %d\n", num1);
printf("Float Variable: %.2f\n", num2);
printf("Character Variable: %c\n", letter);

✅ %d — prints integer
✅ %.2f — prints float with 2 decimal places
✅ %c — prints character

🖥️ Output:

Integer Variable: 10
Float Variable: 20.50
Character Variable: A


🛠️ Step 7: Function Call

int result = sum(num1, (int)num2);
printf("Sum of %d and %d is: %d\n", num1, (int)num2, result);

✅ num2 float hai, lekin sum() int leta hai → (int)num2 se typecast
✅ Result ko variable result me store karke print kiya

🖥️ Output:

Sum of 10 and 20 is: 30

🛠️ Step 8: Function Definition

int sum(int a, int b) {
    return a + b;
}

✅ 2 integers ka sum return karta hai
✅ return a + b; — add karke output return


🔚 Final Output

🔥 C Program Structure 🔥
-------------------------
1️⃣ #include <stdio.h>
2️⃣ int main() {
3️⃣    // Variables
4️⃣    // Function Call
5️⃣    return 0;
6️⃣ }

Integer Variable: 10
Float Variable: 20.50
Character Variable: A
Sum of 10 and 20 is: 30


 