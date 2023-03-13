# Java sample code

Let's review this code and check if there is any compilation error or compilation warning or not.
If the code is correct the try to find output.

```java
public class Main {
    public static void main(String[] args) {
        Child.printString();
        Child.printValue();
    }
}

class Parent {
    public static void printString() {
        System.out.println("Hi");
    }
    public static void printValue() {
        System.out.println("1");
    }
}

class Child extends Parent {
    public static void printValue() {
        System.out.println("2");
    }
}
```
