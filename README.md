# Acccenture Project

<img src="https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Data/logo.png" width="420" height="200">   

[Certificate](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task4/accenture.pdf)  

Welcome! This project is a web internship at Accenture as a Data analyst. This is my first project on GitHub and also my first web internship. Enjoy exploring the project!

## Task 1:  Project Understanding

First task is to read the brief from Social Buzz. [Read the brief](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task1/Data_Analytics%20Client%20Brief.pdf) to:
- Understand the client and business problem at hand.
- Identify the requirements that need to be delivered for this project.
- Identify which tasks you should focus on as a Data Analyst.

So, we are start our engagement with Social Buzz, we are running a 3 month initial project in order
to prove to them that we are the best firm to work with. They are expecting the following:
- An audit of their big data practice
- Recommendations for a successful IPO
- An analysis of their content categories that highlights the top 5 categories with the
largest aggregate popularity

Tasks to be delegated:
- Creation of an up-to-date big data best practices presentation
- Extraction of sample data sets using SQL
- On-site audit of their data-center
- Merging of sample data set tables
- Virtual session with Social Buzz team to present previous client success stories relevant
to them
- Preparation of best practice document for IPO
- Loading of sample data sets into Accenture sandbox database
- Technology architecture workshop with Social Buzz Data Team to understand their
technology landscape
- Stress testing of their technology to identify weak spots
- Communication with previous IPO companies within our client base for reference stories
- Analysis of sample data sets with visualizations
- Full documentation of the process that we can guide them through for IPO

**Completed a short knowledge check:**

**Question 1 of 2**

Which statement best describes the business problem that Accenture is tasked to address for this project?   
**Answer:** The client has reached a massive scale within recent years and does not have the resources internally to handle it.

**Question 2 of 2**

Which statement lists the three requirements that Accenture is tasked to fulfill for this project?  
**Answer:** Audit of big data practice, recommendations for IPO, analysis of popular content.

**Meet your Accenture team**   

📃[My team](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task1/Internal%20stakeholder%20chart.pdf)   

The team is structured in three key groups:

- **Industry experts** in the social media space to ensure we accurately understand Social Buzz’s sector.   
- **IPO experts** who will deliver on the IPO requirement.   
- **Data experts** who will provide Big Data insights and content category analysis.   

**Completed a short knowledge check:**  

**Question 1 of 1**
Which task out of these options is the most relevant to you as a data analyst, and therefore which one will you work on?  
**Answer:** Analysis of sample data sets with visualizations to understand the popularity of different content categories   

## Task 2: Data Cleaning & Modeling

**Let's dive into the data**

So, let’s have a look at what data have to work with. The client has sent through:

- **7 data sets** - each data set contains different columns and values.   
- **A data model** - this shows the relationships between all of the data sets, as well as any links that you can use to merge tables.  

**Requirements gathering**

First step is to use this data model to identify which datasets will be required to answer our business question - which is to to figure out the top 5 categories with the largest popularity.

📃[Data Model](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task2/Data%20model.pdf)

Definitions of different data types:
- **String** - Sequence of characters, digits, or symbols—always treated as text
- **UUID** - Universally Unique Identifiers
- **Array** - List with a number of elements in a specific order—typically of the same type
- **Integer** - Numeric data type for numbers without fractions
- **Timestamp** - Number of seconds that have elapsed since midnight (00:00:00 UTC), 1st January 1970 (Unix time)

**Completed a short knowledge check:**  

**Question 1 of 1**  Which three data sets will you need to complete your analysis?   
**Answer:** Reaction, Content, Reaction Types.  

**Data sets**  

To clarify why we made this selection:  
- The brief carefully it states that the client wanted to see “An analysis of their content categories showing the top 5 categories with the largest popularity”.
- As explained in the data model, popularity is quantified by the “Score” given to each reaction type.
- We therefore need data showing the content ID, category, content type, reaction type, and reaction score.
- So, to figure out popularity, we’ll have to add up which content categories have the largest score.

**Data Cleaning**  

Data cleaning is a common and very important task when working with data.

**First:** Open the three data sets below

📃[Reactions](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task2/Reactions.csv)    

📃[Content](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task2/Content.csv)   

📃[Reaction types](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task2/ReactionTypes.csv)     

**Second:** Clean the data by:   
- removing rows that have values which are missing,
- changing the data type of some values within a column, and
- removing columns which are not relevant to this task.

As a result should be three cleaned data sets. 

**Data Modelling**

**1. Create a final data set by merging your three tables together**  

We can use a “VLookUp” formula for merging three tables together. So I did it.

**2. Figure out the Top 5 performing categories**  

Using pivot tables, I got sums for each of the categories. I sorted by decreasing score and got top 5 performing categories.  

| Category | Score SUM |   
| -------- | -------- |  
| Animals | 74965 |
| Science | 71168 |
| Healthy eating | 69339 |
| Technology | 68738 |
| Food | 66676 | 

📃[The end result](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task2/CleanedDataset_TheTopFiveCategories.xlsx) it's one spreadsheet which contains: a cleaned dataset and the top 5 categories.

## Task 3: Data Visualization & Storytelling

**Build your presentation Structure**  
Here is a [template](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task3/Data%20Analytics%20template%20-%20Task%203_final.pptx) that Accenture use to create a presentation.   

**Completed a short knowledge check:**  

**Question 1 of 1**  Have you completed slides 2-6 in your presentation?  
**Answer:** Yes!  

**Create my charts**

The final step of this task is to populate slides 7 - 10 with my data insights.

We know that the client wants to understand the top 5 content categories. Have a think about what are the best ways to present this? In a pie chart? In a bar chart?  

There are also some other interesting insights that we might want to share with them. For example:   
- How many unique categories are there?
- How many reactions are there to the most popular category?
- What was the month with the most posts?   

**1. Insights**  

<img src="https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task3/Insights.jpg" width="620" height="340">

There are a total of 16 unique categories. 

With the help of pivot tables, the largest number of reactions to categories was determined. Сhose the largest one, that is "Animal". I got 1897 Reactions to content with animals. 

Also got the month with the most posts. To do this, I added a new column called "Month" to the [Cleaned Dataset](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task3/CleanedDataset_TheTopFiveCategories_forPresentation.xlsx) and determined in which month the post was made using the MONTH() formula. Then, using pivot tables, I determined the month with the largest number of posts. It was May.   

| Month | COUNT Month |   
| -------- | -------- |  
| 1 | 2126 |
| 2 | 1914 |
| 3 | 2012 |
| 4 | 1974 |
| 5 | 2138 |   
| 6 | 2021 |
| 7 | 2070 |
| 8 | 2114 |
| 9 | 2022 |
| 10 | 2056 |  
| 11 | 2034 |
| 12 | 2092 |

**2. Bar chart**  

<img src="https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task3/Graph1.jpg" width="620" height="340">

A bar chart is a great way to show popularity for Top 5 categories. It's visually clear and easy to understand.  

**3. Circle chart**

<img src="https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task3/Graph2.jpg" width="620" height="340">  


I reformat the data to show popularity in percents.

**Summary**   

During the data analysis, we prepared a presentation that reflects the key insights. The main task was to determine the five most popular categories of content. To do this, we used different visualization techniques, such as pie and bar charts, to visually represent these categories and their percentage content.

The analysis also revealed other interesting findings that may be useful to the client. We determined the number of unique categories, looked at the reactions to the most popular category and determined the month with the most posts.

All this data was visualized in clear and understandable graphs to make it easier for the client to understand. Using Excel, we provided effective information visualization. We are confident that our presentation provides information that will enable the client to better understand the dynamics and underlying trends in their content.  


📃[Full presentation](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task3/Data%20Analytics%20template%20-%20Task%203_final.pptx)   
📃[Updated Cleared Dataset](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task3/CleanedDataset_TheTopFiveCategories_forPresentation.xlsx)




## Task 4: Present to the Client

**Presentation tips**

When presenting to the client there are a few things that you should remember:
1. They may not all be familiar with data, so you need to make sure you talk to them in business-friendly language.   
2. You want to show them that you’ve understood their business and requirements, so use their terminology and language relevant to the task.   
3. This is your time to shine and to show them how great you are! Try to present your work with confidence and conviction, if you don’t feel confident talking about your results then it’s a good indication that you don’t understand them fully or may need to revisit the dataset! Speaking about your results should feel natural when you explain what you’ve done.  
4. A good presentation always takes a lot of preparation. The more you practice presenting your content, the more confident you will be when the time comes. Practice with your housemates, friends, family, anyone that is free! Ask for feedback and keep improving until you’re happy with your presentation and you’re confident in presenting your content.
