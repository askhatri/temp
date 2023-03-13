# Java sample code 1

Let's review this code and check if there is any compilation error or compilation warning or not.
If the code is correct the try to find output.

```java
public class Main {
    public static void main(String[] args) {
        int i;
        System.out.println("Value of i is " + i);
    }
}
```

# Java sample code 2

```java
public class Main {
    public static void main(String[] args) {
        try {
            int i = 5 / 0;
            System.out.println("Value of i is " + i);
        } catch (Exception e) {
            System.out.println("General Exception");
        } catch (ArithmeticException e) {
            System.out.println("ArithmeticException");
        }
    }
}
```
