
✅ **Relational Operators in C (==, !=, >, <, >=, <=)**

🔹 Relational operators ka use do values ko compare karne ke liye hota hai.
   Yeh hamesha **true (1)** ya **false (0)** return karte hain.


📌 **Relational Operators Table**

| Operator | Description           | Example      |
|----------|-----------------------|--------------|
| ==       | Equal to              | a == b       |
| !=       | Not equal to          | a != b       |
| >        | Greater than          | a > b        |
| <        | Less than             | a < b        |
| >=       | Greater than or equal | a >= b       |
| <=       | Less than or equal    | a <= b       |


----------------------------------------

🔹 **Example 1: Equal to (==) & Not Equal to (!=)**
```c

#include <stdio.h>

int main() {
    int a = 10, b = 20;

    printf("a == b : %d\n", a == b); // 0 (false)
    printf("a != b : %d\n", a != b); // 1 (true)

    return 0;
}

🔹 == →(Equal to) to → Yeh check karta hai ki dono values barabar hain ya nahi. 
      Agar barabar hain to 1 (true) return karega, nahi to 0 (false).

🔹 != → Not Equal to → Yeh check karta hai ki dono values alag hain ya nahi. 
      Agar alag hain to 1 (true) return karega, warna 0 (false). 
      
----------------------------------------


🔹 **Example 2: Greater than (>) & Less than (<)**

#include <stdio.h>
int main() {
    int x = 30, y = 25;

    printf("x > y : %d\n", x > y);  // 1 (true)
    printf("x < y : %d\n", x < y);  // 0 (false)

    return 0;
}

🔹 > → Greater than → Yeh check karega ki pehli value dusri se badi hai ya nahi. 
        Agar badi hai to 1 (true), nahi to 0 (false).

🔹 < → Less than → Yeh check karega ki pehli value dusri se chhoti hai ya nahi. 
        Agar chhoti hai to 1 (true), warna 0 (false).

----------------------------------------


🔹 **Example 3: Greater than or Equal to (>=) & Less than or Equal to (<=)**

#include <stdio.h>
int main() {
    int m = 50, n = 50;

    printf("m >= n : %d\n", m >= n); // 1 (true)
    printf("m <= n : %d\n", m <= n); // 1 (true)

    return 0;
}

🔹 >= → Greater than or Equal to → Yeh check karega ki pehli value dusri se badi
             ya barabar hai ya nahi. Agar haan, to 1 (true), warna 0 (false).

🔹 <= → Less than or Equal to → Yeh check karega ki pehli value dusri se chhoti 
         ya barabar hai ya nahi. Agar haan, to 1 (true), warna 0 (false).


----------------------------------------

🎯 **Relational Operators kaha use hote hain?**

✅ if statements → Condition check karne ke liye
✅ Loops (while/for) → Condition based iteration
✅ Sorting/Searching → Compare karne ke liye

