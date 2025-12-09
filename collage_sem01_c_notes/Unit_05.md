# Unit 5: Pointers in C (Exam Oriented Notes)

Pointers are variables that store the **address of another variable**. They are powerful tools in C for memory management and efficient programming.

## ✅ Declarations

* To declare a pointer, use the `*` symbol.

```c
int *ptr;  // pointer to an integer
float *fptr; // pointer to a float
```

* Assign address to a pointer using `&`.

```c
int x = 10;
int *ptr = &x;
```

## ✅ Passing Pointers to Functions

* Enables functions to modify the original variable.

```c
#include <stdio.h>
void increment(int *p) {
    (*p)++;
}
int main() {
    int a = 5;
    increment(&a);
    printf("%d", a); // Output: 6
    return 0;
}
```

## ✅ Operations on Pointers

* **Dereferencing:** Access the value at the address stored in a pointer.

```c
int x = 10;
int *ptr = &x;
printf("%d", *ptr); // prints 10
```

* **Pointer arithmetic:** You can increment/decrement pointers.

```c
ptr++; // moves to next memory location of the type
```

## ✅ Pointer Arrays

* Array of pointers stores addresses of variables.

```c
int a = 5, b = 10;
int *arr[2];
arr[0] = &a;
arr[1] = &b;
```

## ✅ Arrays of Pointers

* Can point to multiple arrays or strings.

```c
char *names[] = {"Alice", "Bob", "Charlie"};
printf("%s", names[1]); // prints Bob
```

## ✅ Structures and Pointers

* Pointers can point to structures and access members using `->` operator.

```c
#include <stdio.h>
struct Student {
    char name[20];
    int age;
};
int main() {
    struct Student s = {"John", 20};
    struct Student *ptr = &s;
    printf("Name: %s, Age: %d", ptr->name, ptr->age);
    return 0;
}
```

🧠 Explanation:
Pointers store addresses and allow direct memory manipulation. They are used with functions, arrays, and structures for efficient programming.

