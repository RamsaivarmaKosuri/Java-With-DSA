# Else If in Java

`else if` is used when we want to check **multiple conditions**.

Java checks conditions from top to bottom.

As soon as one condition becomes:

```text
true
```

that block executes and remaining conditions are skipped.

---

## Syntax

```java
if(condition1) {

    // executes if condition1 is true

}
else if(condition2) {

    // executes if condition2 is true

}
else {

    // executes when all conditions are false

}
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int age = 16;

        if(age >= 18) {
            System.out.println("Adult");
        }
        else if(age >= 13) {
            System.out.println("Teenager");
        }
        else {
            System.out.println("Child");
        }

    }
}
```

## Output

```text
Teenager
```

---

## Understanding

Java checks condition one by one.

### First Condition

```java
age >= 18
```

Output:

```text
false
```

So Java moves to next condition.

### Second Condition

```java
age >= 13
```

Output:

```text
true
```

So:

```text
Teenager
```

gets printed.

Then Java stops checking further conditions.

---

## Important Note

`if` → checks first condition

`else if` → checks additional conditions

`else` → executes when all conditions are false
