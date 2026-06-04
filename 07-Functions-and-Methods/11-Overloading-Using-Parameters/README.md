# Overloading Using Parameters

One way to achieve Function Overloading is by changing the number of parameters.

In this approach:

- Method Name remains the same.
- Number of Parameters changes.

Java identifies the correct method based on the number of arguments passed during the function call.

---

## Definition

Function Overloading using parameters means:

```text
Same Function Name
+
Different Number of Parameters
```

---

## Program

```java
public class JavaBasics {

    // function to calculate sum of 2 numbers
    public static int sum(int a, int b) {
        return a + b;
    }

    // function to calculate sum of 3 numbers
    public static int sum(int a, int b, int c) {
        return a + b + c;
    }

    public static void main(String[] args) {

        System.out.println(sum(3, 5));

        System.out.println(sum(5, 3, 3));

    }
}
```

---

## Output

```text
8
11
```

---

## Easy Understanding

Method 1:

```java
sum(3,5)
```

Receives:

```text
2 Parameters
```

Therefore Java calls:

```java
sum(int a,int b)
```

Result:

```text
3 + 5 = 8
```

---

Method 2:

```java
sum(5,3,3)
```

Receives:

```text
3 Parameters
```

Therefore Java calls:

```java
sum(int a,int b,int c)
```

Result:

```text
5 + 3 + 3 = 11
```

---

## Method Selection Diagram

```text
sum(3,5)
    │
    ▼
sum(int a,int b)
    │
    ▼
8


sum(5,3,3)
    │
    ▼
sum(int a,int b,int c)
    │
    ▼
11
```

---

## Dry Run Table

### Function Call

```java
sum(3,5)
```

| Parameter | Value |
|-----------|--------|
| a | 3 |
| b | 5 |

Calculation:

```text
3 + 5 = 8
```

Output:

```text
8
```

---

### Function Call

```java
sum(5,3,3)
```

| Parameter | Value |
|-----------|--------|
| a | 5 |
| b | 3 |
| c | 3 |

Calculation:

```text
5 + 3 + 3 = 11
```

Output:

```text
11
```

---

## Comparison

| Method | Parameters |
|----------|------------|
| sum(int a,int b) | 2 |
| sum(int a,int b,int c) | 3 |

Method name is same.

Number of parameters is different.

Therefore Function Overloading occurs.

---

## Key Learning

- Function names can be same.
- Number of parameters can be different.
- Java selects the correct method automatically.
- Function Overloading improves code readability.
- Similar operations can use the same method name.

---

## Special Note

From my notes:

```text
Function to calculate sum of 2 numbers

Function to calculate sum of 3 numbers
```

Both methods have the same name:

```java
sum()
```

but the number of parameters is different.

Therefore Java treats them as separate methods and this is called Function Overloading using Parameters.
