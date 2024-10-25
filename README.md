# Employee Attrition Analysis

An individual project focused on analyzing which factors impact employee attrition and identifying potential areas for HR intervention.

##  Project Overview 


I worked with the [IBM HR Analytics Atrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset/data), available on Kaggle. It contains data related to employee atrition within an organization, including various personal, professional and organizational attributes. 

The **main goal** is to analyze the reasons behind employee attrition and identify factors influencing turnover. 

*There is a lack information on the specific reasons for employee terminations and exits, so the recommendations provided may not apply to every situation. Conducting further research, such as exit interviews, could be beneficial in understanding the conditions and challenges the company faces in retaining talent.*

## 💻 Technologies used 

- Jupyter Notebooks
- Python (pandas, matplotlib, seaborn)
- Tableau
- GitHub

## 📁 Project structure 

- `data/`: Contains the dataset used for analysis 
- `notebooks/`: Jupyter Notebooks containing data cleaning, analysis, and visualizations
- `README.md`: Project documentation and instructions

## 📊 Project Summary 

This data set contains information on 1470 employees regarding:

- **Demographic information**: age, gender and marital status
- **Employment details**: job role, job level, department and field 
- **Performance and Satisfaction**: employee's satisfaction on work environment, job involvement, job satsifaction, performance rating, relationship satisfaction and work-life balance
- **Financial details**: daily and monthly rates, monthly income, percentage increase in salary over previous year and stock option level
- **Work experience**: total of years the employee has been with the company, duration in the curent job role, years since last promotion, duration with current manager, total years of work experience
- **Job Conditions**: overtime, travel requirement, distance from home, n° of training in the previous years

## 🔍 Exploratory Data Analysis

### Total Attrition Ratio

- Total employees: 1470
- Employees in the company: 1233
- Employees who left: 237
- Ratio: **16,12 %** of employees have left the company

![Screenshot 2024-10-25 at 18 54 37](https://github.com/user-attachments/assets/43003731-797e-4606-b8de-759ab6abec16)


### Demographics

#### Age

This is the distribution of the employees' age:

![Screenshot 2024-10-25 at 18 05 15](https://github.com/user-attachments/assets/142feda0-ee2f-4418-97e3-6c8f88d17af0)

- The average age is 36,9
- The age range is broad, 18 to 60
- Half of the employees are in between 30 and 43

It is a relatively symmetric distribution, suggesting a farily **balanced and diverse workforce**. 
  
After separating both populations (employees who stayed and employees who left) and comparing the same statistical data,

| Value | Stayed | Left |
| :-: | :-: | :-: |
| Average | 37,6  | 33,6  |
| Range | 18 to 60 | 18 to 58 |
| 50 % of employees | 31 to 43 | 28 to 39  |

we observe that the average, range and IQR is sligthly lower, indicating that **younger employees are more likely to leave.**

Taking a closer look at the attrition rate by age:

![Screenshot 2024-10-25 at 19 13 32](https://github.com/user-attachments/assets/a357f019-a893-49f4-84ce-48e48a7c6d06)

we observe that the **youngest employees have the highest attrition rates**, with age 19 having 66,67 % and followed by age 20 with 54,55 % attrition rate. 

This finding suggests:

- Limited job satisfaction or career growth opporunities
- Transitioning phases in life

**Recommendations:**

- Employee Engagement Programs
- Mentorship opportunities
- Career Development Pathways

The data implies that retention efforts may need to focus more on younger employees, who appear to have a higher likelihood of leaving. This insight could guide strategies like targeted development programs, mentoring, or career pathing initiatives aimed at younger employees to encourage retention.

#### Gender







