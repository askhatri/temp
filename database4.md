# Write simple SQL query

## Table structure

There are two tables:

<table>
 <tr> <td> <b> Table 1 </b> </td>
  <td><b>employee</b></td> </tr>
 <tr> <td> Column 1 </td> <td>employee_id</td> </tr>
 <tr> <td> Column 2 </td> <td>employee_name</td> </tr>
</table>

<table>
 <tr> <td> <b> Table 2 </b> </td>
  <td><b>department</b></td> </tr>
 <tr> <td> Column 1 </td> <td>department_id</td> </tr>
 <tr> <td> Column 2 </td> <td>department_name</td> </tr>
</table>

<table>
 <tr> <td> <b> Table 3 </b> </td>
  <td><b>ed_map</b></td> </tr>
 <tr> <td> Column 1 </td> <td>employee_id</td> </tr>
 <tr> <td> Column 2 </td> <td>department_id</td> </tr>
</table>

## Table data

One employee can work for one or more department. One department can have one or more employees.

Department table:
<table>
 <tr> <td> <b> department_id </b> </td>
  <td><b>department_name</b></td> </tr>
 <tr> <td> 1 </td> <td>Engineering</td> </tr>
 <tr> <td> 2 </td> <td>Sales</td> </tr>
 <tr> <td> 3 </td> <td>Finance</td> </tr>
</table>

Employee table:
<table>
 <tr> <td> <b> employee_id </b> </td>
  <td><b>employee_name</b></td> </tr>
 <tr> <td> 1 </td> 
   <td>Mike</td></tr>
 <tr> <td> 2 </td>
   <td>Sam</td></tr>
 <tr> <td> 3 </td> <td>Rita</td> </tr>
</table>

Employee Department table:
<table>
 <tr> <td> <b> employee_id </b> </td>
  <td><b>department_id</b></td> </tr>
 <tr> <td> 1 </td> <td>1</td> </tr>
 <tr> <td> 2 </td> <td>1</td> </tr>
 <tr> <td> 2 </td> <td>2</td> </tr>
 <tr> <td> 3 </td> <td>2</td> </tr>
 <tr> <td> 3 </td> <td>3</td> </tr>
</table>

## Requirement

Write a query to get employee name and department name.

## Execute the following SQL in Sqlite Online

```sql
drop table Customers;
drop table Orders;
drop table Shippings;
create table employee (employee_id int, employee_name varchar(100));
create table department (department_id int, department_name varchar(100));
create table ed_map (employee_id int, department_id int);
insert into employee values (1, 'Mike'), (2, 'Sam'), (3, 'Rita');
insert into department values (1, "Engineering"), (2, "Sales"), (3, "Finance");
insert into ed_map values (1, 1), (2, 1), (2, 2), (3, 2), (3, 3);
```

## Use Sqlite Online URL

Right click --> Open in new tab. <br>
https://www.programiz.com/sql/online-compiler/

# Sample output
<table>
 <tr> <td> <b> employee_name </b> </td>
  <td><b>department_name</b></td> </tr>
 <tr> <td> Mike </td> <td>Engineering</td> </tr>
 <tr> <td> Sam </td> <td>Engineering</td> </tr>
 <tr> <td> Sam </td> <td>Sales</td> </tr>
 <tr> <td> Rita </td> <td>Sales</td> </tr>
 <tr> <td> Rita </td> <td>Finance</td> </tr>
</table>
