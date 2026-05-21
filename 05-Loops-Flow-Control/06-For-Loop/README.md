# For Loop

A `for loop` is used to repeatedly execute a block of code.

It is mostly used when we know:

```text
how many times
```

the loop should run.

---

## Syntax

```java
for(initialisation; condition; updation) {

    // do something

}
```

---

## Understanding Syntax

### 1. Initialisation

```java
int i = 1
```

Used to initialize the loop variable.

It runs:

```text
only one time
```

at the beginning.

---

### 2. Condition

```java
i <= 5
```

Checks whether loop should continue.

If condition becomes:

```text
true
```

loop runs.

If:

```text
false
```

loop stops.

---

### 3. Updation

```java
i++
```

Used to update loop variable.

Usually:

```text
increase or decrease
```

happens here.

---

## Example Program

Print numbers from:

```text
1 to 5
```

```java
public class JavaBasics {
    public static void main(String[] args) {

        for(int i = 1; i <= 5; i++) {
            System.out.println(i);
        }

    }
}
```

## Output

```text
1
2
3
4
5
```

---

## Code Understanding

### Step 1

```java
int i = 1
```

Loop starts from:

```text
1
```

---

### Step 2

Condition:

```java
i <= 5
```

checks whether loop should continue.

Initially:

```text
1 <= 5 → true
```

So loop runs.

---

### Step 3

```java
System.out.println(i);
```

prints current value.

---

### Step 4

```java
i++
```

increases value by:

```text
1
```

This repeats until:

```text
i becomes 6
```

Then condition becomes:

```text
false
```

and loop stops.

---

## Dry Run

```text
i = 1 → print 1
i = 2 → print 2
i = 3 → print 3
i = 4 → print 4
i = 5 → print 5
i = 6 → stop
```

---

## Your Notes

### For Loop Syntax

```java
for(initialisation; condition; updation) {

    // do something

}
```

---

## Difference Between While and For Loop

### While Loop

Used when number of iterations is:

```text
not fixed
```

### For Loop

Used when number of iterations is:

```text
known
```
