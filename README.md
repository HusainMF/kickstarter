# kickstarter Project

# Cleaning Process:
1- Filtered the category "Games".

2- Merged the two sub-categories "Borad games & cards" (one of them has a spelling error).

3- Dropped the "URL" column ---> we don't need it in our analysis.

4- Dropped the nulls in the "Location" column ---> we only have 11 missing out of 553 total board game campaigns (~2%), so the impact is very small.

5- Deleted the misslabeled value in the "Funded Percentage" column (only 1 row) ---> can't contribute meaningful insights.

6- Removed duplicate (one row, project id: 2143119805) ---> to maintain data accuracy and improves workflow in tasks such as sorting, filtering, and summarizing.

7- Change the name of the column (Goal) to Requested Funding ---> for easier understanding.

8- Change the name of the column (pledged) to Received Funding ---> for easier understanding.

9- Converted the "Requested Funding" and "Received Funding" columns to dollar curency ---> to make it more understandable and readable. 

10- Converted the "Funded Percentage" column to percentage format (it was in just numbers/decimal) ---> to make it more understandable and readable.

11- Converted the "duration" column to number with 0 decimal format ---> to make it more realistic because it calculates the duration in days

12- Add Duration_Group, Month, Is_Successful, and Goal_Range columns ---> To facilitate comparison and analysis


# Data Dictionary
The columns:
   | Columns Name  |              Describtion                | Data Type |
   |---------------|-----------------------------------------|-----------|
   | Project ID   b|  all the project IDs in the data        | integer   |
   | Name          |  all the names of each project          | String    |
   | Category      |   the category "Games"                  | String    |
   | Sub Category  |  the sub category that we will be focus on which is "Board Games & Card"   | String    |
   | Location      |  the country name and its state         | String    |
   | Status        |  the status of the project, whether it success, failed...    | String    |
   | Goal          | is the goal or the capital that each project need to start the business       | Integer   |
   | Pledged       | the amount of money each project earned | Integer   |
   | funded percentage | the amount of the pledged over the goal amount                          | Float     |
   | backers      | the number of backers                   | Integer   |
   | Funded Date  | the last date when the creator recieved the funds from the backers               | Date      |
   | Levels       | The number of levels that the backers can fund to the creator                  | Integer   |
   | Reward Levels| How much money the backers can fund to the creator                              | Integer   |
   | Updates      | How many times each project did an update | Integer |
   | Comments     | Number of comments each project has     | Integer   |
   | duration     | The length of the duration              | Float     |
   | Duration_Group| Categorizes each campaign based on how many days it lasted | Categorical 
   | Month        | Extracted from the campaign launch date to identify the month it started | String
   | Is_Successful| Indicates whether a campaign was successful or not | Binary 
   | Goal_Range | Groups campaigns by how much funding they aimed to raise | Categorical 

