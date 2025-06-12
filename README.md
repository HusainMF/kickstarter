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
2- | Name          |  all the names of each project          | String    |
3- | Category      |   the category "Games"                  | String    |
4- | Sub Category  |  the sub category that we will be 
                    focus on which is "Board Games & Card"   | String    |
5- | Location      |  the country name and its state         | String    |
6- | Status        |  the status of the project,
                    whether it success, failed...            | String    |
7- | Goal          | is the goal or the capital that each
                    project need to start the business       | Integer   |
8- | Pledged       | the amount of money each project earned | Integer   |
9- | funded percentage | the amount of the pledged over 
                    the goal amount                          | Float     |
10- | backers      | the number of backers                   | Integer   |
11- | Funded Date  | the last date when the creator recieved
                    the funds from the backers               | Date      |
12- | Levels       | The number of levels that the backers
                    can fund to the creator                  | Integer   |
13- | Reward Levels| How much money the backers can fund to
                    the creator                              | Integer   |
14- | Updates      | How many times each project did an update | Integer |
15- | Comments     | Number of comments each project has     | Integer   |
16- | duration     | The length of the duration              | Float     |
