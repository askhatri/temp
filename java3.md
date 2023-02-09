# Sort customers by Name

## Requirement

* We need to short this list by name of the customer.
* There is a class Customer. It has two fields "name" and "age".
* I have added simple data with list of "customers".
* We can use anything like lamda, streams, collections api, comparator, comparable.
* The list size in output should be same as the list size in of "customers" (input). i.e. 7
* Fill free correct or fix anything in the initial version of code listed below.

## Copy following code in w3school

```java
import java.util.*;

public class Main {
  public static void main(String[] args) {
    List<Customer> customers = new ArrayList<>();
    customers.add(new Customer("H", 23));
    customers.add(new Customer("A", 21));
    customers.add(new Customer("F", 24));
    customers.add(new Customer("D", 25));
    customers.add(new Customer("G", 34));
    customers.add(new Customer("B", 34));
    customers.add(new Customer("E", 22));
    // TODO: write the code to sort customers by name
    System.out.println(customers);
  }
}
class Customer {
    private String name;
    private Integer age;
    Customer(String n, Integer a) {
         name = n;
         age = a;
    }
    public String toString() {
            return "\n[name=" + name + ", age=" + age + "]\n";
    }
}
```

## Use w3school URL

<a href="https://www.w3schools.com/java/tryjava.asp?filename=demo_compiler" target="_blank">W3schools</a> - [https://www.w3schools.com/java/tryjava.asp?filename=demo_compiler](https://www.w3schools.com/java/tryjava.asp?filename=demo_compiler)
