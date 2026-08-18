Employee Performance Analysis
Understanding the workforce factors associated with employee performance

📌 Project Overview

Employee performance is one of the areas HR teams constantly monitor, but knowing who is performing well and who isn't is only part of the problem.

A more useful question is:

What patterns are associated with employees who are struggling, and where should HR look first?

This project explores employee performance alongside factors such as engagement, absence, training, manager support, age, gender and department.

The goal was not simply to create another HR dashboard, but to build an analysis that could help HR move from identifying a performance problem to identifying where attention may be needed.

🎯 Business Problem

An organization may know that some employees are underperforming, but a performance score by itself doesn't provide much direction.

HR needs to understand:

How is the workforce performing overall?
How many employees need improvement?
Where are performance concerns concentrated?
Are there workforce factors associated with weaker performance?
Do performance patterns differ across employee groups?
Which employees may require further attention?

Without this context, HR reporting can become purely descriptive.

The objective of this project was therefore to use employee data to identify meaningful patterns around performance and turn those findings into a practical dashboard for HR decision-making.

🧠 Analytical Approach

I approached the project in stages rather than building the dashboard immediately.

1. Data preparation

The dataset was reviewed and prepared for analysis using Power Query.

This included:

Checking data types
Reviewing numerical ranges
Creating meaningful categorical groupings
Preparing demographic fields
Creating performance-related categories
Checking the consistency of the dataset

The dataset includes European employee/workforce data and contains employee-level information across performance, engagement, attendance, training and workforce characteristics.

📊 Dataset

The analysis uses an employee-level synthetic dataset designed around a European workforce context.

Key variables
Category	Variables
Employee information	Employee ID, Age, Gender
Workforce	Department, Country, Job Level
Performance	Performance Score, Performance Level
Engagement	Engagement Score, Engagement Level
Attendance	Absence, Absence Level
Development	Training Hours, Training Level
Management	Manager Support Score, Manager Support Level
Work patterns	Overtime Hours, Overtime Level

The dataset was intentionally structured to support HR analytics questions rather than simply demonstrate visualization techniques.

🔎 Exploratory Analysis

Before building the final dashboard, I used an exploration phase to understand the relationships within the dataset.

The goal was to answer:

What is actually worth putting on the final dashboard?

Rather than assuming every variable was important, I compared performance across different workforce factors.

Performance

The first step was establishing the overall performance picture.

Key metrics

Average Performance: 75.99

Needs Improvement: 24.42%

High Performers: 14.25%

This showed that while the majority of employees were meeting expectations, a meaningful proportion of the workforce required attention.

That led to the next question:

What characteristics are associated with employees who need improvement?

🔎 Engagement Analysis

Engagement produced the strongest pattern in the exploration.

Employees were grouped into:

Low Engagement
Moderate Engagement
High Engagement

The analysis showed a significant difference in performance concerns across these groups.

Needs Improvement rate
Engagement Level	Needs Improvement
Low	67.96%
Moderate	27.58%
High	7.18%

This became one of the central findings of the project.

Employees with low engagement were substantially more represented in the Needs Improvement group than employees with moderate or high engagement.

This does not prove that low engagement causes poor performance.

Instead, it indicates a strong association worth investigating further.

👥 Manager Support

Manager support was also explored to understand whether performance differed across different levels of perceived support.

The analysis showed:

Manager Support	Average Performance
Low	70
Moderate	74
High	80

The pattern suggests that employees reporting higher levels of manager support also tended to have higher average performance.

This makes manager support a potentially useful area for HR and people managers to investigate.

🎓 Training

Training exposure was examined to see whether employee development was associated with performance.

Training Level	Average Performance
Low	73
Moderate	76
High	81

Employees in the higher training group had higher average performance.

Again, this is an association, not proof that additional training directly causes higher performance.

However, it provides a useful signal for HR when thinking about learning and development.

📅 Absence

Absence was also examined.

Absence Level	Average Performance
Low	79
Moderate	76
High	72

The pattern showed that higher absence levels were associated with lower average performance.

This creates another potential area for HR investigation, particularly where repeated absence and performance concerns occur together.

👤 Demographic Analysis

Demographic variables were explored to determine whether performance differences existed across employee groups.

The analysis included:

Age group
Gender
Department

Age groups were structured as:

<25
25–34
35–44
45–55
>55

Gender and department were also examined for differences in average performance.

These variables were treated primarily as contextual filters and comparison dimensions, rather than being positioned as primary explanations for performance.

This was intentional.

Not every difference in a dataset deserves to become a headline finding.

📈 Dashboard Design

After exploration, the dashboard was designed around the questions an HR professional would most likely need answered.

The final dashboard uses a minimalist layout rather than displaying every analysis performed during exploration.

Dashboard sections
1. Performance KPIs

Three headline KPIs provide an immediate workforce overview:

Average Performance — 75.99
Needs Improvement — 24.42%
High Performers — 14.25%
2. Performance Distribution

A donut chart shows the distribution of employees across performance categories:

Meets Expectations
Needs Improvement
Exceeds Expectations
Unsatisfactory

This gives HR an immediate understanding of the overall performance composition.

3. Performance by Department

Department-level performance is included to provide workforce context and allow HR to identify areas where performance patterns may differ.

The differences are relatively modest, so department is treated as a contextual dimension rather than the primary driver of the analysis.

4. Performance by Age Group

Age groups are used to examine whether performance patterns vary across different stages of the workforce.

The age grouping was deliberately standardized into:

<25 | 25–34 | 35–44 | 45–55 | >55

A custom sort column was created in Power Query to ensure the groups appeared in logical age order rather than alphabetical order.

5. Performance by Gender

Gender was included as another demographic comparison.

The purpose is not to suggest that gender determines performance, but to allow HR to check whether performance patterns differ across workforce groups.

👀 Employees Requiring Attention

One of the most important design decisions was adding an employee-level table.

Instead of stopping at:

“24.42% of employees need improvement.”

the dashboard allows HR to move closer to the employees behind the number.

Employees Requiring Attention

The table includes fields such as:

Employee ID
Department
Age
Gender
Engagement Level
Performance Level
Manager Support
Absence

This makes the dashboard more actionable.

An HR professional can identify employees showing combinations of concerning indicators and decide whether further investigation or intervention is appropriate.

The dashboard therefore moves from:

Workforce overview → pattern identification → employee-level attention

💡 Key Findings
1. A meaningful proportion of employees need improvement

24.42% of employees were classified as needing improvement.

This represents a sizeable enough group to warrant further investigation.

2. Engagement showed the strongest relationship with performance concerns

The most notable finding was among low-engagement employees.

67.96% of employees in the low-engagement group were classified as needing improvement.

Compared with:

27.58% among moderate engagement
7.18% among high engagement

This makes engagement an important area for HR to investigate.

3. Manager support showed a clear performance pattern

Average performance increased across manager-support levels:

70 → 74 → 80

This suggests that employees experiencing stronger manager support also tended to report stronger performance.

4. Training showed a positive pattern

Average performance increased from:

73 → 76 → 81

across low, moderate and high training groups.

This provides a potential signal for HR's learning and development strategy.

5. Higher absence was associated with lower performance

Average performance declined from:

79 → 76 → 72

as absence increased.

This highlights the importance of looking at attendance alongside performance rather than treating the two as completely separate HR metrics.

🎯 Recommendations

Based on the analysis, I would recommend that HR consider:

1. Investigating low-engagement employees

The large difference in performance concerns across engagement levels makes this the strongest starting point.

HR could investigate:

Employee feedback
Manager relationships
Workload
Recognition
Career development
Role satisfaction

The aim would be to understand why engagement is low rather than assuming the reason.

2. Strengthening manager support

Because higher manager-support levels were associated with stronger performance, organizations could consider:

Manager coaching
Regular one-to-one conversations
Feedback practices
Clearer performance expectations
Manager effectiveness assessments
3. Review development opportunities

The relationship between training and performance suggests that HR should examine whether employees with weaker performance have adequate access to relevant training and development.

4. Monitor absence alongside performance

Employees with both high absence and performance concerns may warrant closer review.

The goal should not be to assume that absence causes poor performance, but to understand whether there are underlying workforce or employee-support issues.

5. Move from reporting to targeted intervention

Instead of treating every employee as requiring the same intervention, HR can use the dashboard to identify groups and individuals that may need further investigation.

⚠️ Important Analytical Note

This analysis identifies associations, not causation.

For example, the analysis shows that low engagement is strongly associated with performance concerns.

It does not prove:

“Low engagement causes poor performance.”

There may be other factors influencing both variables.

The dashboard should therefore be used as a decision-support and investigation tool, rather than as an automated system for judging employees.

🛠️ Tools Used

Power BI
Dashboard development, data visualization and interactive reporting.

Power Query
Data preparation, transformation and creation of analytical groupings.

DAX
KPI calculations, performance metrics and percentage measures.

Excel
Initial data handling and dataset preparation.

📌 Project Outcome

The final dashboard transforms employee-level HR data into a simple decision-making view.

Instead of only answering:

“How are our employees performing?”

it helps HR move toward:

“Where are the performance concerns, what patterns are associated with them, and which employees may require attention?”

The biggest lesson from the project was that good HR analytics isn't about putting every available metric on a dashboard.

It's about finding the signals that matter, knowing which ones don't, and presenting the information in a way that helps someone make a better decision.

🚀 Future Improvements

If additional organizational data were available, the analysis could be extended to include:

Employee survey comments and sentiment
Historical performance reviews
Promotion history
Compensation changes
Manager changes
Employee turnover
Exit interview data
Team-level workload
Longitudinal engagement data

This would allow HR to move from cross-sectional analysis toward predictive and longitudinal people analytics.


📊 Final Dashboard
<img width="1522" height="801" alt="Screenshot 2026-08-17 101202" src="https://github.com/user-attachments/assets/3d6c474f-baf8-4e3b-96e2-5ff7c13d7b88" />


Employee Performance Analysis

Understanding the workforce factors associated with employee performance.

Tools: Power BI | DAX | Power Query | Excel

Key finding:

67.96% of employees with low engagement were in the Needs Improvement group.

Business focus:

Identify performance concerns, understand the workforce patterns around them, and help HR know where to look next.
