# HR_Analytics

## Type of Project: Logistic regression

### 1.	Introduction
  Our application is a well analyzed model for a company to help them determine how to retain talent. It has been observed that a company loses way more money by hiring new people and training them for a period of time than giving their well-deserved employee incentives. Our motivation lies on determining what the company is not doing or needs to do for their employees, so that they can retain their employees. Our model will be created considering the most impactful parameters that can help determine factors that impact employees’ decision to stay or leave.

### 2.	Data Sets
The dataset belongs to Human Resource which is also the domain.
Number of rows: 14999
Number of columns: 10

| Field Name           | Data Type     | Type	Category     |
| -------------------- | ------------- | ----------------- |
| satisfaction_level   | Quantitative  | Discrete          |
|last_evaluation	     | Quantitative	 | Discrete          |
| number_project	     | Quantitative	 | Discrete          |
| average_montly_hours | Quantitative	 | Discrete          |
| time_spend_company	 | Quantitative	 | Discrete          |
| Work_accident	       | Qualitative	 | Asymmetric Binary |
| left	               | Qualitative	 | Asymmetric Binary |
| promotion_last_5years| Qualitative	 | Asymmetric Binary |
| department	         | Qualitative	 | Nominal           |
| salary               | Qualitative	 | Ordinal           |

There are two categorical data: 
1.	Department
2.	Salary

| Category Name | Category Type |
| ------------- | ------------- | 
| Department    | Accounting    |
|               | HR            |
|               | IT            | 
|               | Management    |
|               | Marketing     |
|               | Product_mng   |
|               | RandD         |
|               | Sales         |
|               | Support       |
|               | Technical     |
| Salary	      | High          |
|               | Medium        |
|               | Low           |

### 3.	Research Problems 
The primary goal of our research is to find a solution for the problem of the best and most experienced employees leaving the company prematurely. These are some of the researched problems which we want to explore:

- Exploring number of employees and projects distributed over departments and check if any department is under staffed leading to high load on the existing employees and having no balance in work and personal life.
- Check the satisfaction level of employees over their duration of tenure to check if it reduced over time.
- Considering different parameters like time_spend_company, number_project, and salary against people who have left company in past, we can determine which of these reasons impact the most in losing talent.
- We will explore employee details and analyze the ones that need to be retained.
- A company needs to know which employees were valuable and have left or might leave. 

### 4.	Potential Solutions
- For problems like the first one listed above we are planning to have plot of number of employees, number_project and department to compare the allocation of staff and number of projects per department. This can help us analyze that if a certain department has more number of projects and very few employees allocated, the HR needs to provide that department with more number of employees to balance the amount of work distributed.
- For problems like 3 and 4, we will analyze data set by considering all the factors and determining their statistical descriptions like (mean, mode, median, variance, etc.) and finding correlations between the parameters to see how influential they are.
- We will plot bar graphs before different parameters against “left” to check their impact on people leaving the company.
- We will build and compare different models and determine the best model that helps us understand what leads to employees leaving the company.
- Our model should be able to determine employees probable on leaving the companies and this will help the company to reach out to them, in order to retain the talent. This can be done department wise or taking into consideration other factors like time_spend_company for retaining experienced employees.

### 5.	Evaluations
Our approach for evaluation of the model will progress something like this:
- We have already identified the dependent(left) and independent (rest of the variables) variables and the hypothesis we need to build out model on.
- We have analyzed our categorical data which are salary and department.
- We will determine correlations between the variables before and after model selection(VIF) to find the effect of the variables on each other.
- We will plot scatter plots to check the variance of data and determine if any transformation is required or not.
- For Model selection and evaluation, we will use hold-out metric to split them into Train data and test data. We will use “train data” for model selection and “test data” for model evaluation based on RMSE values. Models having higher RMSE will be rejected.
- In model selection we will identify the most significant variables and eliminate the in significant using hypothesis testing.

### 6.	Expected Outcomes
Based on the model we should be able to determine the factors that most likely lead to the premature resignation of the talent. The model is expected to help us analyze and determine why are the best and experienced employees are leaving the company.
The model will help us determining employees most probable to leave but are an asset to the company. If done against different departments, their respective managers can be informed about it.







