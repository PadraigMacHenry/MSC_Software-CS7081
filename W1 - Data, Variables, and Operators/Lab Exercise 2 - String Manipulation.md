This exercise explores common string operations in Java, such as extracting characters, converting case, and replacing text.

---

## Task
Write a Java program that:
1. Declares a `String` and assigns your name to it.
2. Prints the string.
3. Prints the number of characters in the string.
4. Prints the first and last characters.
5. Prints the string in uppercase.
6. Replaces all occurrences of a specific letter (e.g., 'a') with `*`.
7. Prints the position of the first occurrence of the character 'n'.

---

## Solution
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

---
## Keywords
#Java #Strings #StringMethods #LabExercise
### [[Home Page]] | [[Week 1 Topic Summary]] | [[Week 2 Topic Summary]]

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]