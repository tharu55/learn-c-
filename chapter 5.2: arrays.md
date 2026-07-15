

## 1. Memory Address of an Array ⭐⭐⭐

Every element in an array has its own memory address.

The address of each element can be accessed using the **address-of operator (`&`)**.

### Example

```cpp
#include <iostream>
using namespace std;

int main()
{
    int marks[5] = {85, 90, 78, 88, 95};

    cout << &marks[0] << endl;
    cout << &marks[1] << endl;
    cout << &marks[2] << endl;

    return 0;
}
```

### Important Points

* Every element has a different memory address.
* The addresses are stored continuously.
* This concept is very important for learning **Pointers** later.

---

# 2. Array Size

The size of an array is the maximum number of elements it can store.

```cpp
int marks[5];
```

Here,

* Array Name = `marks`
* Size = **5**
* Valid Index = **0 to 4**

---

# 3. Array Length Using `sizeof()` ⭐⭐⭐

C++ provides the `sizeof()` operator to calculate the number of elements.

```cpp
int marks[] = {10,20,30,40,50};

int length = sizeof(marks) / sizeof(marks[0]);

cout << length;
```

### Output

```
5
```

### Why does this work?

* `sizeof(marks)` → Total size of the array in bytes.
* `sizeof(marks[0])` → Size of one element.
* Total size ÷ Size of one element = Number of elements.

---

# 4. Default Values

Default values depend on where the array is declared.

### Local Array

```cpp
int arr[5];
```

Values are **garbage values** (uninitialized).

---

### Global Array

```cpp
int arr[5];
```

Values are automatically initialized to **0**.

---

# 5. Types of Initialization ⭐⭐

### Complete Initialization

```cpp
int arr[5]={1,2,3,4,5};
```

---

### Partial Initialization

```cpp
int arr[5]={10,20};
```

Remaining elements become **0**.

Output

```
10 20 0 0 0
```

---

### Size Automatically Decided

```cpp
int arr[]={1,2,3,4,5};
```

Compiler counts the elements automatically.

---

# 6. Array Traversal

Traversal means visiting every element of an array one by one.

Traversal is usually done using:

* for loop
* while loop
* do-while loop

---

# 7. Searching in an Array

Searching means finding whether a value exists in an array.

Example:

```
Array:
10 20 30 40 50

Search:
30

Result:
Found
```

---

# 8. Updating Array Elements

Array values can be changed.

```cpp
marks[2]=100;
```

Now

```
85 90 100 88 95
```

---

# 9. Copying Arrays

In C++, one array cannot be directly assigned to another.

Wrong

```cpp
arr2 = arr1;
```

Instead, copy each element using a loop.

---

# 10. Passing Arrays to Functions

Arrays can be passed as function parameters.

Example

```cpp
void display(int arr[], int size)
```

This topic becomes important when learning **Functions**.

---

# 11. Out-of-Bounds Access ⭐⭐⭐

This is one of the most important concepts.

Example

```cpp
marks[10];
```

If the array size is 5,

this index is **invalid**.

Possible problems:

* Garbage value
* Wrong output
* Program crash
* Undefined Behaviour

---

# 12. Difference Between Array and Variable

| Variable               | Array                     |
| ---------------------- | ------------------------- |
| Stores one value       | Stores multiple values    |
| One memory location    | Multiple memory locations |
| One name for one value | One name for many values  |

---

# 13. Where Arrays Are Used

Arrays are used in:

* Student management systems
* Banking applications
* Hospital management
* Image processing
* Games
* Search engines
* Artificial Intelligence
* Machine Learning
* Data Structures
* Operating Systems

---

# 14. Limitations of Arrays

* Fixed size
* Same data type only
* Difficult to insert/delete elements
* Memory may be wasted
* No automatic resizing

---


