# While Loop

A `while loop` is used to repeatedly execute a block of code until the condition becomes:

```text
false
```

---

## Syntax

```java
while(condition) {

    // do something

}
```

### Understanding

First:

```text
condition gets checked
```

If condition is:

```text
true
```

code executes.

Again condition checks.

This process repeats until condition becomes:

```text
false
```

---

## Flow of While Loop

```text
Condition Check
      ↓
True → Execute Code
      ↓
Again Condition Check
      ↓
False → Stop
```

---

## Example: Print Hello 10 Times

```java
public class JavaBasics {
    public static void main(String args[]) {

        int counter = 0;

        while(counter < 10) {
            System.out.println("Hello");
            counter++;
        }

        System.out.println("Printed hello 10 times");

    }
}
```

## Output

```text
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Printed hello 10 times
```

---

## Code Understanding

### Step 1

```java
int counter = 0;
```

A variable is created to count repetitions.

---

### Step 2

Condition:

```java
counter < 10
```

checks whether counter is less than 10.

Initially:

```text
0 < 10 → true
```

So loop runs.

---

### Step 3

```java
counter++;
```

increases counter value by:

```text
1
```

Without this line:

```text
Infinite Loop
```

will happen because condition never changes.

---

## Your Notes

### While Loop Syntax

```java
while(condition){

    // do something

}
```

---

## Important Note

Always update loop variable.

Example:

```java
counter++;
```

Otherwise loop may run forever.
