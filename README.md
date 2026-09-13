# Titanic Exploratory Data Analysis 🚢

## About the Project
This project explores the Titanic dataset using Python to understand passenger survival patterns. It includes data cleaning, feature creation, statistical analysis, and visualization.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset
The dataset contains **891 passengers and 15 columns** and is loaded using Seaborn:

    df = sns.load_dataset("titanic")

Key features include age, gender, passenger class, fare, family members, embarkation port, and survival status.

## Data Cleaning
- Filled 177 missing age values with the mean age.
- Removed the `deck` column because it contained many missing values.
- Filled missing `embarked` values with the most frequent value.
- Two missing values remain in `embark_town`, which is not used in the analysis.

## Feature Engineering
- **Family Size:** Calculated as `sibsp + parch`. This counts accompanying family members and excludes the passenger.
- **Age Group:** Divided passengers into Child, Teenager, Young Adult, Adult, and Senior categories.

## Analysis and Visualizations
- Survival rate by gender
- Survival rate by passenger class
- Survival rate by age group
- Survival rate by embarkation port
- Survival rate by family size
- Age distribution histogram
- Correlation heatmap

## Key Findings

| Passenger Group | Survival Rate |
| --- | ---: |
| Female | 74.20% |
| Male | 18.89% |
| First Class | 62.96% |
| Second Class | 47.28% |
| Third Class | 24.24% |
| Children | 57.97% |
| Seniors | 22.73% |

- Female passengers had a higher survival rate than male passengers.
- First-class passengers had the highest survival rate among ticket classes.
- Children had the highest survival rate among the defined age groups.
- Survival rates varied across embarkation ports and family sizes.

These findings describe associations in the dataset and do not establish causation. Age-based results are affected by filling missing ages with the mean.

## Skills Demonstrated
Data cleaning, exploratory data analysis, feature engineering, Pandas groupby operations, data visualization, and interpretation of findings.

## Author Name
Akash Sonar
## Conclusion
This project demonstrates how Python can be used to clean, explore, and visualize data to identify passenger survival patterns. It focuses on exploratory analysis and does not include a prediction model.
