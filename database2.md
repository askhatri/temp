# Storing employees data

## Table structure

There are two tables:

<table>
 <tr> <td> <b> Table 1 </b> </td>
  <td><b>employee</b></td> </tr>
 <tr> <td> Column 1 </td> <td>employee_id</td> </tr>
 <tr> <td> Column 2 </td> <td>department_id</td> </tr>
 <tr> <td> Column 3 </td> <td>employee_name</td> </tr>
</table>

<table>
 <tr> <td> <b> Table 2 </b> </td>
  <td><b>department</b></td> </tr>
 <tr> <td> Column 1 </td> <td>department_id</td> </tr>
 <tr> <td> Column 2 </td> <td>department_name</td> </tr>
</table>

Those tables are linked by `department_id` column.

## Table data

One employee can work for one or more department. One department can have one or more employees.

Department table:
<table>
 <tr> <td> <b> department_id </b> </td>
  <td><b>department_name</b></td> </tr>
 <tr> <td> department1 </td> <td>Engineering</td> </tr>
 <tr> <td> department2 </td> <td>Sales</td> </tr>
 <tr> <td> department2 </td> <td>Finance</td> </tr>
</table>

Employee table:
<table>
 <tr> <td> <b> employee_id </b> </td>
  <td><b>department_id</b></td> 
  <td><b>employee_name</b></td> </tr>
 <tr> <td> employee1 </td> <td>department1</td> 
   <td>Mike</td></tr>
 <tr> <td> employee2 </td> <td>department1</td> 
   <td>Sam</td></tr>
 <tr> <td> employee2 </td> <td>department2</td>
   <td>Sam</td></tr>
 <tr> <td> employee3 </td> <td>department2</td> <td>Rita</td> </tr>
 <tr> <td> employee3 </td> <td>department3</td> <td>Rita</td> </tr>
</table>

## Question

How to optimize those tables so that we can avoid storing employee's name like "Sam" and "Rita" multiple time?

