# Output in Java

Java provides methods to display output on the screen.

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        System.out.print("Hello");
        System.out.println("Hello");
        System.out.print("Hello\n");

    }
}
```

## Types of Output Statements

### `System.out.print()`

Prints output on the same line.

Example:

```java
System.out.print("Hello");
System.out.print("World");
```

Output:

```text
HelloWorld
```

---

### `System.out.println()`

Prints output and moves to the next line.

Example:

```java
System.out.println("Hello");
System.out.println("World");
```

Output:

```text
Hello
World
```

---

### `\n` (New Line)

`\n` is used to move text to the next line.

Example:

```java
System.out.print("Hello\n");
System.out.print("World");
```

Output:

```text
Hello
World
```

## Quick Revision

- `print()` → same line  
- `println()` → next line  
- `\n` → manually gives new line
