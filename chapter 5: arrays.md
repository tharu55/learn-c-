# 📘 Arrays in C++

## Introduction

Sometimes we need to store many values in a program. If we create a separate variable for each value, the program becomes long and difficult to manage.

To solve this problem, C++ provides **arrays**.

An array lets us store **many values of the same data type** in **one variable**.

---

# Definition

An **array** is a variable that stores **more than one value** of the **same data type**.

Instead of creating many variables, we create **one array**.

---

# Why Do We Use Arrays?

Suppose you want to store the marks of 5 students.

Without an array, you need five variables.

```cpp
int mark1 = 85;
int mark2 = 90;
int mark3 = 78;
int mark4 = 88;
int mark5 = 95;
```

This works, but if there are 100 students, you need 100 variables.

Using an array, all the marks can be stored in one variable.

```cpp
int marks[5] = {85, 90, 78, 88, 95};
```

Now the program is shorter and easier to understand.

---

# Advantages of Arrays

* Store many values in one variable.
* Reduce the number of variables.
* Make programs easier to write.
* Work well with loops.
* Save time when writing code.

---

# Array Declaration

Before using an array, we must declare it.

### Syntax

```cpp
data_type array_name[size];
```

### Example

```cpp
int marks[5];
```

Here,

* `int` → data type
* `marks` → array name
* `5` → number of values the array can store

---

# Array Initialization

Initialization means giving values to an array.

```cpp
int marks[5] = {85, 90, 78, 88, 95};
```

Now the array contains five values.

---

# Array Index

Every value in an array has a position.

This position is called the **index**.

The index always starts from **0**.

| Index | Value |
| ----: | ----: |
|     0 |    85 |
|     1 |    90 |
|     2 |    78 |
|     3 |    88 |
|     4 |    95 |

For an array of size **5**, the index goes from **0 to 4**.

---

# Accessing Array Elements

To get a value from an array, we use its index.

Example:

```cpp
cout << marks[0];
```

Output

```
85
```

`marks[0]` gives the first value of the array.

---

# Printing All Array Elements

Instead of printing each value one by one, we use a loop.

```cpp
for(int i = 0; i < 5; i++)
{
    cout << marks[i] << " ";
}
```

