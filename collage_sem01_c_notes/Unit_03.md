# Unit 3: Arrays, Structures, and Basic Searching & Sorting 

## ✅ Arrays in C

Arrays are used to store multiple values of the same type in a single variable.

### 1️⃣ Array Notation and Representation

✅ Syntax:

```c
data_type array_name[size];
```

Example:

```c
int arr[5]; // Array of 5 integers
```

### 2️⃣ Manipulating Array Elements

* Access using index: `arr[0]`, `arr[1]`, ...
* Assign values: `arr[0] = 10;`
* Loop through array to read/write elements

```c
for(int i = 0; i < 5; i++) {
    arr[i] = i * 2;
}
```

### 3️⃣ Multi-Dimensional Arrays

✅ Syntax:

```c
data_type array_name[rows][columns];
```

Example:

```c
int matrix[2][3] = {{1,2,3},{4,5,6}};
```

### 4️⃣ Character Arrays and Strings

* String is a character array ending with `\0`

```c
char str[10] = "Hello";
```

* Access individual characters: `str[0]`, `str[1]`...

## ✅ Structures in C

Structure allows grouping different data types under a single name.

✅ Syntax:

```c
struct structure_name {
    data_type member1;
    data_type member2;
    ...
};
```

Example:

```c
struct Student {
    char name[20];
    int age;
};
```

## ✅ Union in C

* Similar to structure but shares the same memory location for all members.

```c
union Data {
    int i;
    float f;
    char str[20];
};
```

## ✅ Enumerated Data Types

* Used to define named integer constants

```c
enum Week {Mon, Tue, Wed, Thu, Fri, Sat, Sun};
```

## ✅ Array of Structures

* Array can store multiple structure variables

```c
struct Student arr[5];
```

## ✅ Basic Searching Algorithms

### 1️⃣ Linear Search

* Search elements sequentially until found.

```c
int linearSearch(int arr[], int n, int key) {
    for(int i = 0; i < n; i++) {
        if(arr[i] == key) return i;
    }
    return -1;
}
```

## ✅ Basic Sorting Algorithms

### 1️⃣ Bubble Sort

* Compare adjacent elements and swap if out of order.

```c
void bubbleSort(int arr[], int n) {
    for(int i = 0; i < n-1; i++) {
        for(int j = 0; j < n-i-1; j++) {
            if(arr[j] > arr[j+1]) {
                int temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }
        }
    }
}
```

🧠 Explanation:
Bubble Sort repeatedly moves the largest element to the end in each pass.
