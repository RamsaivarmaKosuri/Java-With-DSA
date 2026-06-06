# Inverted and Rotated Half Pyramid

This pattern is a combination of:

- Inverted Half Pyramid
- Right Rotation using Spaces

It helps in understanding:

- Nested Loops
- Space Management
- Pattern Rotation Logic
- Row and Column Relationships

---

## Pattern Output

For:

```java
invRotHalfPyramid(4,4);
```

Output:

```text
   *
  **
 ***
****
```

---

## Program

```java
public class JavaBasics {

    public static void invRotHalfPyramid(int rows,int cols){

        for(int i=1;i<=rows;i++){

            for(int j=1;j<=cols;j++){

                if(i==rows ||
                   j==cols ||
                   i+j==5 ||
                   i+j==6){

                    System.out.print("*");

                }else{

                    System.out.print(" ");

                }
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {

        invRotHalfPyramid(4,4);

    }
}
```

---

## Understanding the Pattern

For:

```text
rows = 4
cols = 4
```

The pattern looks like:

```text
Row 1 →    *
Row 2 →   **
Row 3 →  ***
Row 4 → ****
```

Notice:

```text
Stars increase

1 → 2 → 3 → 4
```

while

```text
Spaces decrease

3 → 2 → 1 → 0
```

---

## Visual Grid

```text
(1,1) (1,2) (1,3) (1,4)

(2,1) (2,2) (2,3) (2,4)

(3,1) (3,2) (3,3) (3,4)

(4,1) (4,2) (4,3) (4,4)
```

Star Positions:

```text
      *
    * *
  * * *
* * * *
```

Which prints as:

```text
   *
  **
 ***
****
```

---

## Why i + j ?

For a 4 × 4 grid:

```text
i + j = 5
```

creates:

```text
(1,4)
(2,3)
(3,2)
(4,1)
```

and

```text
i + j = 6
```

creates:

```text
(2,4)
(3,3)
(4,2)
```

These positions help form the pyramid shape.

---

## Dry Run

Input:

```text
rows = 4
cols = 4
```

### Row 1

| i | j | Condition | Output |
|---|---|------------|---------|
| 1 | 1 | False | Space |
| 1 | 2 | False | Space |
| 1 | 3 | False | Space |
| 1 | 4 | j==cols | * |

Output:

```text
   *
```

---

### Row 2

| i | j | Condition | Output |
|---|---|------------|---------|
| 2 | 1 | False | Space |
| 2 | 2 | False | Space |
| 2 | 3 | i+j=5 | * |
| 2 | 4 | j==cols | * |

Output:

```text
  **
```

---

### Row 3

| i | j | Condition | Output |
|---|---|------------|---------|
| 3 | 1 | False | Space |
| 3 | 2 | i+j=5 | * |
| 3 | 3 | i+j=6 | * |
| 3 | 4 | j==cols | * |

Output:

```text
 ***
```

---

### Row 4

| i | j | Condition | Output |
|---|---|------------|---------|
| 4 | 1 | Last Row | * |
| 4 | 2 | Last Row | * |
| 4 | 3 | Last Row | * |
| 4 | 4 | Last Row | * |

Output:

```text
****
```

---

## Final Output

```text
   *
  **
 ***
****
```

---

## Easy Understanding Trick

Think:

```text
Spaces ↓

3
2
1
0
```

and

```text
Stars ↑

1
2
3
4
```

As rows increase:

```text
Spaces decrease

Stars increase
```

This creates the rotated pyramid.

---

## Alternative Logic (Easy Method)

Most students solve it using:

```java
for(int i=1;i<=n;i++){

    for(int j=1;j<=n-i;j++){
        System.out.print(" ");
    }

    for(int j=1;j<=i;j++){
        System.out.print("*");
    }

    System.out.println();
}
```

This produces the same output and is easier to remember.

---

## Key Learning

- Spaces play an important role in pattern problems.
- Increasing stars and decreasing spaces create rotation.
- Row and Column relationships help form shapes.
- Multiple conditions can be combined to generate patterns.

---

## Special Note

Remember:

```text
Spaces Decrease
        ↓
Stars Increase
        ↓
Right Rotated Pyramid
```

This idea is used again in:

- Full Pyramid
- Diamond Pattern
- Butterfly Pattern
- Pascal's Triangle
