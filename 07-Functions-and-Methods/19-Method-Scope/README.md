# Method Scope

Scope refers to:

```text
Where a variable can be accessed in a program.
```

If a variable is declared in one place, it cannot always be used everywhere.

The area where a variable can be accessed is called its:

```text
Scope
```

---

## Definition

From my notes:

```text
Agar aap koi bhi variable ko define kiya aur us variable ko kaha kaha use kar sakte hai vo ban jata hai us variable ka scope.
```

Simple Meaning:

```text
Scope tells us where a variable is visible and usable.
```

---

## What is Method Scope?

A variable declared inside a method can only be used inside that method.

It cannot be accessed outside that method.

---

## Example

```java
public class JavaBasics {

    public static void sum() {

        int a = 10;
        int b = 20;

        System.out.println(a + b);
    }

    public static void main(String[] args) {

        sum();

    }
}
```

Output:

```text
30
```

Here:

```text
a and b
```

are created inside:

```java
sum()
```

Therefore they can only be used inside:

```java
sum()
```

---

## Wrong Example

```java
public class JavaBasics {

    public static void sum() {

        int a = 10;
        int b = 20;

    }

    public static void main(String[] args) {

        System.out.println(a);

    }
}
```

Output:

```text
Error
```

Reason:

```text
a belongs to sum() method.

main() cannot access it.
```

---

## Visual Representation

```text
sum()

 ├── a = 10
 ├── b = 20
 └── Accessible Here


main()

 └── Cannot Access a and b
```

---

## Easy Understanding

Think of every method as a separate room.

Example:

```text
Room 1 = sum()

Room 2 = main()
```

If:

```text
a = 10
```

is kept inside Room 1,

then Room 2 cannot directly use it.

Each room has its own variables.

---

## Dry Run

Program:

```java
public static void sum(){

    int a = 10;

    System.out.println(a);

}
```

| Step | Action |
|--------|---------|
| 1 | Method sum() starts |
| 2 | Variable a is created |
| 3 | Value 10 stored in a |
| 4 | Print a |
| 5 | Method ends |
| 6 | Variable a is destroyed |

Output:

```text
10
```

---

## Important Point

Variables created inside a method:

```text
Exist only while the method is running.
```

After the method finishes:

```text
The variables are removed from memory.
```

---

## Real Life Example

```text
Classroom A
```

has:

```text
Board Marker
```

Students inside Classroom A can use it.

Students in:

```text
Classroom B
```

cannot directly use it.

Similarly:

```text
Variables inside one method
cannot be directly used in another method.
```

---

## Key Learning

- Scope means visibility of a variable.
- Method Scope limits variables to a specific method.
- Variables created inside a method stay inside that method.
- Other methods cannot directly access them.
- Variables are destroyed after method execution completes.

---

## Special Note

Remember:

```text
Created Inside Method
          ↓
Use Inside Method
          ↓
Method Ends
          ↓
Variable Destroyed
```

This is called:

```text
Method Scope
```
