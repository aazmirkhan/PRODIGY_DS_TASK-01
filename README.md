PRODIGY_DS_01 – Age and Gender Distribution Visualization

✅ Task 01 – Data Science Internship @ Prodigy InfoTech

Completed Task-01 of my DS internship at Prodigy InfoTech!  
In this task, I worked with the Titanic dataset to analyze and visualize two key features — age and gender. The objective was to apply basic data analysis and visualization techniques using Google Colab to understand how these variables are distributed.

📌 Objective
To explore and visualize demographic variables using appropriate plots in Python. The goal was to represent gender (categorical) and age (continuous) data using a bar plot and histogram, respectively.

📂 Dataset
[Titanic Dataset](https://raw.githubusercontent.com/pandas-dev/pandas/master/doc/data/titanic.csv)  
This dataset includes information about passengers on the Titanic, including age, sex, class, and survival status.

🛠️ Tools & Libraries
- Google Colab
- Python
- Pandas
- Seaborn
- Matplotlib

📊 Visualizations

1. **Bar Plot – Gender Distribution**  
   Visualizes the number of male and female passengers.

2. **Histogram – Age Distribution**  
   Shows the age spread of passengers with a KDE line for distribution curve.

💻 Code Snippet

```python
# Importing libraries
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load dataset
df = pd.read_csv("https://raw.githubusercontent.com/pandas-dev/pandas/master/doc/data/titanic.csv")

# Gender Distribution
sns.countplot(data=df, x='Sex')
plt.title("Gender Distribution")
plt.show()

# Age Distribution
sns.histplot(data=df, x='Age', bins=15, kde=True)
plt.title("Age Distribution")
plt.show()
