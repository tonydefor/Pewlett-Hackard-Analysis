# Pewlett-Hackard-Analysis

## Overview of Analysis

- Using the ERD's we created in this module as a reference and our knowledge of SQL queries, we created a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions— we used the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, we also used the COUNT() function to create a table that has the number of retirement-age employees by most recent job title. Finally, because we want to include only current employees in our analysis, we were sure to exclude those employees who have already left the company.


## Results

- We the excluded employees that have already left the company by filtering on the to_date to keep only those date that are equal to 9999-01-01. This enabled us to create a new table which we named Unique titles. We found 133,776 retiring employees, but there are duplicate entries for some employees because they have switched titles over the years, the results shows us only 72,458 employees ready to retire.

<img width="822" alt="retirement_title" src="https://user-images.githubusercontent.com/47859209/195966910-e8b1a3ab-bfc4-4654-8ebe-9b04004dd2fd.png">

<img width="821" alt="unique_titles" src="https://user-images.githubusercontent.com/47859209/195966974-60ba1d28-4526-49fa-b5cb-47c9c4b0cbcf.png">


- By creating another query and retrieving the number of titles from the Unique titles table, we in turn created another table by using the group function. This sortred out the most recent employees who are retiring.

<img width="804" alt="retirment_most_recent" src="https://user-images.githubusercontent.com/47859209/195967024-aeda8da4-6312-4e15-b9a3-5b3b24d21f05.png">

## Summary

### Mentorship Eligibility

- We retrieved some similar columns from our Employees ttable, Department Employee Table and joined our titles column from our titles table. We then filtered the data from the to_date column for all the current employee. After that we sorted out our table by employee number, This resulted us in determining the mentorship eligibility for our employees. 

<img width="822" alt="mentorship_eligibility" src="https://user-images.githubusercontent.com/47859209/195967211-7b9b8171-0653-4966-b491-78ea4303dbbd.png">

Overall, our analyses pointed out some issues of concern:

- We were able to deduce that there are no salary increases.

- There are repeated names of employees and in different departments, which makes us believe that the databases of the employees and departments have not been updated based on their last position.

- The active managers are less than the number of departments, which makes us think that there are departments without a manager and the rest have double the burden of having to deal with those departments.
There are only 1,549 employees with the possibility of a Mentoring Program.


