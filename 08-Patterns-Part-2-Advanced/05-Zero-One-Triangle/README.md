# 0-1 Triangle Pattern

The 0-1 Triangle is a special pattern where:

- `1` is printed when the sum of row and column is even.
- `0` is printed when the sum of row and column is odd.

This pattern helps in understanding:

- Nested Loops
- Conditional Logic
- Even and Odd Numbers
- Pattern Visualization

---

## Pattern Output

For:

```java
Triangle(5);
```

Output:

```text
1
01
101
0101
10101
```

---

## Program

```java
public class JavaBasics {

    public static void Triangle(int n){

        for(int i=1;i<=n;i++){

            for(int j=1;j<=i;j++){

                if((i+j)%2==0){

                    System.out.print("1");

                }else{

                    System.out.print("0");

                }
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {

        Triangle(5);

    }
}
```

---

## Logic

We check:

```java
(i + j) % 2
```

If:

```java
(i + j) % 2 == 0
```

Print:

```text
1
```

Else:

```text
0
```

---

## Why Does It Work?

### Even Sum

```text
1 + 1 = 2
```

Even

```text
Print 1
```

---

### Odd Sum

```text
2 + 1 = 3
```

Odd

```text
Print 0
```

---

## Dry Run

Input:

```text
n = 5
```

---

### Row 1

| i | j | i+j | Even/Odd | Output |
|---|---|------|----------|---------|
| 1 | 1 | 2 | Even | 1 |

Output:

```text
1
```

---

### Row 2

| i | j | i+j | Even/Odd | Output |
|---|---|------|----------|---------|
| 2 | 1 | 3 | Odd | 0 |
| 2 | 2 | 4 | Even | 1 |

Output:

```text
01
```

---

### Row 3

| i | j | i+j | Even/Odd | Output |
|---|---|------|----------|---------|
| 3 | 1 | 4 | Even | 1 |
| 3 | 2 | 5 | Odd | 0 |
| 3 | 3 | 6 | Even | 1 |

Output:

```text
101
```

---

### Row 4

| i | j | i+j | Even/Odd | Output |
|---|---|------|----------|---------|
| 4 | 1 | 5 | Odd | 0 |
| 4 | 2 | 6 | Even | 1 |
| 4 | 3 | 7 | Odd | 0 |
| 4 | 4 | 8 | Even | 1 |

Output:

```text
0101
```

---

### Row 5

| i | j | i+j | Even/Odd | Output |
|---|---|------|----------|---------|
| 5 | 1 | 6 | Even | 1 |
| 5 | 2 | 7 | Odd | 0 |
| 5 | 3 | 8 | Even | 1 |
| 5 | 4 | 9 | Odd | 0 |
| 5 | 5 | 10 | Even | 1 |

Output:

```text
10101
```

---

## Final Output

```text
1
01
101
0101
10101
```

---

## Visual Representation

```text
1

0 1

1 0 1

0 1 0 1

1 0 1 0 1
```

Notice:

```text
1 and 0 alternate continuously.
```

---

## Easy Understanding Trick

Remember:

```text
(i + j) Even
        ↓
      Print 1
```

```text
(i + j) Odd
       ↓
     Print 0
```

That's the entire pattern logic.

---

## Pattern Building

Check each box:

```text
Row + Column
```

If:

```text
Even → 1
```

If:

```text
Odd → 0
```

The triangle automatically forms.

---

## Key Learning

- Conditions can be used to create patterns.
- Even and Odd concepts are very useful in pattern problems.
- `(i + j) % 2` is a common pattern trick.
- Outer loop controls rows.
- Inner loop controls columns.

---

## Special Note

Remember:

```java
(i + j) % 2 == 0
```

means:

```text
Print 1
```

and

```java
(i + j) % 2 != 0
```

means:

```text
Print 0
```

This single condition creates the entire 0-1 Triangle Pattern.
