# Sleep Deprivation and Cognitive Performance Analysis

## Overview
This project explores the impact of sleep deprivation on cognitive performance and emotional regulation using a dataset that includes sleep metrics, cognitive task results, and demographic information. The analysis is conducted using Python and libraries like `pandas`, `numpy`, `matplotlib`, and `seaborn`. The project involves **data exploration**, **statistical analysis**, and **visualizations** to uncover patterns and trends, providing actionable insights into the effects of sleep deprivation on mental and emotional well-being.

---

## Dataset Description
The dataset contains the following key columns:
- **Sleep Metrics**: `Sleep_Hours`, `Sleep_Quality_Score`, `Daytime_Sleepiness`
- **Cognitive Performance**: `Stroop_Reaction_Time`, `N_Back_Accuracy`, `PVT_Time`
- **Emotional Regulation**: `Emotion_Regulation_Score`
- **Demographics**: `Age`, `Gender`, `BMI`
- **Lifestyle Factors**: `Caffeine_Intake`, `Physical_Activity_Level`, `Stress_Level`

---

## Key Steps in the Analysis

### 1. **Data Loading and Exploration**
- Loaded the dataset from an SQLite database (`sleep_study.db`) into a pandas DataFrame.
- Explored the dataset using methods like `.head()`, `.info()`, and `.describe()`.
- Checked for missing values and unique values in categorical columns.

### 2. **Data Transformation**
- Normalized numerical columns (e.g., `Sleep_Hours`) to a 0-1 scale.
- Created new features like `Sleep_Efficiency` (Sleep Quality Score / Sleep Hours).
- Encoded categorical variables (e.g., `Gender`) for analysis.

### 3. **Statistical Analysis**
- Calculated descriptive statistics for numerical columns.
- Analyzed correlations between variables using a correlation matrix.
- Grouped data by gender and stress level to calculate averages for key metrics.

### 4. **Visualizations**
- **Distributions**: Histograms for `Sleep_Hours`, `Sleep_Quality_Score`, `PVT_Time`, `N_Back_Accuracy`, and `Emotion_Regulation_Score`.
- **Correlation Heatmap**: Visualized relationships between numerical variables.
- **Scatter Plots**: Explored relationships between sleep metrics and cognitive/emotional performance.
- **Boxplots**: Compared key metrics by gender.

---

## Tools and Libraries
- **Python**: Primary programming language.
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical operations.
- **Matplotlib/Seaborn**: Data visualization.
- **SQLite3**: Database interaction.

---

## File Structure
```
project/
├── data/
│   └── transformed_sleep_data.csv       # Transformed dataset
├── database/
│   └── sleep_study.db                   # SQLite database
├── scripts/
│   └── sleep_cognition_analysis.ipynb   # Analysis script
└── README.md                            # Project documentation
```

---

## How to Run the Analysis
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd project
   ```
2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn sqlite3
   ```
3. Run the analysis script:
   ```bash
   python scripts/sleep_cognition_analysis.ipynb
   ```
4. Check the output:
   - Transformed data: `data/transformed_sleep_data.csv`
   - Visualizations: Displayed in the script output.

---

## Key Insights
- **Sleep Hours**: Normalized to a 0-1 scale for consistent analysis.
- **Sleep Efficiency**: A new feature created to measure sleep quality relative to sleep duration.
- **Gender Differences**: Males tend to have slightly higher sleep hours and quality scores compared to females.
- **Stress Levels**: Higher stress levels are associated with lower sleep hours and quality.
- **Cognitive Performance**: Sleep deprivation negatively impacts reaction times and memory accuracy.

---

## Future Enhancements
- Add machine learning models to predict cognitive performance based on sleep metrics.
- Integrate with cloud storage (e.g., AWS S3) for scalability.
- Automate the analysis pipeline using workflow management tools like Apache Airflow.

---

## Author
Md Islam
GitHub: https://github.com/mdislam1

---
