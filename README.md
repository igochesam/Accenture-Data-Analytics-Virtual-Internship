# Accenture-Data-Analytics-Virtual-Internship
The virtual internship programme was divided into four parts. 


## Task 1
The first task was all about getting familiar with the responsibilities of a Data Analyst at Accenture, a typical project team structure, and how to review a client project brief. I needed to read and analyze the [client project brief](https://github.com/igochesam/Accenture-Data-Analytics-Virtual-Internship/files/13595980/Data_Analytics.Client.Brief.pdf) to understand the client and business problem, identify the requirements to be delivered, and identify which tasks to focus on as a data analyst.
After carefully studying the brief, I was able to gain the following insights:
1. The client has reached a massive scale within recent years and does not have the resources internally to handle it.
2. I needed to analyze sample data sets with visualizations to understand the popularity of different content categories


## Task 2
The second task required me to identify which datasets would be required to answer the client’s business question, to clean the datasets and merge them to prepare the data for analysis, and finally to determine the answer to the client’s business question. In general, the task was about how to clean, model and analyze data to create valuable insights for the client. The client had sent 7 data sets, each of which contains different columns and values; a data model showing the relationships between all of the data sets, as well as any links that you can use to merge tables. This task involved requirements gathering, data cleaning, and data modelling.

So I swung into action by studying the [data model](https://github.com/igochesam/Accenture-Data-Analytics-Virtual-Internship/files/13596057/Data.model.pdf) and a thorough consideration helped me see that I needed just three datasets for the analysis, namely Content, Reactions, and ReactionTypes. They can be found in the uploaded files. This decision was made simply because the brief carefully  states that the client wanted to see “An analysis of their content categories showing the top 5 categories with the largest popularity”, and as explained in the data model, popularity is quantified by the “Score” given to each reaction type. I therefore needed data showing the content ID, category, content type, reaction type, and reaction score. So, to figure out popularity, it made sense to add up which content categories have the largest score.

I then proceeded to clean the data by deleting columns that were irrelevant like the URL column from the Content dataset. There were of course empty rows in the Reactions dataset but these were easily dealt with by deleting them, considering that they did not constitute a significant percentage in relation to the entire dataset. I also took note of similar names of categories like "animals" and Animals, and made sure that I gave such categories the same name so they don't incorrectly appear as different categories.

Next, I created a final data set by merging the three tables together, as can be seen in the Excel file in the uploads. The Reaction table was used as the base table, and then the relevant columns were joined from Content data set, and next the Reaction Types data set. This was done using the VLookUp formula. 

Having done this, it was easy to figure out the top 5 performing categories by addinig up the total scores for each category using the SUMIF formula. The end result can be seen in the Excel file named Accenture in the file uploads.


## Task 3
This task was all about data visualisation and storytelling. This [file](https://github.com/igochesam/Accenture-Data-Analytics-Virtual-Internship/files/13596347/Data.Analytics.template.-.Task.3_final.pptx) contains a presentation to this effect.

## Task 4
This involved a video presentation to the client on the steps taken and the insights gained from the data.
