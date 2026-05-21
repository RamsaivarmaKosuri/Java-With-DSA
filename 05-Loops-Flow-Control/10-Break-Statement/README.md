# Break Statement

The `break` statement is used to:

```text
exit the loop immediately
```

When Java encounters:

```java
break;
```

the loop stops instantly.

---

## Why Do We Use Break?

Sometimes we want to stop a loop early when a condition is met.

Instead of running full loop, we use:

```text
break statement
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        for(int i = 1; i <= 5; i++) {

            if(i == 3) {
                break;
            }

            System.out.println(i);
        }

        System.out.println("I am out of loop");

    }
}
```

## Output

```text
1
2
I am out of loop
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
break;
```

---

### Step 3

Loop stops immediately.

So:

```text
3, 4, 5
```

never print.

---

## Dry Run

```text
i = 1 → print 1
i = 2 → print 2
i = 3 → break
Loop stops
```

Then:

```text
I am out of loop
```

prints.

---

## Your Notes

```java
public class JavaBasics {
    public static void main(String[] args) {

        for(int i = 1; i <= 5; i++) {

            if(i == 3) {
                break;
            }

            System.out.println(i);
        }

        System.out.print("I am out of loop");
    }
}
```

---

## Important Note

```java
break;
```

works in:

- `for loop`
- `while loop`
- `do while loop`
- `switch statement`

It immediately:

```text
stops execution
```
