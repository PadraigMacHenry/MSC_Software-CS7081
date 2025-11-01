## Overview
The `if` statement in Java allows the program to execute a block of code conditionally, based on whether a specified condition is `true` or `false`.

---

## Equality and Relational Operators
| Operator | Description               | Example          |
|----------|---------------------------|------------------|
| `==`     | Equal to                  | `num1 == num2`   |
| `!=`     | Not equal to              | `num1 != num2`   |
| `>`      | Greater than              | `num1 > num2`    |
| `<`      | Less than                 | `num1 < num2`    |
| `>=`     | Greater than or equal to  | `num1 >= num2`   |
| `<=`     | Less than or equal to     | `num1 <= num2`   |

---

## Example: Comparing Two Numbers
```java
public class IfStatementExample {
    public static void main(String[] args) {
        int number1 = 3;
        int number2 = 10;

        System.out.println("Numbers to compare: " + number1 + " and " + number2);

        if (number1 > number2) {
            System.out.println("Biggest number: " + number1);
        } else if (number2 > number1) {
            System.out.println("Biggest number: " + number2);
        } else {
            System.out.println("Numbers are the same");
        }
    }
}
```

**Output:**
```
Numbers to compare: 3 and 10
Biggest number: 10
```

---

## Example: Handling Equal Numbers
```java
public class IfElseExample {
    public static void main(String[] args) {
        int number1 = 44;
        int number2 = 44;

        System.out.println("Numbers to compare: " + number1 + " and " + number2);

        if (number1 > number2) {
            System.out.println("Biggest number: " + number1);
        } else if (number2 > number1) {
            System.out.println("Biggest number: " + number2);
        } else {
            System.out.println("Numbers are the same");
        }
    }
}
```

**Output:**
```
Numbers to compare: 44 and 44
Numbers are the same
```

---
## Key Points
- Use `if`, `else if`, and `else` to control program flow based on conditions.
- Equality and relational operators (`==`, `!=`, `>`, `<`, `>=`, `<=`) are used to form conditions.
- Always ensure conditions are mutually exclusive and cover all possible cases.

---
## Keywords
#Java #IfStatements #Conditionals #EqualityOperators #RelationalOperators #DecisionMaking

### [[Home Page]] | [[Week 1 Topic Summary]] | [[Week 2 Topic Summary]]

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]
