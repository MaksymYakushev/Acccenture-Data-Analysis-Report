# Acccenture Project

<img src="https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Data/logo.png" width="420" height="200">

.....

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

[**Meet your Accenture team**](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task1/Internal%20stakeholder%20chart.pdf)

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

So, let’s have a look at what data you have to work with. The client has sent through:

- **7 data sets** - each data set contains different columns and values.   
- **A data model** - this shows the relationships between all of the data sets, as well as any links that you can use to merge tables.  

**Requirements gathering**

First step is to use this data model to identify which datasets will be required to answer your business question - which is to to figure out the top 5 categories with the largest popularity.

[Data Model](https://github.com/MaksymYakushev/Acccenture-Data-Analysis-Report/blob/main/Task2/Data%20model.pdf)

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

To clarify why you made this selection:  
- The brief carefully it states that the client wanted to see “An analysis of their content categories showing the top 5 categories with the largest popularity”.
- As explained in the data model, popularity is quantified by the “Score” given to each reaction type.
- We therefore need data showing the content ID, category, content type, reaction type, and reaction score.
- So, to figure out popularity, we’ll have to add up which content categories have the largest score.

**Data Cleaning**  

Data cleaning is a common and very important task when working with data.

**First:** Open the three data sets below

Reactions
Content
Reaction types


## Task 3

## Task 4
