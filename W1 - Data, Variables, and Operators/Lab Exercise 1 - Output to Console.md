This exercise focuses on using escape sequences (`\n` for newline and `\t` for tab) to format console output in Java.

---

## Task
Modify the `HelloWorld` program to produce the following output:

```
Hello World! I am alive
Hello World! I am alive
I can write on two lines!

        *
       ***
      *****
     *******
    *********
Happy Christmas
Macbeth

First Witch	When shall we three meet again?
		In thunder, lightning, or in rain?
Second Witch	When the hurlyburly's done,
		When the battle's lost and won.
Third Witch	That will be ere the set of sun
```

---

## Solution
```java
public class HelloWorld {
    public static void main(String[] args) {
        // Adding more text to the line
        System.out.println("Hello World! I am alive");

        // Adding a new line
        System.out.println("Hello World! I am alive");
        System.out.println("I can write on two lines!\n");

        // Adding a blank line and multiple lines
        System.out.println("        *");
        System.out.println("       ***");
        System.out.println("      *****");
        System.out.println("     *******");
        System.out.println("    *********\n");

        // Using tab character
        System.out.println("Happy Christmas");
        System.out.println("Macbeth\n");

        // Formatting with tabs
        System.out.println("First Witch\tWhen shall we three meet again?");
        System.out.println("\t\tIn thunder, lightning, or in rain?");
        System.out.println("Second Witch\tWhen the hurlyburly's done,");
        System.out.println("\t\tWhen the battle's lost and won.");
        System.out.println("Third Witch\tThat will be ere the set of sun");
    }
}
```

---
## Keywords
#Java #ConsoleOutput #EscapeSequences #LabExercise
### [[Home Page]] | [[Week 1 Topic Summary]] | [[Week 2 Topic Summary]]

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]