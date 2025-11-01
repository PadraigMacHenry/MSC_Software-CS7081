## Overview
Fall-through is a behavior in Java `switch` statements where execution continues from a matching `case` label to all subsequent `case` blocks until a `break` statement or the end of the `switch` block is encountered.

---

## How It Works
1. The `switch` statement evaluates the expression **once** at the start.
2. It jumps to the matching `case` label and executes its code.
3. **Without a `break` statement**, execution "falls through" to the next `case` block, regardless of whether the next `case` matches the expression's value.
4. Fall-through continues until a `break` statement or the end of the `switch` block is reached.

---

## Example
```java
public class FallThroughExample {
    public static void main(String[] args) {
        int number = 3;
        switch (number) {
            case 1:
                System.out.println("The number 1");
            case 3:
                System.out.println("The number 3"); // Executed
            case 2:
                System.out.println("The number 2"); // Executed due to fall-through
                break; // Stops further fall-through
            case 7000000:
                System.out.println("The number 7,000,000"); // Not executed
        }
    }
}
```
**Output:**
```
The number 3
The number 2
```

---

## Key Points
- Fall-through is **intentional** and allows multiple `case` labels to execute the same code.
- **Use `break` statements** to prevent unintended fall-through.
- **Omitting `break`** can lead to bugs if fall-through is not intended.

---

## Common Pitfalls
Forgetting to include `break` statements can cause unintended execution of multiple `case` blocks.

**Example of unintended fall-through:**
```java
public class UnintendedFallThrough {
    public static void main(String[] args) {
        int score = 90;
        switch (score) {
            case 100:
                System.out.println("Perfect!");
            case 90:
                System.out.println("Excellent!"); // Executed
            case 80:
                System.out.println("Good"); // Also executed (fall-through)
        }
    }
}
```
**Output:**
```
Excellent!
Good
```

---

## Best Practices
- Always include a `break` statement at the end of each `case` block **unless intentional fall-through is desired**.
- Use comments to indicate intentional fall-through for clarity:
  ```java
  switch (value) {
      case 1:
      case 2: // Intentional fall-through
          System.out.println("1 or 2");
          break;
      case 3:
          System.out.println("3");
          break;
  }
  ```

---

## Summary
- Fall-through allows multiple `case` blocks to execute sequentially.
- Use `break` to control the flow and prevent unintended fall-through.
- Fall-through is a powerful feature but can introduce bugs if misused.

---
## Keywords
#Java #SwitchStatement #FallThrough #ControlFlow