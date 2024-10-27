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
- Miro board
- GitHub

## 📁 Project structure 

- `data/`: Contains the dataset used for analysis 
- `notebooks/`: Jupyter Notebooks containing data cleaning, analysis, and visualizations
- `README.md`: Project documentation and instructions

## 📊 Project Summary 

This data set contains information on 1470 employees on:

- **Demographic information**: age, gender and marital status
- **Employment details**: deparment, job role
- **Performance and Satisfaction**: employee's satisfaction on work environment, job involvement, job satsifaction, performance rating, relationship satisfaction and work-life balance
- **Financial details**: daily and monthly rates, monthly income, percentage increase in salary over previous year and stock option level
- **Work experience**: total of years the employee has been with the company, duration in the curent job role, years since last promotion, duration with current manager, total years of work experience
- **Job Conditions**: overtime, travel requirement, distance from home, n° of training in the previous years

You can look at the detailed analysis in the section below

## 🔍 Exploratory Data Analysis

### Total Attrition Ratio

- Total employees: 1470
- Employees in the company: 1233
- Employees who left: 237
- Ratio: **16,12 %** of employees have left the company

![Screenshot 2024-10-25 at 18 54 37](https://github.com/user-attachments/assets/43003731-797e-4606-b8de-759ab6abec16)


### Demographics
<details><summary>Age</summary>

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

</details>
<details><summary>Gender</summary>

This is the distribution of employees by gender:

![Screenshot 2024-10-26 at 13 58 25](https://github.com/user-attachments/assets/1a9750bf-3882-4732-8c5f-0476e83e5404)

Since there are more males employees overall, there will naturally be more male employees among those employees who left. However, let's take a look at the separate **attrition rates**:

- Male: 17 %
- Female: 14.8 %

While the difference between male and female employees is not very large, it does indicate a **higher likelihood for male employees to leave the company**.

</details>

### Employment details

<details>
<summary>Department</summary>

This is the distribution of employees by department:

![Screenshot 2024-10-26 at 13 58 04](https://github.com/user-attachments/assets/e901c640-14b3-4726-9d23-a4236864b377)

Research and Development is the department with the highest number of employees, followed by Sales and Human Resources. As expected, R&D also has the highest number of employees who have left. However, let's take a closer look at the attrition rates:

- Sales: 20.6 %
- Human Resources: 19 %
- Research & Development: 13.8 %

We observe that **employees in Sales and Human Resources are more likely to leave**, with attrition rates of 20.6% and 19% respectively, exceeding the acceptable range of 10-15%. 

Although R&D has a notable lower rate of 13,8 % , it is also worthy to look at, since it is at the higher end of the expected range. 

**Recommendations:**

- Review compensation and commission structures
- Review onboarding processes to improve early employee retention
- Implement regular employee engagement surveys
- Develop targeted retentinon strategies for each department based on heir challenges and employee feedback
  
</details>

<details>
<summary>Job Role</summary>

Now that we already have the information by department, let's take a closer look at the existing roles. 

![image](https://github.com/user-attachments/assets/4a775e40-9115-440d-a002-f1cbb2be8dc0)

Let's take a closer look at the attrition rates per role, we find that:

![Screenshot 2024-10-26 at 15 51 34](https://github.com/user-attachments/assets/84cc60dc-f4cb-449d-a944-79b91482b0bb)

- **Sales Representatives** have a worrying high attrition rate
- Despite R&D being the department with lower attriiton rates, **Laboratory Technician** is the role with the second highest attrition rate with almost 24 %
- As expected, **Human Resources** job roles also have high attrition rates, although it only affects to the associates, not to the Managers
- Sales Executives and Research Scientists follow the ranking, with moderately high rates

**Findings and recommendations:**

**- Sales department:**

Although the department analysis alrady gave us a hint, we can confirm now that **Sales is the most critical department**, with two of its three roles being the ones with the highest attrition rates. In this situation, it is crucial to:

+ evaluate the workload and sales targets
+ develop mentorship programs and development oportunities
+ review assignments and distribute accounts

**- Human Resources:**

Being the second departtment with higher turnover by a very narrow margin, the situation for **Human Resources is also concerning**. Taking into account that most of the department consist of Human Resources Associates and Managers count with a low turonver rate, we recommend:

+ provide opportunities for professional development and certifications
+ consider horizontal promotions
+ evaluate workload and stress levels
+ improve career development paths and opportunities

**- R&D:**

Although the turnover rate is lower than in other departments, the analysis of job roles provided insights into what the company needs to address in R&D, as two of its positions are among the top five with the highest likelihood of turnover.

+ review work conditions and safety protocols
+ opportunities for continued education and attendance at industry conferences
+ ensure cutting-edge technoloy and resources

</details>

### Performance and satisfaction

<details><summary>Satisfaction on work environment</summary>


</details>

