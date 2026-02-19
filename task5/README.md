# Titanic Dataset Analysis - Task 5

## Overview
This notebook performs a comprehensive exploratory data analysis (EDA) on the Titanic dataset (`train.csv`), focusing on data cleaning, missing value handling, and visualization of key patterns.

## Dataset
- **Source:** train.csv (Titanic passenger dataset)
- **Contents:** Passenger information including age, fare, class, gender, and survival status

## Key Findings

### 1. Data Exploration
- Loaded the Titanic dataset and examined the first few rows
- Identified data types and structure of the dataset
- Generated statistical summaries for numerical columns

### 2. Missing Values Analysis
Initial missing values identified:
- **Age:** Missing values present
- **Cabin:** Large number of missing values
- **Embarked:** Few missing values (typically 2 rows)

### 3. Data Cleaning & Preprocessing
The following data cleaning steps were performed:
- **Age Missing Values:** Filled with the median age to preserve the dataset
- **Cabin Column:** Dropped entirely due to excessive missing values (>70%)
- **Embarked Column:** Dropped rows with missing values (only 2 rows)
- **Result:** Clean dataset ready for analysis with no missing values

### 4. Visualizations & Insights

#### Age Distribution
- Generated histogram with KDE (Kernel Density Estimation)
- Shows the age distribution of passengers aboard the Titanic
- Most passengers were between 20-40 years old

#### Fare Analysis
- Created boxplot to detect outliers in passenger fares
- Identified premium fares (first-class tickets)
- Revealed fare outliers indicating luxury accommodations

#### Correlation Analysis
- Generated correlation heatmap for all numerical features
- Shows relationships between:
  - Passenger class (Pclass)
  - Age
  - Fare
  - Survival outcome
- Key observation: Higher fare correlates with increased survival rate

#### Survival Analysis by Class & Gender
- Bar plot showing survival rates across passenger classes and gender
- **Key Findings:**
  - Women had significantly higher survival rates across all classes
  - First-class passengers had better survival odds than lower classes
  - The "women and children first" evacuation protocol is evident in the data

## Technologies Used
- **Pandas:** Data manipulation and analysis
- **NumPy:** Numerical computations
- **Matplotlib:** Visualization
- **Seaborn:** Statistical data visualization

## Conclusion
The analysis reveals that passenger survival on the Titanic was strongly influenced by:
1. **Gender:** Women had priority in lifeboats
2. **Passenger Class:** Higher class passengers had better access to lifeboats
3. **Age:** Age demographics affected proximity to lifeboats and mobility
4. **Fare:** Affluent passengers (higher fares) were more likely to survive


