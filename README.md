# Students-Performance

## The data were downloaded from [Kaggle](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?rvi=1) and were updated there by Jakki Seshapanpu, under the name of "Students Performance in Exams". Below are detailed the variables that comprise this dataset.

<ul style='font-size: 18px; line-height: 2; text-align: justify;'>
    <li><b>Gender</b> - Students' genders</li>
    <li><b>Parental level of education</b> - How much students' parents studied</li>
    <li><b>Race/Ethnicity</b> - Ethnic groups of the students</li>
    <li><b>Lunch</b> - Kind of lunch that students usually get</li>
    <li><b>Test preparation course</b> - Level of preparation course</li>
    <li><b>Math score</b> - Score in Math </li>
    <li><b>Writing score</b> - Score in Writing</li>
    <li><b>Reading score</b> - Score in Reading</li>
</ul>

## I have added a few more subjects, described by ChatGPT 3.5 as more common in American high schools:

<ul style='font-size: 18px; line-height: 2; text-align: justify;'>
    <li><b>Science</b> - Score in Science</li>
    <li><b>Social Studies</b> - Score in Social Studies</li>
    <li><b>Foreign Language</b> - Score in Foreign Language</li>
    <li><b>Physical Education</b> - Score in Physical Education</li>
</ul>

##  Initially, I performed a normal test to check if the three subjects in the original dataset were distributed like a normal distribution, which was not the case. Therefore, since I was going to generate data for the new subjects, I chose to replace the data for these three subjects with new, normally distributed values. Together, these scores will compose an overall average for each student, and through it, we will be able to determine if they are approved or not ($\mu$ $\geq$ 60). From this, I checked the probability of selecting one who passed among all the students, which subject they got better and worst too.

## It was also necessary to change from 'none' to 'no one' in the 'Test preparation course' variable to avoid conflicts with Python itself (Version 3.11).

## In this project, I performed an ANOVA (oneway) and a ztest (two-sided) related to categorical variables to check if any of these influenced (justification) the students' performance. Each categorical variable divide the students into smaller groups.


## The descriptive statistics (measures of central tendency, dispersion, and shape) was carried out, calculating the average of each student, the average per subject, standard deviation, mode, median, percentiles, quartiles, distribution of grades, skewness, kurtosis and correlation. In some cases, horizontal bar graphs, boxplots, and line graphs were used, always applying data visualization techniques described in the book [Storytelling with Data](https://www.storytellingwithdata.com/). 

## I also used [DataSpell 2023.2.4](https://www.jetbrains.com/dataspell/) to work.