# Do While Loop

A `do while loop` is used to repeatedly execute a block of code.

It is similar to:

```text
while loop
```

But there is one important difference:

```text
Do While Loop executes at least one time
```

even if condition becomes:

```text
false
```

---

## Syntax

```java
do {

    // do something

} while(condition);
```

---

## How Do While Loop Works

### Step 1

First:

```text
code executes
```

---

### Step 2

Then:

```text
condition gets checked
```

If condition becomes:

```text
true
```

loop runs again.

If:

```text
false
```

loop stops.

---

## Flow of Do While Loop

```text
Execute Code
      ↓
Check Condition
      ↓
True → Repeat
False → Stop
```

---

## Example Program

Print:

```text
Hello
```

5 times.

```java
public class JavaBasics {
    public static void main(String[] args) {

        int counter = 1;

        do {

            System.out.println("Hello");
            counter++;

        } while(counter <= 5);

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
```

---

## Code Understanding

### Step 1

```java
int counter = 1;
```

Loop starts from:

```text
1
```

---

### Step 2

Code inside:

```java
do { }
```

executes first.

So:

```text
Hello
```

prints.

---

### Step 3

```java
counter++;
```

increases counter value.

---

### Step 4

Condition:

```java
counter <= 5
```

gets checked.

If:

```text
true
```

loop repeats.

If:

```text
false
```

loop stops.

---

## Difference Between While and Do While

### While Loop

First:

```text
condition checks
```

Then:

```text
code executes
```

---

### Do While Loop

First:

```text
code executes
```

Then:

```text
condition checks
```

---

## Example Showing Difference

### While Loop

```java
int x = 10;

while(x < 5) {
    System.out.println("Hello");
}
```

## Output

```text
Nothing prints
```

because condition is false.

---

### Do While Loop

```java
int x = 10;

do {
    System.out.println("Hello");
} while(x < 5);
```

## Output

```text
Hello
```

because do-while runs:

```text
at least one time
```

---

## Your Notes

```java
do {

    // do something

} while(condition);
```

---

## Important Note

A:

```text
semicolon ;
```

must be written after:

```java
while(condition);
```
