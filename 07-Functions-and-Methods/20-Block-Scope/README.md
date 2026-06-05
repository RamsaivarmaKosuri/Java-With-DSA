# Block Scope

## What is Block Scope?

A block is a section of code enclosed within:

```java
{
    
}
```

Variables declared inside a block can only be used inside that block.

This is called:

```text
Block Scope
```

---

## Definition

Simple Meaning:

```text
A variable declared inside a block can only be accessed inside that block.
```

Outside the block, the variable cannot be used.

---

## Example

```java
public class JavaBasics {

    public static void main(String[] args) {

        {
            int a = 10;

            System.out.println(a);
        }

    }
}
```

Output:

```text
10
```

Here:

```text
a
```

is declared inside the block:

```java
{
    int a = 10;
}
```

Therefore it can be used only inside that block.

---

## Wrong Example

```java
public class JavaBasics {

    public static void main(String[] args) {

        {
            int a = 10;
        }

        System.out.println(a);

    }
}
```

Output:

```text
Compile Time Error
```

Reason:

```text
a was declared inside the block.

After the block ends,
a is no longer accessible.
```

---

## Dry Run

Program:

```java
{
    int a = 10;

    System.out.println(a);
}
```

| Step | Action |
|--------|---------|
| 1 | Block starts |
| 2 | Variable a is created |
| 3 | Value 10 stored in a |
| 4 | Print a |
| 5 | Block ends |
| 6 | Variable a is destroyed |

Output:

```text
10
```

---

## Easy Understanding

Think of a block as a room.

```text
{
    int a = 10;
}
```

Inside the room:

```text
a is visible
```

Outside the room:

```text
a is invisible
```

---

## Example with Loop

```java
public class JavaBasics {

    public static void main(String[] args) {

        for(int i = 1; i <= 3; i++) {
            System.out.println(i);
        }

    }
}
```

Output:

```text
1
2
3
```

Here:

```text
i
```

belongs to the:

```java
for()
```

block.

After the loop ends:

```text
i cannot be accessed.
```

---

## Wrong Example with Loop

```java
public class JavaBasics {

    public static void main(String[] args) {

        for(int i = 1; i <= 3; i++) {
            System.out.println(i);
        }

        System.out.println(i);

    }
}
```

Output:

```text
Compile Time Error
```

Reason:

```text
i exists only inside the loop block.
```

---

## Method Scope vs Block Scope

| Method Scope | Block Scope |
|-------------|-------------|
| Variable belongs to a method | Variable belongs to a block |
| Accessible throughout the method | Accessible only inside the block |
| Destroyed when method ends | Destroyed when block ends |

Example:

```java
public static void main(String[] args) {

    int x = 5; // Method Scope

    {
        int y = 10; // Block Scope
    }

}
```

Here:

```text
x → available throughout main()

y → available only inside the block
```

---

## Visual Representation

```text
main()

├── x = 5
│
├── {
│      y = 10
│   }
│
└── x accessible here

y NOT accessible here
```

---

## Key Points

- A block is enclosed within `{ }`.
- Variables declared inside a block have Block Scope.
- Block variables cannot be used outside the block.
- Loops and if statements create blocks.
- Variables are destroyed when the block ends.

---

## Special Note

Remember:

```text
Created Inside Block
         ↓
Used Inside Block
         ↓
Block Ends
         ↓
Variable Destroyed
```

This is called:

```text
Block Scope
```
