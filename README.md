# student-exam-score-analysis

Data Loading and Initial Inspection:
The script begins by importing necessary libraries (pandas, numpy, matplotlib, seaborn).
The data from student_score.csv is loaded into a DataFrame df.
Initial data exploration is conducted using df.head() to display the first few rows, and df.info() to show the data types and null values in each column. df.shape is used to get the dimensions of the DataFrame.

Descriptive Statistics and Null Value Analysis:
df.describe() is used to get descriptive statistics for numeric columns.
df.isnull().sum() checks for and counts null values in each column.

Gender Distribution Visualization:
A bar chart visualizes gender distribution using Seaborn's countplot. The plot is annotated with labels showing counts for each gender.
It is mentioned that there are more females than males in the dataset.

Analysis of Parental Impact on Scores:
Group by operations are performed on the ParentEduc (parent education level) and ParentMaritalStatus columns to aggregate average scores in math, reading, and writing.
Heatmaps are created to visualize the relationship between these factors and students' scores. It is concluded that parent education significantly impacts students' scores, while marital status does not.

Score Distribution Analysis:
Boxplots are created for Math, Reading, and Writing scores to visualize the distribution and identify potential outliers.

Ethnic Group Distribution:
Unique values in the EthnicGroup column are printed.
Counts for each ethnic group are calculated and displayed in both a pie chart and a count plot, showing the percentage distribution of ethnic groups.

Weekly Study Hours Analysis:
Unique values in the WklyStudyHours column are printed.
The data is grouped by the weekly study hours, and counts are displayed in a pie chart and a count plot, illustrating the distribution of students' weekly study hours.
