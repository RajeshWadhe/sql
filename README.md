# sql
sql queries


1. Display details of jobs where the minimum salary is greater than 10000.

i) Query -- > SELECT JOB_ID,JOB_TITLE,MIN_SALARY,MAX_SALARY FROM JOBS
        WHERE MIN_SALARY>10000;
ii) Query -- > SELECT *FROM JOBS WHERE MIN_SALARY>10000;

2. Display the first name and join date of the employees who joined between 2002 and 2005.

Query -- > SELECT FIRST_NAME, HIRE_DATE FROM  EMPLOYEES
                   WHERE HIRE_DATE BETWEEN '2003-01-01' AND '2005-12-31';

3. Display first name and join date of the employees who is either IT Programmer or Sales Man.
 
Query  -- > SELECT FIRST_NAME, HIRE_DATE FROM EMPLOYEES
WHERE JOB_ID IN('SA_MAN','IT_PROG');

4. Display employees who joined after 1st January 2008.

Query -- > SELECT EMPLOYEE_ID,FIRST_NAME, LAST_NAME
FROM EMPLOYEES
WHERE HIRE_DATE >'2008-01-01';

5.  Display details of employee with ID 150 or 160.

Query -- > SELECT *FROM EMPLOYEES
WHERE EMPLOYEE_ID IN(150,160);

Query -- > SELECT *FROM EMPLOYEES
WHERE EMPLOYEE_ID=150 OR EMPLOYEE_ID=160;


6. Display first name, salary, commission pct, and hire date for employees with salary less than 10000.

Query -- > SELECT FIRST_NAME, SALARY, COMMISSION_PCT, HIRE_DATE 
FROM EMPLOYEES 
WHERE SALARY<10000;

7. Display job Title, the difference between minimum and maximum salaries for jobs with max salary in the range 10000 to 20000.

Query -- > SELECT JOB_TITLE, MAX_SALARY-MIN_SALARY AS DIFF
     FROM JOBS
     WHERE MAX_SALARY BETWEEN 10000 AND 20000;

8. Display first name, salary, and round the salary to thousands.

Query -- > SELECT FIRST_NAME, ROUND(SALARY,-3)
                   FROM EMPLOYEES;

9. Display details of jobs in the descending order of the title.

Query -- >  SELECT *FROM JOBS
ORDER BY JOB_TITLE DESC;

10. Display employees where the first name or last name starts with S.

Query -- > SELECT *FROM EMPLOYEES 
WHERE FIRST_NAME LIKE 'S%' OR LAST_NAME LIKE 'S%';

11. Display employees who joined in the month of May.

Query -- > SELECT *FROM EMPLOYEES 
WHERE TO_CHAR(HIRE_DATE,'MM')='05';

12. Display details of the employees where commission percentage is null and salary in the range 5000 to 10000 and department is 30.

13. Display first name and date of first salary of the employees.

14. Display first name and experience of the employees.

15. Display first name of employees who joined in 2001.
16. Display first name and last name after converting the first letter of each name to upper case and the rest to lower case.
17. Display the first word in job title.
18. Display the length of first name for employees where last name contain character ‘b’ after 3rd 
position.
19. Display first name in upper case and email address in lower case for employees where the first 
name and email address are same irrespective of the case.
20. Display employees who joined in the current year.
21. Display the number of days between system date and 1st January 2011.
22. Display how many employees joined in each month of the current year.
23. Display manager ID and number of employees managed by the manager.
24. Display employee ID and the date on which he ended his previous job.

25. Display number of employees joined after 15th of the month.

Query -- > SELECT COUNT(*) FROM EMPLOYEES 
WHERE TO_CHAR(HIRE_DATE,'DD')>'15';

26. Display the country ID and number of cities we have in the country.
27. Display average salary of employees in each department who have commission percentage.
28. Display job ID, number of employees, sum of salary, and difference between highest salary and 
lowest salary of the employees of the job.
29. Display job ID for jobs with average salary more than 10000.
30. Display years in which more than 10 employees joined.
31. Display departments in which more than five employees have commission percentage.
32. Display employee ID for employees who did more than one job in the past.
33. Display job ID of jobs that were done by more than 3 employees for more than 100 days.
34. Display department ID, year, and Number of employees joined.
35. Display departments where any manager is managing more than 5 employees.
36. Change salary of employee 115 to 8000 if the existing salary is less than 6000.
37. Insert a new employee into employees with all the required details.
38. Delete department 20.
39. Change job ID of employee 110 to IT_PROG if the employee belongs to department 10 and the 
existing job ID does not start with IT.
40. Insert a row into departments table with manager ID 120 and location ID in any location ID for 
city Tokyo.
41. Display department name and number of employees in the department.
42. Display job title, employee ID, number of days between ending date and starting date for all 
jobs in department 30 from job history.
43. Display department name and manager first name.
44. Display department name, manager name, and
city.
45. Display country name, city, and department name.
46. Display job title, department name, employee last name, starting date for all jobs from 2000 to 
2005.
47. Display job title and average salary of employees
48. Display job title, employee name, and the difference between maximum salary for the job and 
salary of the employee.
49. Display last name, job title of employees who have commission percentage and belongs to 
department 30.
50. Display details of jobs that were done by any employee who is currently drawing more than 
15000 of salary.
51. Display department name, manager name, and salary of the manager for all managers whose 
experience is more than 5 years.
52. Display employee name if the employee joined before his manager.
53. Display employee name, job title for the jobs employee did in the past where the job was done 
less than six months.
54. Display employee name and country in which he is working.
55. Display department name, average salary and number of employees with commission within 
the department.
56. Display the month in which more than 5 employees joined in any department located in 
Sydney.
57. Display details of departments in which the maximum salary is more than 10000.
58. Display details of departments managed by ‘Smith’.
59. Display jobs into which employees joined in the current year.
60. Display employees who did not do any job in the past.
61. Display job title and average salary for employees who did a job in the past.
62. Display country name, city, and number of departments where department has more than 5 
employees.
63. Display details of manager who manages more than 5 employees.
64. Display employee name, job title, start date, and end date of past jobs of all employees with 
commission percentage null.
65. Display the departments into which no employee joined in last two years.
66. Display the details of departments in which the max salary is greater than 10000 for employees 
who did a job in the past.
67. Display details of current job for employees who worked as IT Programmers in the past.
68. Display the details of employees drawing the highest salary in the department.
69. Display the city of employee whose employee ID is 105.
70. Display third highest salary of all employees	



PL/SQL Programs
(Write stored procedures for all the given problems)
1. Write a program to interchange the salaries of employee 120 and 122.
2. Increase the salary of employee 115 based on the following conditions: If experience is more 
than 10 years, increase salary by 20% If experience is greater than 5 years, increase salary by 
10% Otherwise 5% Case by Expression:
3. Change commission percentage as follows for employee with ID = 150. If salary is more than 
10000 then commission is 0.4%, if Salary is less than 10000 but experience is more than 10 
years then 0.35%, if salary is less than 3000 then commission is 0.25%. In the remaining cases 
commission is 0.15%.
4. Find out the name of the employee and name of the department for the employee who is 
managing for employee 103.
5. Display missing employee IDs.
6. Display the year in which maximum number of employees joined along with how many joined 
in each month in that year.
7. Change salary of employee 130 to the salary of the employee with first name ‘Joe’. If Joe is not 
found,then take average salary of all employees. If more than one employee with first name ‘Joe’ is found,then take the least salary of the employees with first name Joe.
8. Display Job Title and Name of the Employee who joined the job first day.
9. Display 5th and 10th employees in Employees table.
10. Update salary of an employee based on department and commission percentage. If department is 40 increase salary by 10%. If department is 70 then 15%, if commission is more than .3% then 5% otherwise 10%.
11. Create a function that takes department ID and returns the name of the manager of the department.
12. Create a function that takes employee ID and return the number of jobs done by the employee in the past.
13. Create a procedure that takes department ID and changes the manager ID for the department 
to the employee in the department with highest salary. (Use Exceptions).
14. Create a function that takes a manager ID and return the names of employees who report to 
this manager. The names must be returned as a string with comma separating names.
15. Ensure no changes can be made to EMPLOYEES table before 6am and after 10pm in a day.
16. Create a Trigger to ensure the salary of the employee is not decreased.


	 

