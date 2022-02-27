# Pewlett-Hackard-Analysis

## Overview 

The purpose of this analysis was to prepare Bobby's manager for the increase in retirement of his current employees by identifying the employees that have reached the age of retirement and determining which employees are eligible for a mentorship program which could fill those positions. 

### Analysis
[SQL](https://github.com/Lan-kdl/Pewlett-Hackard-Analysis/blob/main/Queries/Employee_Database_challenge.sql)

### Data
[Retirement Titles](https://github.com/Lan-kdl/Pewlett-Hackard-Analysis/blob/main/Data/retirement_titles.csv)
[Unique Titles](https://github.com/Lan-kdl/Pewlett-Hackard-Analysis/blob/main/Data/unique_titles.csv)
[Retiring Titles](https://github.com/Lan-kdl/Pewlett-Hackard-Analysis/blob/main/Data/retiring_titles.csv)
[Mentorship Eligibility](https://github.com/Lan-kdl/Pewlett-Hackard-Analysis/blob/main/Data/mentorship_eligibilty.csv)


## Results

- Of all of the department titles, the titles with the most employees of retirement age are senior engineer with 25,916 employees and senior staff with 24,926 employees. 
- Of all the employees of retirement age, less than 1% (0.00276%) are managers. Out of all employees at retirement age, only 1.5% are assisstant engineers. 

![Titles_Retiring](https://user-images.githubusercontent.com/95589611/155901567-8f1f698a-2934-4400-a180-08a0c490e56f.png)

Data: [Retiring Titles](https://github.com/Lan-kdl/Pewlett-Hackard-Analysis/blob/main/Data/retiring_titles.csv)

- There are 1,149 employees who are eligeable for a mentorship program. 
- The title with the most available for a mentorship program is senior staff with 456 employees available, while the field with the least amount of eligible employees is assistant engineer with only 67 employees available.
 
![mentorship_eligibility](https://user-images.githubusercontent.com/95589611/155901588-ad8ff7aa-e1f7-46a7-be72-77d44e27d839.png)

Data: [Mentorship Eligibility](https://github.com/Lan-kdl/Pewlett-Hackard-Analysis/blob/main/Data/mentorship_eligibilty.csv)

## Summary: 
As the "silver tsunami" begins to make impact, 72,458 roles will need to be filled: 

![count_of_roles](https://user-images.githubusercontent.com/95589611/155901624-a6edc39f-07dd-4b58-8894-e849f7011e59.png)

Unfortunatley, there are not enough retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees. There are far more roles that will need to be filled than there are employees to mentor those who might fill those roles. For example, there are 25,916 senior engineering roles that might need to be filled once the "silver tsunami" hits while there are only 259 of those employees who are able to mentor the next generation. In order to fill those positions, the mentors would have to take on just over 100 apprentices each which is not practicle. Even the senior staff, which has the most employees eligible for mentoring would still have to take on 57 apprentices each.

### Table suggestions

In order to better prepare Bobby's manager for the "silver tsunami" I suggest making a table which would display all current employees which have been with the company for over 10 years. You could use the current date of employeement and the from_date to determine these employees. I believe that this table would be beneficial because you could expand the range of employees who might be elegible for a promotion without mentorship. 

![current_emp_10_yrs](https://user-images.githubusercontent.com/95589611/155903404-023da695-2795-4a38-9553-9eda5fcea2f8.png)
![current_emp_10_yr_titles](https://user-images.githubusercontent.com/95589611/155903408-bf53093f-18b4-44c1-a8bf-a00abe05a2bf.png)

Another table that I would recommend would be one that list those with mentorship eligibility that have worked other positions than the one they are currently hired in. This would be useful because you could use those employees to mentor the next generation of employees in a department other than their current department of employeement. 

![multiple_titles](https://user-images.githubusercontent.com/95589611/155903436-56fe3e97-3244-4f4f-8be3-4488be4a5bab.png)
![multiple_titles_graph](https://user-images.githubusercontent.com/95589611/155903441-216bf99c-3cec-434b-844d-bdfc5a2d967f.png)

I might also suggest a query that identifies those employees just under retirment age, though still seasoned enough to either be promoted or mentors to the next generation of employees. 

![almost_retirement](https://user-images.githubusercontent.com/95589611/155903450-4ea92f76-35b7-4730-bed0-fd49ad342bab.png)

