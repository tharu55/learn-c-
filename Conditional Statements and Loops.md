# 📘 C++ Notes

# Conditional Statements and Loops

---

# 1. Conditional Statements

## Definition

A **conditional statement** is used to make decisions in a program.

It checks whether a condition is **true** or **false**. Based on the result, the program decides which block of code to execute.

**Simple Definition:**

> A conditional statement allows the program to make decisions.

---

## Why do we use Conditional Statements?

We use conditional statements when a program needs to choose between different actions.

### Examples

* Check if a person is eligible to vote.
* Find the largest number.
* Check whether a number is even or odd.
* Display a grade based on marks.

---

# Types of Conditional Statements

1. `if`
2. `if-else`
3. `else if` Ladder
4. Nested `if`
5. `switch`
6. Ternary Operator (`?:`)

---

# 1. if Statement

## Definition

The **if statement** executes a block of code **only if the condition is true**.

If the condition is false, the program skips that block.

### Syntax

```cpp
if(condition)
{
    // code
}
```

### Example

```cpp
#include <iostream>
using namespace std;

int main() {

    int age = 20;

    if(age >= 18)
    {
        cout << "You can vote.";
    }

    return 0;
}
```

### Output

```
You can vote.
```

### Explanation

* `age >= 18` is the condition.
* Since age is 20, the condition is true.
* The code inside the `if` block executes.

---

# 2. if-else Statement

## Definition

The **if-else statement** is used when there are **two possible choices**.

* If the condition is true → `if` block executes.
* If the condition is false → `else` block executes.

### Syntax

```cpp
if(condition)
{
    // code if true
}
else
{
    // code if false
}
```

### Example

```cpp
#include <iostream>
using namespace std;

int main() {

    int age = 16;

    if(age >= 18)
    {
        cout << "Eligible to vote";
    }
    else
    {
        cout << "Not eligible to vote";
    }

    return 0;
}
```

### Output

```
Not eligible to vote
```

---

# 3. else if Ladder

## Definition

The **else if ladder** is used when there are **more than two conditions**.

The program checks the conditions **from top to bottom**.

As soon as one condition becomes true, its block executes and the remaining conditions are skipped.

### Syntax

```cpp
if(condition1)
{
    // code
}
else if(condition2)
{
    // code
}
else
{
    // code
}
```

### Example

```cpp
#include <iostream>
using namespace std;

int main() {

    int marks = 82;

    if(marks >= 90)
    {
        cout << "Grade A";
    }
    else if(marks >= 75)
    {
        cout << "Grade B";
    }
    else if(marks >= 50)
    {
        cout << "Grade C";
    }
    else
    {
        cout << "Fail";
    }

    return 0;
}
```

### Output

```
Grade B
```

---

# 4. Nested if

## Definition

A **Nested if** means writing an `if` statement inside another `if` statement.

It is used when one condition should be checked only after another condition is true.

### Example

```cpp
#include <iostream>
using namespace std;

int main() {

    int age = 20;
    bool hasLicense = true;

    if(age >= 18)
    {
        if(hasLicense)
        {
            cout << "You can drive.";
        }
    }

    return 0;
}
```

### Output

```
You can drive.
```

---

# 5. switch Statement

## Definition

A **switch statement** is used when one variable has many fixed values.

It is often simpler than writing many `else if` statements.

### Syntax

```cpp
switch(variable)
{
    case value:
        // code
        break;

    default:
        // code
}
```

### Example

```cpp
#include <iostream>
using namespace std;

int main() {

    int day = 3;

    switch(day)
    {
        case 1:
            cout << "Monday";
            break;

        case 2:
            cout << "Tuesday";
            break;

        case 3:
            cout << "Wednesday";
            break;

        default:
            cout << "Invalid Day";
    }

    return 0;
}
```

### Output

```
Wednesday
```

---

# 6. Ternary Operator

## Definition

The **ternary operator** is a short form of the `if-else` statement.

### Syntax

```cpp
(condition) ? true_statement : false_statement;
```

### Example

```cpp
#include <iostream>
using namespace std;

int main() {

    int age = 20;

    (age >= 18) ? cout << "Adult" : cout << "Minor";

    return 0;
}
```

### Output

```
Adult
```

---

# What is a Loop?

## Definition

A **loop** is used to execute the same block of code **again and again** until a condition becomes false.

**Simple Definition:**

> A loop repeats a task multiple times.

---

## Why do we use Loops?

Instead of writing the same code many times, we use loops.

### Example

Without a loop:

```cpp
cout << "Hello";
cout << "Hello";
cout << "Hello";
cout << "Hello";
cout << "Hello";
```

With a loop:

```cpp
for(int i = 1; i <= 5; i++)
{
    cout << "Hello\n";
}
```

---

 
