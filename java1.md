# Use w3school URL

<a href="https://www.w3schools.com/java/tryjava.asp?filename=demo_compiler" target="_blank">W3schools</a>

[https://www.w3schools.com/java/tryjava.asp?filename=demo_compiler](https://www.w3schools.com/java/tryjava.asp?filename=demo_compiler)

# Use following code

```java
import java.util.*;

public class Main {
  public static void main(String[] args) {
    List<Customer> customers = new ArrayList<>();
    customers.add(new Customer("B", 23));
    customers.add(new Customer("A", 21));
    customers.add(new Customer("F", 24));
    customers.add(new Customer("D", 25));
    customers.add(new Customer("C", null));
    customers.add(null);
    customers.add(new Customer(null, 22));
    // TODO: write the code to sort customers by age
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

# Requirement

* There is a class Customer. It has two fields "name" and "age".
* I have added simple data with list of "customers".
* We need to short this list by age of the customer.
* We can use anything like lamda, streams, collections api, comparator, comparable.
* We can write code anywhere this is file.
* We can change anything in the file but it should compile and produce correct output.
* The list size in output should be same as the list size in of "customers" (input). i.e. 7
