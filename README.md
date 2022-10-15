# Pewlett-Hackard-Analysis

## Overview

- Using the ERD's we created in this module as a reference and our knowledge of SQL queries, we created a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions— we used the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, we also used the COUNT() function to create a table that has the number of retirement-age employees by most recent job title. Finally, because we want to include only current employees in our analysis, we were sure to exclude those employees who have already left the company.

<img width="822" alt="retirement_title" src="https://user-images.githubusercontent.com/47859209/195966727-e903a1ae-9c53-4948-a829-da362724fe66.png">
