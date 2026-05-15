# Creating a Java File

## What is a Java File?

A Java file is a file where Java code is written.

A Java file always ends with:

```text
.java
```

Example:

```text
JavaBasics.java
```

---

## Steps to Create a Java File

### Step 1

Open your code editor (VS Code / Eclipse).

### Step 2

Create a new file.

### Step 3

Save the file with `.java` extension.

Example:

```text
HelloWorld.java
```

---

## Basic Structure of a Java File

```java
public class HelloWorld {
    public static void main(String[] args) {

    }
}
```

---

## Important Rules

### 1. File Name and Class Name Must Be Same

Correct:

```text
File Name: HelloWorld.java
Class Name: HelloWorld
```

Wrong:

```text
File Name: Java.java
Class Name: HelloWorld
```

This gives an error.

---

### 2. Java is Case Sensitive

These are different:

```text
JavaBasics
javabasics
JAVABASICS
```

Java treats them as different names.

---

## Example Program

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello Java");
    }
}
```

Output:

```text
Hello Java
```

---

## Important Note

Every Java program must be saved with:

```text
.java
```

extension.
