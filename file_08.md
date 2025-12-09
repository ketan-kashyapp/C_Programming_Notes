# 🚀 Task 3: `sizeof()` se Size Check Karna!

Ek simple C program jo `int`, `float`, `double`, aur `char` ka size check karega using `sizeof()` operator.

---

## 📄 Code:

```c
#include <stdio.h>

int main() {
   printf("Size of int: %u bytes\n", sizeof(int));
   printf("Size of float: %u bytes\n", sizeof(float));
   printf("Size of double: %u bytes\n", sizeof(double));
   printf("Size of char: %u bytes\n", sizeof(char));
   return 0;
}


🔍 Output Example:

Size of int: 4 bytes
Size of float: 4 bytes
Size of double: 8 bytes
Size of char: 1 bytes


📌 sizeof Direct Data Types ke Saath:

printf("Size of int: %lu bytes\n", sizeof(int));
printf("Size of float: %lu bytes\n", sizeof(float));

✅ Jab kisi variable ka naam nahi ho, tab bhi direct data type use karke size check kiya ja sakta hai.


📌 Array ke Size kaise Pata Karein:

int arr[5];
printf("Size of array: %lu bytes\n", sizeof(arr));
printf("Number of elements in array: %lu\n", sizeof(arr) / sizeof(arr[0]));

✅ Total array ka size aur uske elements ki count nikalne me help karta hai.


📌 sizeof Pointer ke Saath:

int *p;
printf("Size of pointer: %lu bytes\n", sizeof(p));

✅ Pointer ka size architecture par depend karta hai (32-bit = 4 bytes, 64-bit = 8 bytes).


💡 Pro Tip: Always use %lu instead of %u with sizeof() for better portability!


