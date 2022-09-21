# School_District_Analysis
Aggregate the data and showcase trends in school performance.

## Overview of Project
### Purpose
The purpose of this project was to assist Maria, the cheif data scienct for a city school district, analyze information from a variety of sources in a variety of formats. I will be assisting her analyze data on student funding and standardized test scores, as well as aggregate the data and showcase trends in school performance. 

## Analysis and Challenges

- For this project, I needed to utilize the three-phase process to prepare and organize my tasks and responsibilities. The three-phase process is: 

    1. Collect the data
    
    2. Prepare the data
    
    3. Analyze the data
    
- To begin my analysis, I needed to import the appropriate dependencies so that I could properly import the data. Now, I can collect the data, by creating a path to the dataset by using the os.path.join() function to tell Jupyter Notebook that I want to open the full student dataset, but since I don't know the direct path, use this function to find the dataset: full_student_data = os.path.join('../Resources/new_full_student_data.csv'). After generating the path, I can read the file byt using Pandas read.csv function. 

- Once the data was collected, I needed to prepare the data so that when I begin to run analyses, I don't run into any errors. Therefore, I needed to check for any missing data in the dataset. If there were any rows that had missing data, I needed to drop them from the dataset and then verify that they were dropped. I also needed to check to see if there were any duplicate rows. If there were duplicate rows I needed to drop those as well, and then verify that they were dropped. The reason I needed to drop missing data rows and duplicate rows was to make the analysis more clear and accurate once ran. 

- Looking at the data, the grade column had the "th" at the end of each grade. To make the analysis easier to run, I needed to remove the "th" at the end of each grade and change the value from a string to an integer. By changing grade from an object to an integer, when I ran the descriptive statistics on the dataset, we were also able to get those descriptives for grade as well. 

- Now that the data has been prepared, I was able to analyze the data. However, before I start to run comparative analysis I wanted to make sure I understood that data I was working with. Therefore, I decided to drill into the data itself a little further. For example, I wanted to look at the descriptive information for grade nine, so I used the describe function and set my grade equal to nine to get the input in Table 1. 

Table 1. 

![Descriptives of Grade 9](Descriptives_of_Grade_9.png)



