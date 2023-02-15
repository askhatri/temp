# Java sample code 1

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
