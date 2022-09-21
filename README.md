# School_District_Analysis
Aggregate the data and showcase trends in school performance.

## Overview of Project
### Purpose
The purpose of this project was to assist Maria, the cheif data scienct for a city school district, analyze information from a variety of sources in a variety of formats. I will be assisting her analyze data on student funding and standardized test scores, as well as aggregate the data and showcase trends in school performance. 

## Analysis

- For this project, I needed to utilize the three-phase process to prepare and organize my tasks and responsibilities. The three-phase process is: 

    1. Collect the data
    
    2. Prepare the data
    
    3. Analyze the data
    
- To begin my analysis, I needed to import the appropriate dependencies so that I could properly import the data. Now, I can collect the data, by creating a path to the dataset by using the os.path.join() function to tell Jupyter Notebook that I want to open the full student dataset, but since I don't know the direct path, use this function to find the dataset: full_student_data = os.path.join('../Resources/new_full_student_data.csv'). After generating the path, I can read the file byt using Pandas read.csv function. 

- Once the data was collected, I needed to prepare the data so that when I begin to run analyses, I don't run into any errors. Therefore, I needed to check for any missing data in the dataset. If there were any rows that had missing data, I needed to drop them from the dataset and then verify that they were dropped. I also needed to check to see if there were any duplicate rows. If there were duplicate rows I needed to drop those as well, and then verify that they were dropped. The reason I needed to drop missing data rows and duplicate rows was to make the analysis more clear and accurate once ran. 

- Looking at the data, the grade column had the "th" at the end of each grade. To make the analysis easier to run, I needed to remove the "th" at the end of each grade and change the value from a string to an integer. By changing grade from an object to an integer, when I ran the descriptive statistics on the dataset, we were also able to get those descriptives for grade as well. 

- Now that the data has been prepared, I was able to analyze the data. However, before I start to run comparative analysis I wanted to make sure I understood that data I was working with. Therefore, I decided to drill into the data itself a little further. For example, I wanted to look at the descriptive information for grade nine, so I used the describe function and set my grade equal to nine to get the input in Table 1. 

Table 1. 

![Descriptives of Grade 9](https://github.com/mrma2318/School_District_Analysis/blob/5bfc805847bb74b994748dc2456dac8f9ae4cc65/Student_Data_Challenge_Starter_Code/Resources/Descriptives_of_Grade_9.png)


- After exploring the dataset a little deeper, I could finally compute my analyses. I wanted to compare between district verus charter schools for budget, size and scores. To analyze the budget for each school type based on grade, I needed to group by school based on grade and set it to calculate the mean for each. See Table 2. 

Table 2. 

![Average Budget Per Grade for Each School](https://github.com/mrma2318/School_District_Analysis/blob/5ae52944bbe4759fe180783a0400213242462f0c/Student_Data_Challenge_Starter_Code/Resources/Avg_Budget_Per%20Grade_Type.png)

- Based on Table 2, you can see that on average, the Public school had a higher budget compared to the Charter school for each grade. Then I wanted to see how many students there were in each school. To do this, I needed to group by the school name and sort based on the student id. I also wanted to sort the schools in decending order so that the school with the highest number of students showed at the top of the table. See Table 3. 

Table 3. 

![Number of Students Per School](https://github.com/mrma2318/School_District_Analysis/blob/27eac103b99589a34f0c39a4d1f9062cc4dd62ae/Student_Data_Challenge_Starter_Code/Resources/Number_Students.png)

- Lastly, I wanted to compare the math scores and reading scores for each school. To complete this analysis I needed to group by school type and set it to find the average. Then I could set the code to find the average for math and reading scores. See Table 4. 

Table 4. 

![Average Math and Reading Scores Per School Type](https://github.com/mrma2318/School_District_Analysis/blob/48b020bb30af878929e7d26b583b376e7d782f49/Student_Data_Challenge_Starter_Code/Resources/Avg_Math_Reading.png)

- From Table 4, you can see that students performed slightly better on math in the Charter schools compared to the Public schools. However, regardless of the type of school students went to, their average reading scores were about the same. 

## Results

- There are two conclusions we can draw from these outcomes. The first one is that Public schools have a higher budget compared to Charter schools. The second one is that Charter schools perform slightly better in math compared to Public Schools, but regardless of the type of school students go to, they perform equally in reading. 

- There are some additional anlaysis that could be completed on this dataset. For example, looking at the total number of students in public versus charter schools. Since we know that Public schools have a higher budget, looking at potential factors that explain the why would be beneficial. If Public schools have a higher number of students than Charter schools, then that would probably explain why Public schools have a higher budget, trying to accommodate for the additional number of students. 

- Another analysis we could look at is which schools were Public schools, and which ones were Charter schools. If there is a greater number of Public schools, it could explain the difference in budget as well. Having a higher budget could be due to having to support a greater number of public schools compared to charter schools. Understanding the number of Public schools compared to Charter schools, might also explain why Public schools have a higher number of students in total as well. Having additional Public schools means having a higher student rate. 