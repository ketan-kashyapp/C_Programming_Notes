# Unit 4: Functions in C (Exam Oriented Notes)

Functions are a block of code designed to perform a particular task. Using functions makes the program modular, easier to read, and reduces code repetition.

## ✅ Introduction

* Functions divide a program into smaller modules.
* Helps in reusability of code and better organization.

## ✅ Types of Functions

1️⃣ **Built-in Functions:** Provided by C standard library (e.g., `printf()`, `scanf()`).
2️⃣ **User-defined Functions:** Created by the programmer to perform specific tasks.

## ✅ Functions with Array

* Arrays can be passed to functions to manipulate multiple data elements at once.

```c
void printArray(int arr[], int n) {
    for(int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
}
```

## ✅ Passing Parameters to Functions

### 1️⃣ Call by Value

* Copies the value of an argument into the function parameter.
* Changes inside the function do **not** affect the original variable.

```c
void square(int x) {
    x = x * x;
}
```

### 2️⃣ Call by Reference

* Passes the address of a variable to the function.
* Changes inside the function affect the original variable.

```c
void square(int *x) {
    *x = (*x) * (*x);
}
```

### 3️⃣ Passing Arrays to Functions

* Arrays are always passed by reference in C.
* The function can modify array elements directly.

```c
void modifyArray(int arr[], int n) {
    for(int i = 0; i < n; i++) {
        arr[i] = arr[i] + 1;
    }
}
```

## ✅ Recursive Functions

* A function that calls itself directly or indirectly.
* Used to solve problems that can be broken into smaller sub-problems.

```c
int factorial(int n) {
    if(n == 0) return 1;
    else return n * factorial(n - 1);
}
```

🧠 Explanation:
Recursive function continues calling itself until the base condition is met. Example above calculates factorial of a number.
