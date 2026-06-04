# Overloading Using Data Types

Another way to achieve Function Overloading is by changing the data types of parameters.

In this approach:

- Method Name remains the same.
- Number of Parameters remains the same.
- Data Types of Parameters change.

Java identifies the correct method based on the type of arguments passed during the function call.

---

## Definition

Function Overloading using Data Types means:

```text
Same Function Name
+
Same Number of Parameters
+
Different Data Types
```

---

## Program

```java
public class JavaBasics {

    // function to calculate int sum
    public static int sum(int a, int b) {
        return a + b;
    }

    // function to calculate float sum
    public static float sum(float a, float b) {
        return a + b;
    }

    public static void main(String[] args) {

        System.out.println(sum(1, 2));

        System.out.println(sum(1.5f, 4.5f));

    }
}
```

---

## Output

```text
3
6.0
```

---

## Easy Understanding

### Function Call 1

```java
sum(1,2)
```

Arguments:

```text
int, int
```

Java selects:

```java
sum(int a,int b)
```

Calculation:

```text
1 + 2 = 3
```

Output:

```text
3
```

---

### Function Call 2

```java
sum(1.5f,4.5f)
```

Arguments:

```text
float, float
```

Java selects:

```java
sum(float a,float b)
```

Calculation:

```text
1.5 + 4.5 = 6.0
```

Output:

```text
6.0
```

---

## Method Selection Diagram

```text
sum(1,2)
   │
   ▼
sum(int,int)
   │
   ▼
3


sum(1.5f,4.5f)
   │
   ▼
sum(float,float)
   │
   ▼
6.0
```

---

## Dry Run Table

### Function Call

```java
sum(1,2)
```

| Parameter | Value |
|-----------|--------|
| a | 1 |
| b | 2 |

Calculation:

```text
1 + 2 = 3
```

Output:

```text
3
```

---

### Function Call

```java
sum(1.5f,4.5f)
```

| Parameter | Value |
|-----------|--------|
| a | 1.5 |
| b | 4.5 |

Calculation:

```text
1.5 + 4.5 = 6.0
```

Output:

```text
6.0
```

---

## Comparison

| Method | Data Type |
|----------|-----------|
| sum(int a,int b) | int |
| sum(float a,float b) | float |

Method name is same.

Number of parameters is same.

Data types are different.

Therefore Function Overloading occurs.

---

## Visual Representation

```text
sum()

├── sum(int,int)

└── sum(float,float)
```

Java automatically chooses the correct method based on the argument types.

---

## Key Learning

- Function names can be the same.
- Number of parameters can remain the same.
- Data types can be different.
- Java selects the correct method automatically.
- Function Overloading improves code readability and reusability.

---

## Special Note

From my notes:

```text
Function to calculate int sum

Function to calculate float sum
```

Both methods have the same name:

```java
sum()
```

The number of parameters is the same.

The data types are different.

Therefore Java treats them as separate methods and this is called Function Overloading using Data Types.
