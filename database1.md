# Write simple SQL query

There are two tables:

<table>
 <tr> <td> <b> Table 1 </b> </td>
  <td><b>employee</b></td> </tr>
 <tr> <td> Column 1 </td> <td>employee_id</td> </tr>
 <tr> <td> Column 2 </td> <td>manager_id</td> </tr>
 <tr> <td> Column 3 </td> <td>salary</td> </tr>
</table>

<table>
 <tr> <td> <b> Table 2 </b> </td>
  <td><b>manager</b></td> </tr>
 <tr> <td> Column 1 </td> <td>manager_id</td> </tr>
 <tr> <td> Column 2 </td> <td>manager_name</td> </tr>
</table>

Those tables are linked by `manager_id` column.

## Requirement

Write a query to get manager name and sum of salary of all employees reporting to him/her

## Execute the following SQL in Sqlite Online

```sql
drop table Customers;
drop table Orders;
drop table Shippings;
create table employee (employee_id int, manager_id int, salary int);
create table manager (manager_id int, manager_name varchar(100));
insert into employee values (1,1,10000), (2,2,20000), (3,2, 10000), (4,4,15000), (5,4, 25000);
insert into manager values (1, "manager1"), (2, "manager2"), (3, "manager3"), (4, "manager4");
```

## Use Sqlite Online URL

Right click --> Open in new tab. <br>
https://www.programiz.com/sql/online-compiler/

## Output:

<table>
 <tr> <td> <b> Manager Name </b> </td>
  <td><b>Sum of Salary</b></td> </tr>
 <tr> <td> manager1 </td> <td>10000</td> </tr>
 <tr> <td> manager2 </td> <td>30000</td> </tr>
 <tr> <td> manager3 </td> <td>null</td> </tr>
 <tr> <td> manager4 </td> <td>40000</td> </tr>
</table>
