# Pewlett Hackard Analysis

## Overview

The purpose of this analysis is to address the aging workforce at Pewlett Hackard. In order to account for this, I have been tasked with identifying employees who are most likely to retire soon by their title and employees who could transition to a part time mentorship program compared to just retiring. I used PostgreSQL to complete my analysis.

### Current Storage of Data

Pewlett Hackard currently stores their employee data in 6 different csv files. Here is the entity relationship diagram of those datasets.

![employee_db](https://github.com/Wall-E28/pewlett_hackard_analysis/blob/master/EmployeeDB.png)

## Results

### Retiring Pewlett Hackard Employees by Titles

The current criteria for this analysis is to find employees born between 01/01/1952 and 12/31/1955. The major takeaways from this analysis are:

1. There are 90,396 employees who are likely to retire soon
2. 57,668 employees are senior level employees
3. 43,636 employees are engineers
4. 40,497 employees are staff
5. Only 2 managers need to be replaced

![retiring_titles](https://github.com/Wall-E28/pewlett_hackard_analysis/blob/master/Data/retiring_titles.csv)

### Mentorship Eligibility

The current criteria for this analysis is to find employees born in 1965 and have current roles with no termination dates. The major takeaways from this analysis are:

1. There are 1,550 employees eligible for the mentorship program
2. 741 employees are senior level employees
3. 748 employees are engineers
4. 724 employees are staff
5. There are no managers eligible for this program based on the current criteria

![mentorship_eligibility](https://github.com/Wall-E28/pewlett_hackard_analysis/blob/master/mentorship_eligibility.png)

## Summary

Looking at both of these analyses, we can see that of the 90,396 potential spaces that need to be filled due to retirement, there are only 1,550 employees currently eligible to mentor new employees to fill those positions. That means there is one mentor for every 58 new employees. More importantly, there is only 741 senior level employees eligible to mentor 57,668 vacancies. That means there is one senior level mentor for every 77 new senior level employee.

If we change to criteria for the mentorship program to employees born between 1962 and 1965 those numbers drop to one mentor for every 1.6 new employees and one senior level mentor for every 2.3 new senior level employees. By widening the pool of eligible employees this program has a strong chance at not only surviving, but thriving. More employees will be incentized to mentor if they are only mentoring 2 to 3 people instead of 50+ people. Also, new employees will gain more from one on one mentoring compared to group mentoring that would likely happen in the first situation. While not everyone will want to praticipate in this program, the more current employees who are eligible to better to see this program succeed.

![mentorship_updated](https://github.com/Wall-E28/pewlett_hackard_analysis/blob/master/Data/mentorship_eligibility_updated.csv)