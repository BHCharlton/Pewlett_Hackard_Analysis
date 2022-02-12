# Pewlett_Hackard_Analysis
## Overview of the Analysis
Our client, Pewlett Hackard, is a large company that is planning ahead for the upcoming retirements of several employees over the new few years.  They want to "future-proof" the company by finding out how many people will likely be retiring in that time, and who of those employees will be eligible for the retirement packages their company has to offer.  Pewlett Hackard wants to make sure that the company is ready for swift turnover so that appropriate decisions can be made in regards to hiring, training, and retirements. In order to ensure a smooth transition, the following information was obtained for the analysis:
1. A compilation of the employees within a specific age range who and most likely to retire
2. Identify those employees who are eligible for retirement benefits
4. Determine the number of those who will be retiring
5. Create of a list of retirees grouped by each individual department
6. Find employees who eligible to participate in a mentorship program

## Results
These are the initial data sets that were used in the analysis:
* departments
* dept_emp
* dept_manager
* employees
* salaries
* titles

In this analysis, PostgreSQL relational database system was used through the pgAdmin platform as a way to evaluate, combine, and develop new data sets needed for the analysis.  To begin, the entity relationship diagram (ERD) below was created to see how each data set related to one another, and then be able to determine what information was specifically needed to develop new data sets containing the desired information.

![ERD](https://raw.githubusercontent.com/BHCharlton/Pewlett_Hackard_Analysis/main/EmployeeDB.png)

### Retiree Count Analysis
Using the ERD as a guide, data sets were developed based on the instructions. The analysis was based on defining aging population with birth date between years 1952 to 1955 and hire date between years 1985 to 1988. The analysis returned 133, 776 results, which seems quite high.  However, it should be noted that this data set includes multiple titles held by the same employee due to the fact that they have switched titles within the company throughout their tenure.  Thus, this number is not an accurate representation of the number of retirees.

To eliminate duplicate entries created by the original query, an additional analysis was run using a the distinct_on filter to give us a more practical idea of how many employees will actually be retiring based upon their current position only.

![unique](https://raw.githubusercontent.com/BHCharlton/Pewlett_Hackard_Analysis/main/Unique.PNG)

Is was also important to group the retirees by title to have a clear understanding of which roles would need to be filled, and how many.  There were seven groupings in the data set.

![titles](https://github.com/BHCharlton/Pewlett_Hackard_Analysis/blob/main/retiring_titles.PNG)

### Mentorship Program Eligibility
There will be many people moving on from Pewlett Hackard in the next few years, and it will be important to help prepare new and existing employees for the years ahead.  To be eligible, the employee must be planning to retire, and have been born between January 1 and December 31 of 1965.


### Observations
* There will be 72, 458 who will be eligible for retirement over the next few years
* Seventy percent of those retiring will be from senior level positions, which will likely result in internal title promotion
* There are 1, 149 employees who would be eligible to assist in the mentorship program

## Summary
It is important to plan ahead for the upcoming "silver tsunami" that Pewlett Hackard will be soon faced with.  The workforce is strained right now, and it may be difficult to find enough qualified candidates to assume all the roles that will need to be filled in order to keep business running efficiently.  But not every retiree is simply going to be walking out the same day, and there will be many experienced senior staffers over the next couple of years that should be able to help train those who are looking to move up within the company as well as new employees who are just beginning with Pewlett Hackard.




