# Pewlett_Hackard_Analysis
## Overview of the Analysis
Our client, Pewlett Hackard, is a large company that is planning ahead for the upcoming retirements of several employees over the new few years.  They want to "future-proof" the company by finding out how many people will likely be retiring in that time, and who of those employees will be eligible for the retirement packages their company has to offer.  Pewlett Hackard wants to make sure that the company is ready for swift turnover so that appropriate decisions can be made in regards to hiring, training, and retirements. In order to ensure a smooth transition, the following information was obtained for the analysis:
1. A complilation of the employees within a specific age range who and most likely to retire
2. Identify those employees who are ellibile for retirement benefits
4. Determine the number of those who will be retiring
5. Create of a list of retirees grouped by each individual department
6. Find employees who elibible to participate in a mentorship program

## Results
These are the initial data sets that were used in the analysis:
* departments
* dept_emp
* dept_manager
* employees
* salaries
* titles

In this analysis, PostgreSQL relational database system was used through the pgAdmin platform as a way to evaluate, combine, and develop new data sets needed for the analysis.  To begin, the entity relationsip diagram (ERD) below was created to see how each data set related to one another, and then be able to determine what information was specifically needed to develop new data sets containing the desired information.

![ERD](https://raw.githubusercontent.com/BHCharlton/Pewlett_Hackard_Analysis/main/EmployeeDB.png)

### 1. Retiree Count Analysis
Using the ERD as a guide, data sets were developed based on the instructions. The analysis was based on defining aging population with birth date between years 1952 to 1955 and hire date between years 1985 to 1988. The analysis returned 133, 776 results, which seems quite high.  However, it should be noted that this data set includes multiple titles held by the same employee due to the fact that they have switched titles within the company throughout their tenure.  Thus, this number is not an accurate representation of the number of retirees.

To elliminate duplicate entries created by the original query, an additional analysis was run using a the distinct_on filter to give us a more practical idea of how many employees will actually be retiring based upon their current position only.  This ultimately brings the number of expected retirees down to 72, 458

Is was also important to group the retirees by title to have a clear understanding of which roles would need to be filled, and how many.  There were seven groupings in the data set.

### 2. Mentorship Program Eligibility




