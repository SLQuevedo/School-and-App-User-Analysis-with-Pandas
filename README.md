# pandas-challenge

I completed both PyCity and HeroesOfPymoli challenges. On the rubric it says that you will only be looking at one, if this is true please grade PyCity Schools. Both projects' codes are annotated, so I hope you are able to understand my methodology. 

# PyCity Schools 

# Opening the Project
Inside the PyCitySchool folder there is a file called PyCitySchools.ipynb, please open this file with Jupyter Notebook. I will explain each part of my code as they appear in this ReadMe file. All of my data is rounded to two decimal places for ease of reading.

# Methods 
First I merged the students data with the school data, so that I can pull all of the data I would need from a single source. 

Next I created a dataframe that summaraizes the school district data. I found the total schools, total students, total budget, average math score, average reading score, % of students passing math, % students passing reading and the % of students passing overall for the entire district. 

I then group my combined data by the school name and found each schools type (district or charter), total students attending, the school's budget, the school's budget per student, average math score, average reading score, % of students passing math, % students passing reading and the % of students passing overall. This creates our School Summary dataframe.

Then I sorted my School Summary in descending order to find the top 5 performing schools. I also sort my School Summary in ascending order to find the bottom 5 performing schools. 

In the next section I filter my student data to only include a certain grade level (9th, 10th, 11th, 12th) and group by the school name because I want to create a summary of the average math and reading scores of each grade for each school.

I then set up bins for how much each school was spending per student, so I can look at the relationship between grades/passing rates and how much is spent on each student. I checked the min/max values for the per student budget so I can make sure my bins are within a reasonable range. After grouping my School Summary by the spending bins, I calculate the averages for math/reading scores, and the average % of students passing math/reading/overall within each bin.  

Next I create bins based off school size, so I can see the relationship, if any, between school size and grades/passing rates. I do the same procedure as before and calculate the averages for grades and % of students passing for each size bin. 

Lastly, I created a dataframe showing the average scores and average % passing by school type. To do this I group my School Summary by school type and calculate the averages based off the school type. 

# Results and Analysis
From my analysis I noticed that overall math scores tend to be lower than reading scores. I also noticed that charter schools had better average grades and passing percents than schools within the district. Within each grade level for each school there doesn't seem to be any significant changes between them. The grades and passing rates for small schools seem to be higher than those of large schools. One thing I found interesting was that schools that had a smaller budget per student actually performed better than those with a larger budget per student. I would like to do additional analysis to see a relationship between the student budget and school size because I want to see if larger schools have more or less budget per student. I would also want to analyze the relationship between per student budget/total budget and if a school is district or charter. If we had the data we could also perform analysis for each school and the socioeconomic status of the student body. 


# Heroes of Pymoli

# Opening the Project
Inside the HeroesOfPymoli folder there is a file called HeroesOfPymoli.ipynb, please open this file with Jupyter Notebook. I will explain each part of my code as they appear in this ReadMe file. Percents in my data is rounded by 2 decimal places for ease of reading. 

# Methods

First I find the total number of players. I do this by using the nunique function to make sure I don't count people who made multiple purchases more than only once. I will reference my variable for total players in the future. I create this into a dataframe as per the example. I could have also done a print statement with my single variable. 

Next I create a summary table from the purchase data. For all pruchases, I calculate the average price of items, total number of purchases, and the total revenue. I put these values into a data frame.

I then want to look at gender demographics by grouping the purchase data by gender. I find the number of players per gender and what percent of players each gender is. I put these values into a data frame. 

Next I want to create a data frame that analyzes purchases by gender. Using the same grouping as before, I find how many purchases each gender made using the count function. I also calculate the average purchase price and total amount purchased for each gender. I also calculate the average purchase per person within our gender grouping by dividing the total amount purchased by the total amount of each gender. I put all of these values into a dataframe.

Then I want to analyze the age demographic of the players. To do this I place my purchase data into bins that are split into 8 groups with ages that range from 0-40+ and group by the age groups. I find how many unique players are in each age group and then I divide the result by the total amount of players. This calculates the percent of players in a certain age group. I place the count and percent of players in each age group into a data frame. 

Using the same bins as before, I find how many purchases were made, the average price of the item purchased, the total amount spent and the average amount a person spent in each age group. I put all of these values into a data frame.

Next I want to see the top 5 spenders within the purchase data. First I group my data by screen name (SN) and count how many items each person has purchased. I then calculate the average price of the item each player bought and I find how much each player spent in total. I put all of these values into a data fram and order them by descending order to get the top 5.

Lastly, I find the most popular and most pofitable items. I start this by grouping my data by item ID and item name. I use the count function to count how many of each item was sold. I then find how much each item made in total. To find the item price I divide the total amount the item made and then divide by the purchase count. I create a data frame sorted by descending purchase count to find the most popular items. I create another data frame that is sorted by descending total purchase value to find the most profitable items.

# Results and Analysis

In conclusion, a large majority of the player base are males and/or in the 20-24 years old age group. It it also of note that players in these demographics spent the most money in the game by far. This could be due to the our data set being saturated with these players, so it is unclear if people in the other gender or age categories spend a comparable amount based on their size. It also seems that the more expensive items were the most popular and the most profitable. It would be interesting to compare each items useage stats in game with how many were purchased and how much money it made. 

-Sierra Quevedo
