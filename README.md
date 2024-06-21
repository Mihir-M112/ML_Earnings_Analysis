# ML Earnings Analysis

Welcome to the ML Earnings Analysis project. This initiative aims to provide a comprehensive analysis of the salaries of Machine Learning professionals, leveraging a diverse dataset to uncover key trends and insights. As the field of Machine Learning continues to expand rapidly, understanding compensation trends is crucial for both employers and employees to make informed decisions.

## Approach And Techniques

The goal of this project is to forecast the salaries of AI/ML positions. Below are the data preprocessing techniques employed in this project:

-> Data Preprocessing Techniques
Visualization


Tool: Plotly  
Purpose: To create interactive and informative visual representations of the dataset, aiding in understanding data distributions and relationships between variables.

-> Feature Engineering    
Log Transformation: Applied to address skewness in the data, making the distribution more normal.  
Box-Cox Transformation: Another technique to correct skewness, applied to continuous variables to stabilize variance and make the data more normally distributed.  
Label Encoding: Used for nominal categorical variables, converting them into numerical values.  
One-Hot Encoding: Applied to ordinal categorical variables, creating binary columns for each category to facilitate model training.  
  
-> Feature Selection  
ANOVA (Analysis of Variance): Utilized to identify significant features by comparing means among different groups and determining which features contribute most to the variance in the target variable.  
Post-Lasso: A regularization technique applied to select the most relevant features by shrinking less important feature coefficients to zero, ensuring only the most impactful features are used in the model.  

-> Modeling Techniques  
Deep Learning Framework: TensorFlow with Keras  
Dropout: Implemented to prevent overfitting by randomly dropping units during training.  
Early Stopping: Used to stop training when the model's performance on a validation set stops improving, preventing overfitting and reducing training time.  
By employing these advanced data preprocessing techniques and modeling strategies, this project aims to build robust models capable of accurately forecasting the salaries of AI/ML positions.  

## Dataset Description

The dataset used in this project comprises salary information for Machine Learning professionals and includes the following columns:

work_year: The year of the recorded salary.  
experience_level: The level of experience in the field (e.g., Entry-level, Mid-level, Senior-level).  
employment_type: The type of employment (e.g., Full-time, Contract).  
job_title: The job title of the employee (e.g., Data Scientist, Data Science Manager).  
salary: The salary amount in the local currency.  
salary_currency: The currency of the salary.  
salary_in_usd: The salary converted to USD for standardization.  
employee_residence: The country of residence of the employee.  
remote_ratio: The ratio of remote work (e.g., 0 for on-site, 50 for hybrid, 100 for fully remote).  
company_location: The country where the employing company is located.  
company_size: The size of the company (e.g., Small, Medium, Large).  
  
The dataset contains 16,494 entries, ensuring a robust sample size for analysis. It covers a range of job titles, experience levels, and employment types across different regions and company sizes, providing a rich foundation for deriving meaningful insights into the compensation landscape of Machine Learning professionals in 2024.

#### REFERENCES:
[1] https://ai-jobs.net/salaries/  
[2] https://www.kaggle.com/datasets/chopper53/machine-learning-engineer-salary-in-2024/data

## Virtual Environment

A virtual environment (`venv`) is used to manage the project's dependencies. To set up the virtual environment, run the following commands:

```sh
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
