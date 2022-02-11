# Pewlett_Hackard_Analysis
## Overview of the Analysis
Our client, Pewlett Hackard, is a large company that is planning ahead for the upcoming retirements of several employees over the new few years.  They want to "future-proof" the company by finding out how many people will likely be retiring in that time, and who of those employees will be eligible for the retirement packages their company has to offer.  Pewlett Hackard wants to make sure that the company is ready for swift turnover so that appropriate decisions can be made in regards to hiring, training, and retirements. In order to ensure a smooth transition, the following information was obtained for the analysis:
1. A complilation of the employees within a specific age range who and more likely to retire
2. Identify those employees who are ellibile for retirement benefits
3. Determine the number of who will likely be retiring in each department
4. Create of a list of retirees broken down into each department

## Results
These are several of the different data sets that were used in the analysis:
* departments
* dept_emp
* dept_manager
* employees
* emp_info
* emp_count
* retirement_titles
* retirement_info
* salaries

In this analysis, the PostgreSQL relational database system was used through pgAdmin to as a way to develop, combine, and create new data sets needed for the analysis.  To begin, the entity relationsip diagram (ERD) below was created to see how each data set related to one another, and then be able to determine what information was specifically needed to develop new data sets containing the desired information.

![ERD](https://raw.githubusercontent.com/BHCharlton/Pewlett_Hackard_Analysis/main/EmployeeDB.png)

This shows how we
