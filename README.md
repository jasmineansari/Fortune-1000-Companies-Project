# Fortune-1000-Companies-Project
Pioneered an exacting data refinement and outlier mitigation initiative. Engineered a linear regression model, selectively incorporating  highly correlated numerical columns. Attained a logistic regression model with an exemplary accuracy quotient of 0.99.

The provided file, "Fortune_1000_companies.ipynb," contains a detailed analysis of a dataset comprising information on Fortune 1000 companies. The analysis involves preparing, cleaning, and preprocessing the raw data to address issues like missing values and outliers. Additionally, new features are engineered to enhance the dataset for predictive modeling purposes. The goal is to build both linear regression and logistic regression models to understand the factors influencing a company's revenue and profitability, respectively. The analysis also delves into exploring relationships between key variables such as profitability, CEO-founder dynamics, and their impact on rankings within the Fortune 500 list.

### Dataset Description
The dataset includes various attributes such as company rankings, financial metrics, executive leadership details, and industry-specific data. Some key attributes in the dataset are:
- Rank
- Company
- Ticker
- Sector
- Industry
- Profitable
- Founder_is_CEO
- Female CEO
- Growth_in_Jobs
- Change_in_Rank
- Gained_in_Rank
- Dropped_in_Rank
- Newcomer_to_the_Fortune 500
- Global500
- Best Companies
- Number_of_employees
- MarketCap_March31_M
- Revenues_M
- RevenuePercentChange
- Profits_M
- ProfitsPercentChange
- Assets_M
- CEO
- Country
- HeadquartersCity
- HeadquartersState
- Website
- Company Type
- Footnote
- MarketCap_Updated_M
- Updated

### Working Performed

1. **Data Loading and Cleaning**:
   - The code starts by loading the dataset and checking for missing values in each column using `df.isnull().sum()`[1].
   - It then identifies the data type of the column "Newcomer_to_the_Fortune500" using `df['Newcomer_to_the_Fortune500'].dtype`[1].
   - Missing values in the dataset are handled by filling them with the mode for object type columns and the median for numerical columns using a loop that iterates through each column[1].

2. **Exploratory Data Analysis**:
   - The code further explores the dataset by checking the mode value for the column "Gained_in_Rank" using `df['Gained_in_Rank'].mode()`[1].
   - It also examines the distribution of missing values across all columns using `df.isnull().sum()`[1].
   - The code provides information about the data types and non-null counts for each column in the dataset using `df.info()`[1].
   - Additionally, it checks for duplicated rows in the dataset using `df.duplicated().sum()`[1].

3. **Visualization**:
   - The code includes visualizations that are not directly visible in the provided text snippet, such as plots or graphs that may help in understanding the data distribution and relationships.

4. **Model Building**:
   - Although not explicitly mentioned in the provided text snippet, the code likely involves building linear regression and logistic regression models to analyze factors influencing revenue and profitability, respectively, based on the dataset's attributes.
  
### Algorithms Applied
1. Linear Regression: Used to analyze the relationship between independent variables and a continuous dependent variable (e.g., revenue).
2. Logistic Regression: Employed to model the probability of a binary outcome (e.g., profitability) based on one or more independent variables.

Overall, the code in the file "Fortune_1000_companies.ipynb" focuses on data preparation, cleaning, exploratory data analysis, and potentially model building to gain insights into the performance and characteristics of Fortune 1000 companies.
