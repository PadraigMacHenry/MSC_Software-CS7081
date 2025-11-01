## Overview
Variables are containers for storing data values in Java. They must be declared with a specific type and can hold values of that type only.

---

## Declaring Variables
Variables must be declared before use. The syntax is:
```java
dataType variableName;
```
**Example:**
```java
int age;
double price;
char grade;
boolean isActive;
String name;
```

---

## Variable Naming Rules
- **No reserved words** (e.g., `int`, `class`).
- **Cannot start with a digit** (e.g., `int 1age;` is invalid).
- **Can start with a letter, underscore (`_`), or dollar sign (`$`)**.
- **Use camelCase** for readability (e.g., `bookPrice`).
- **Avoid spaces or special characters** (e.g., `book price` or `book@price` is invalid).

---

## Primitive Data Types
Java has 8 primitive data types:

| Type      | Description                                      | Example               | Default Value |
|-----------|--------------------------------------------------|-----------------------|---------------|
| `byte`    | 8-bit integer                                    | `byte myByte = 16;`   | 0             |
| `short`   | 16-bit integer                                   | `short myShort = 128;`| 0             |
| `int`     | 32-bit integer                                   | `int myInt = 345678;` | 0             |
| `long`    | 64-bit integer                                   | `long myLong = 34567834L;` | 0L        |
| `float`   | 32-bit floating-point number                     | `float myFloat = 3.14728f;` | 0.0f      |
| `double`  | 64-bit floating-point number                     | `double myDouble = 3.12347;` | 0.0       |
| `char`    | 16-bit Unicode character                         | `char myChar = 'a';`  | '\u0000'     |
| `boolean` | `true` or `false`                                | `boolean myBool = true;` | `false`   |

---

## Reference Data Types
- **String** is a reference type and stores sequences of characters.
- **Example:**
  ```java
  String myString = "Padraig McH";
  System.out.printf("My name is: %s\n", myString);
  ```

---

## Initializing Variables
Variables can be initialized at declaration or later:
```java
int sideLength = 6; // Declaring and initializing
double radius;
radius = 9.0; // Initializing later
```

---

## Example: Storing Name and Age
```java
public class DataStorageExample {
    public static void main(String[] args) {
        String name = "Padraig";
        int age = 25;
        System.out.printf("My name is %s. My age is %d\n", name, age);
    }
}
```
**Output:**
```
My name is Padraig. My age is 25
```

---

## Key Points
- Variables must be declared with a type.
- Primitive types store simple values; reference types store objects.
- Always use meaningful variable names for clarity.

---
## Keywords
#Java #Variables #DataTypes #PrimitiveTypes #ReferenceTypes #CodingBestPractices
### [[Home Page]] | [[Week 1 Topic Summary]] |  [[Operators in Java]] 

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]