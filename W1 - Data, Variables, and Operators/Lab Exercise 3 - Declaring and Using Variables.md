
This exercise covers declaring variables of primitive types (`int` and `double`) and performing calculations.

---

## Task 1: Square Area
Write a program that declares the length of a side of a square as an `int` and calculates its area.

---
### Solution
```java
public class SquareArea {
    public static void main(String[] args) {
        // Declare and initialize the side length
        int sideLength = 6;

        // Calculate and print the area
        int area = sideLength * sideLength;
        System.out.println("The area of the square is: " + area);
    }
}
```

---

## Task 2: Circle Area
Write a program that declares the radius of a circle as a `double` and calculates its area (to three decimal places).

---
### Solution
```java
public class CircleArea {
    public static void main(String[] args) {
        // Declare and initialize the radius
        double radius = 9.0;
        final double PI = 3.142; // Use final for constants

        // Calculate and print the area
        double area = PI * radius * radius;
        System.out.printf("The area of the circle is: %.3f", area);
    }
}
```

---
## Keywords
#Java #Variables #PrimitiveTypes #LabExercise
### [[Home Page]] | [[Week 1 Topic Summary]] | [[Week 2 Topic Summary]]

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]