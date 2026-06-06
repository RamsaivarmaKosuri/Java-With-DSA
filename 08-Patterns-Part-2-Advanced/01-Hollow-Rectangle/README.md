# Hollow Rectangle Pattern

The Hollow Rectangle Pattern is an advanced star pattern where:

- Boundary positions contain `*`
- Inner positions contain spaces

This pattern helps in understanding:

- Nested Loops
- Row and Column Logic
- Boundary Conditions
- Pattern Visualization

---

## Pattern Output

For:

```java
hollow_rectangle(4,5);
```

Output:

```text
*****
*   *
*   *
*****
```

---

## Program

```java
public class JavaBasics {

    public static void hollow_rectangle(int rows,int cols){

        for(int i=1;i<=rows;i++){

            for(int j=1;j<=cols;j++){

                if(i==1 || i==rows ||
                   j==1 || j==cols){

                    System.out.print("*");

                }else{

                    System.out.print(" ");

                }
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {

        hollow_rectangle(4,5);

    }
}
```

---

## Logic

A Hollow Rectangle consists of:

```text
Top Boundary
Bottom Boundary
Left Boundary
Right Boundary
```

All boundary positions print:

```text
*
```

All inner positions print:

```text
(space)
```

---

## Boundary Condition

```java
if(i==1 || i==rows ||
   j==1 || j==cols)
```

Meaning:

```text
First Row
Last Row
First Column
Last Column
```

Print:

```text
*
```

Otherwise:

```text
(space)
```

---

## Visual Representation

For:

```text
rows = 4
cols = 5
```

Grid:

```text
(1,1) (1,2) (1,3) (1,4) (1,5)

(2,1) (2,2) (2,3) (2,4) (2,5)

(3,1) (3,2) (3,3) (3,4) (3,5)

(4,1) (4,2) (4,3) (4,4) (4,5)
```

Boundary Cells:

```text
*****
*   *
*   *
*****
```

---

## Dry Run

Input:

```text
rows = 4
cols = 5
```

### Row 1

| i | j | Condition | Output |
|---|---|------------|---------|
| 1 | 1 | First Row | * |
| 1 | 2 | First Row | * |
| 1 | 3 | First Row | * |
| 1 | 4 | First Row | * |
| 1 | 5 | First Row | * |

Output:

```text
*****
```

---

### Row 2

| i | j | Condition | Output |
|---|---|------------|---------|
| 2 | 1 | First Column | * |
| 2 | 2 | Inner Cell | Space |
| 2 | 3 | Inner Cell | Space |
| 2 | 4 | Inner Cell | Space |
| 2 | 5 | Last Column | * |

Output:

```text
*   *
```

---

### Row 3

| i | j | Condition | Output |
|---|---|------------|---------|
| 3 | 1 | First Column | * |
| 3 | 2 | Inner Cell | Space |
| 3 | 3 | Inner Cell | Space |
| 3 | 4 | Inner Cell | Space |
| 3 | 5 | Last Column | * |

Output:

```text
*   *
```

---

### Row 4

| i | j | Condition | Output |
|---|---|------------|---------|
| 4 | 1 | Last Row | * |
| 4 | 2 | Last Row | * |
| 4 | 3 | Last Row | * |
| 4 | 4 | Last Row | * |
| 4 | 5 | Last Row | * |

Output:

```text
*****
```

---

## Final Output

```text
*****
*   *
*   *
*****
```

---

## Easy Understanding Trick

Think:

```text
Border = *

Inside = Space
```

or

```text
First Row    → *
Last Row     → *
First Column → *
Last Column  → *

Everything Else → Space
```

---

## Key Learning

- Nested loops help traverse rows and columns.
- Boundary cells form the rectangle border.
- Inner cells are left empty.
- Conditions are used to identify border positions.
- Hollow Rectangle is the foundation for many advanced patterns.

---

## Special Note

Remember:

```text
Top Row
Bottom Row
Left Column
Right Column
```

These four boundaries create the Hollow Rectangle.

If a cell lies on any boundary:

```text
Print *
```

Otherwise:

```text
Print Space
```
