
Conditional statements (e.g., `if`, `else if`, `while`) rely on operators to evaluate conditions. These operators determine whether a condition is `true` or `false`.

---

## 1. Equality Operators
Equality operators check if two values are equal or not.

| Operator | Name               | Example          | Description                          |
|----------|--------------------|------------------|--------------------------------------|
| `==`     | Equal to           | `x == y`         | Returns `true` if `x` equals `y`     |
| `!=`     | Not equal to       | `x != y`         | Returns `true` if `x` does not equal `y` |

```java
public class EqualityExample {
    public static void main(String[] args) {
        int x = 10;
        int y = 10;
        if (x == y) {
            System.out.println("x is equal to y");
        }
    }
}
```

---

## 2. Relational Operators
Relational operators compare the relative size or order of values.

| Operator | Name               | Example          | Description                          |
|----------|--------------------|------------------|--------------------------------------|
| `>`      | Greater than       | `x > y`          | Returns `true` if `x` is greater than `y` |
| `<`      | Less than          | `x < y`          | Returns `true` if `x` is less than `y`    |
| `>=`     | Greater than or equal to | `x >= y`   | Returns `true` if `x` is greater than or equal to `y` |
| `<=`     | Less than or equal to    | `x <= y`   | Returns `true` if `x` is less than or equal to `y`    |

```java
public class RelationalExample {
    public static void main(String[] args) {
        int x = 15;
        int y = 10;
        if (x > y) {
            System.out.println("x is greater than y");
        }
    }
}
```

---

## 3. Logical Operators
Logical operators combine multiple conditions.

| Operator | Name               | Example          | Description                          |
|----------|--------------------|------------------|--------------------------------------|
| `&&`     | Logical AND        | `x > 0 && y > 0` | Returns `true` if both conditions are `true` |
| `\|\|`   | Logical OR         | `x > 0 \|\| y > 0` | Returns `true` if at least one condition is `true` |
| `!`      | Logical NOT        | `!(x > 0)`       | Returns `true` if the condition is `false` |

```java
public class LogicalExample {
    public static void main(String[] args) {
        int x = 5;
        int y = 10;
        if (x > 0 && y > 0) {
            System.out.println("Both x and y are positive");
        }
    }
}
```

---

## Key Takeaways
- Use **equality operators** (`==`, `!=`) to check for equality or inequality.
- Use **relational operators** (`>`, `<`, `>=`, `<=`) to compare values.
- Use **logical operators** (`&&`, `\|\|`, `!`) to combine or negate conditions.
