# Pewlett-Hackard-Analysis

## Overview
The purpose of this analysis is to figure out how many employees are going to be retiring soon from Pewlett Hackard. The analysis needed to find all the current employees that are soon to be retired and figure out which departments are going be hiring new employees. This also needed to show which employees could mentor the new employees that will be coming in. 

## Results
The results show that there are quite a few employees that are going to be eligible for retirment very soon so they will need to get ready to hire in case they decide to retire:
  -This code breaks down all employees by name that are eligible to retire soon and which department they work in, shown below.
  -Output of above code:
## Results
The analysis produced the following results:
- A list of retirement eligible employees, including their name and any title 
  they had held during their time at PH. This list was filtered from the main employee table using the 
  following query:
  
  ![Retiring_emp_query](https://user-images.githubusercontent.com/85318060/128639860-78079318-3954-49b1-8936-f8ceb6540197.png)
  
  This query used date of birth from 1952-1955, assuming those employees would be the ones ready for retirement in the coming years.
  
- Then using the following query this list was filtered down to only 
  include the most recent title for each staff member:
  
  ![Distinct_query](https://user-images.githubusercontent.com/85318060/128639582-2221a752-1c3a-4f92-982a-35daad4de6ef.png)
  
  This list showed a total of 90,398 employees.
  
- Using this list and the GROUP BY function, a list of the total number of employees in each title 
  was created.

  ![Title_count](https://user-images.githubusercontent.com/85318060/128639701-e17c9fbe-df57-4ed1-b86a-98b7b1b51cd8.png)
  
- Finally, it was decided that employees born in 1965 would be eligible for a mentorship program to 
  prepare for the wave of retiring staff that was coming. The following query was used to determine 
  how many eligible current employees were at PH:

  ![Mentorship_query](https://user-images.githubusercontent.com/85318060/128640043-759a87e3-6423-4a75-b840-89cc93645cc0.png)

  A total of 1,549 employees were determined to be mentorship eligible.
