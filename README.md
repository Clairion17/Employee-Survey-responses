# Employee-Survey-responses

This project analyzes **14,725 employee engagement survey responses** from **Pierce County, WA**. The dataset contains **10 fields** and includes department, role, and multiple survey questions.

 🎯 Project Objectives

 **1. Identify the questions employees agreed/disagreed with the most**

* Calculate average scores for each survey question
* Determine % agreement and % disagreement

 **2. Find patterns by department or job role**

* Compare satisfaction scores across departments
* Identify roles with the highest or lowest sentiment

 **3. Recommend actions for improving employee satisfaction**

* Use insights from the analysis to suggest practical improvements

---

📊 Tools Used

* **Power BI** – data cleaning, modeling, DAX calculations, dashboards, insights
* **Excel** – data cleaning, pivot tables, descriptive analysis
* **Python** (optional) – for extended EDA and plots (if needed)

---

 🛠️ Sample Analysis Code

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
df = pd.read_csv('employee_survey_responses.csv')

Identify question columns
question_cols = [col for col in df.columns if col.startswith('q')]

Calculate agreement statistics
summary = df[question_cols].mean().sort_values(ascending=False)
print(summary)

 Visualize
summary.plot(kind='bar')
plt.title('Average Score per Question')
plt.show()
```

---

 🔍 Key Insights (Example)

* Employees **agree most** with statements related to teamwork and collaboration.
* Employees **disagree most** with statements related to career growth and promotion transparency.
* Certain departments show **lower morale** due to workload issues.
* Frontline roles report **higher stress levels**.

---

💡 Recommendations

* Improve transparency in career progression.
* Provide more training and development opportunities.
* Review workload distribution in high-pressure departments.
* Strengthen leadership communication.

---

📁 Repository Structure

```
├── README.md
├── data/
├── notebooks/
├── scripts/
└── reports/
```

---

If you want, I can also create the folder structure, notebook, or full analysis script for GitHub.
