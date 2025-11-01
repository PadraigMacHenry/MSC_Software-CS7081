## Overview
Operators in Java are symbols that perform operations on variables and values. They are fundamental for manipulating data and controlling program flow.

---

## Arithmetic Operators
Used for basic mathematical operations:

| Operator | Name           | Example      | Description                     |
|----------|----------------|--------------|---------------------------------|
| `+`      | Addition       | `a + b`      | Adds two values                 |
| `-`      | Subtraction    | `a - b`      | Subtracts two values            |
| `*`      | Multiplication | `a * b`      | Multiplies two values           |
| `/`      | Division       | `a / b`      | Divides two values              |
| `%`      | Modulus        | `a % b`      | Returns the division remainder  |

**Example:**
```java
int num1 = 4;
int num2 = 7;
int answer = num1 + num2; // Addition
System.out.println("Answer is: " + answer);
```

**Output:**
```
Answer is: 11
```

---

## Assignment Operator
The `=` operator assigns a value to a variable.

```java
int result = 0;
result = 1 + 2; // result is now 3
result = result - 1; // result is now 2
result = result * 2; // result is now 4
result = result / 2; // result is now 2
result = result + 8; // result is now 10
result = result % 7; // result is now 3
System.out.println(result);
```

**Output:**
```
3
```

---

## Casting
Casting explicitly converts one data type to another. It is useful when precision needs to be preserved.

**Example:**
```java
int num1 = 6;
int num2 = 4;
double answer = (double) num1 / num2; // Casting to double
System.out.println(answer); // Outputs 1.5
```

Without casting:
```java
double answer = num1 / num2; // Outputs 1.0
```

---

## Expressions
An expression is a combination of variables, values, operators, and method calls that produce a result.

**Example:**
```java
int result = 0;
result = 1 + 2 * 3; // Multiplication performed first
System.out.println(result); // Outputs 7
```

---

## Key Points
- Operators perform operations on variables and values.
- Arithmetic operators include `+`, `-`, `*`, `/`, and `%`.
- Casting is used to convert data types explicitly.
- Expressions combine variables, values, operators, and method calls to produce a result.

---
## Keywords
#Java #Operators #ArithmeticOperators #Casting #Expressions #DataManipulation

### [[Home Page]] | [[Week 1 Topic Summary]] |  [[Strings in Java]]

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]