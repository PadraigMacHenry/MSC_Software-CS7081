## Overview
Strings in Java are objects that represent sequences of characters. They are part of the `java.lang` package and are widely used for text manipulation.

---

## Declaring and Initializing Strings
```java
String yourName;
yourName = "John Lennon";
```

---

## Common String Methods
| Method                     | Description                                      | Example                          |
|----------------------------|--------------------------------------------------|----------------------------------|
| `charAt(int index)`        | Returns the character at the specified index.    | `yourName.charAt(0)`             |
| `length()`                 | Returns the length of the string.                | `yourName.length()`              |
| `toUpperCase()`            | Converts the string to uppercase.                | `yourName.toUpperCase()`         |
| `replace(char old, char new)` | Replaces occurrences of a character.          | `yourName.replace('a', '*')`     |
| `indexOf(char ch)`         | Returns the index of the first occurrence of `ch`. | `yourName.indexOf('n')`          |

---

## Example: String Operations
```java
public class StringExample {
    public static void main(String[] args) {
        String yourName = "Keyser Söze";

        // Print the string
        System.out.println("The input String: " + yourName);

        // Print the number of characters
        System.out.println("Number of characters: " + yourName.length());

        // Print the first and last characters
        System.out.println("First character: " + yourName.charAt(0));
        System.out.println("Last character: " + yourName.charAt(yourName.length() - 1));

        // Print the string in uppercase
        System.out.println("Uppercase: " + yourName.toUpperCase());

        // Replace 'a' with '*'
        System.out.println("Replaced 'a' with '*': " + yourName.replace('a', '*'));

        // Find the position of 'n'
        System.out.println("Position of 'n': " + yourName.indexOf('n'));
    }
}
```

**Output:**
```
The input String: Keyser Söze
Number of characters: 11
First character: K
Last character: e
Uppercase: Keyser Söze KEYSER SÖZE
Replaced 'ö' with '*': Keyser S*ze
Position of 'n': 4
```

---
## Keywords
#Java #Strings #StringMethods #TextManipulation #CharacterHandling
### [[Home Page]] | [[Week 1 Topic Summary]] | [[Decision Making with `if` Statements in Java]]

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]