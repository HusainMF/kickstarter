# kickstarter Project

# Cleaning Process:
1- Filtered the category "Games".
2- Merged the two sub-categories "Borad games & cards" (one of them has a spelling error)
3- Dropped the "URL" column
4- Dropped the nulls in the "Location" column
5- Deleted the misslabeled value in the "Funded Percentage" column (only 1 row)
6- Converted the "Goal" and "Pledged" columns to dollar curency.
7- Converted the "Funded Percentage" column to percentage format (it was in just numbers/decimal)


# Data Dictionary
The columns:
   | Columns Name  |              Describtion                | Data Type |
   |---------------|-----------------------------------------|-----------|
   | Project ID   b|  all the project IDs in the data        | integer   |
   | Name          |  all the names of each project          | String    |
   | Category      |   the category "Games"                  | String    |
   | Sub Category  |  the sub category that we will be 
                    focus on which is "Board Games & Card"   | String    |
   | Location      |  the country name and its state         | String    |
   | Status        |  the status of the project,
                    whether it success, failed...            | String    |
   | Goal          | is the goal or the capital that each
                    project need to start the business       | Integer   |
   | Pledged       | the amount of money each project earned | Integer   |
   | funded percentage | the amount of the pledged over 
                    the goal amount                          | Float     |
   | backers      | the number of backers                   | Integer   |
   | Funded Date  | the last date when the creator recieved
                    the funds from the backers               | Date      |
   | Levels       | The number of levels that the backers
                    can fund to the creator                  | Integer   |
   | Reward Levels| How much money the backers can fund to
                    the creator                              | Integer   |
   | Updates      | How many times each project did an update | Integer |
   | Comments     | Number of comments each project has     | Integer   |
   | duration     | The length of the duration              | Float     |
