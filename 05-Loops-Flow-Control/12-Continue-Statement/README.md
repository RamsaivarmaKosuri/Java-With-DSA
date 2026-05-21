# Continue Statement

The `continue` statement is used to:

```text
skip the current iteration
```

of a loop.

Instead of stopping the loop like:

```text
break
```

`continue` skips the current iteration and moves to the:

```text
next iteration
```

---

## Why Do We Use Continue?

Sometimes we want to:

```text
skip certain values
```

without stopping the entire loop.

In such cases, we use:

```text
continue statement
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        for(int i = 1; i <= 5; i++) {

            if(i == 3) {
                continue;
            }

            System.out.println(i);
        }

    }
}
```

## Output

```text
1
2
4
5
```

---

## Code Understanding

### Step 1

Loop starts:

```java
for(int i = 1; i <= 5; i++)
```

Values:

```text
1 → 2 → 3 → 4 → 5
```

---

### Step 2

When:

```java
i == 3
```

condition becomes:

```text
true
```

Java executes:

```java
continue;
```

---

### Step 3

Current iteration gets skipped.

So:

```text
3
```

does not print.

Loop continues with:

```text
4
```

---

## Dry Run

```text
i = 1 → print 1
i = 2 → print 2
i = 3 → skip
i = 4 → print 4
i = 5 → print 5
```

---

## Difference Between Break and Continue

### Break

```text
Stops the entire loop
```

---

### Continue

```text
Skips only current iteration
```

---

## Your Notes

```text
CONTINUE STATEMENT

used to skip an iteration
```

---

## Important Note

```java
continue;
```

does not stop the loop.

It only:

```text
skips one iteration
```

and continues execution.
