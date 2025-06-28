# Prediction-of-Product-Sales

This project analyzes sales data to uncover insights and build predictive models that forecast future sales trends.

## Key Visuals

### 1. Sales by Category
The fat by Item and its distribution by tiers
![Screenshot 2025-05-11 220200](https://github.com/user-attachments/assets/253d5c1d-cb88-4c72-85e4-fecc06f8ccb4)
 


### 2. Sales Over Time
The relationship between the numerical data
![Screenshot 2025-05-11 220150](https://github.com/user-attachments/assets/2d381d87-e648-4b0d-b1e5-0baccdd174e1) 

### 3. Distribution of Item Types in the Dataset
![Screenshot 2025-06-28 124028](https://github.com/user-attachments/assets/cab7afc3-e193-4f0e-9130-f8ef62e27588)

This bar chart shows the frequency of each product category in the dataset.

There are 16 unique item types, with no missing values.

Fruits and Vegetables is the most common category, comprising approximately 14.5% of all records.

Other categories like Frozen Foods and Household also have high counts, indicating diverse product representation.

### 4. Sales Distribution by Item Type
![Screenshot 2025-06-28 124307](https://github.com/user-attachments/assets/8de65fe9-fd6a-4c3d-9b3a-92b275440b5e)
This visualization combines a bar plot and a scatter plot to illustrate how sales vary across product categories.

The bars show the average sales per category.

The scatter points represent individual product sales, highlighting variability within each category.

Although all categories have comparable average sales, some, like Frozen Foods and Household, exhibit a wider spread, suggesting certain items achieve significantly higher sales than others.

### 5. Evaluating best modules in predctions
 both linear refression and random forest have the same results in this data set in evaluationg the accuracy of predections as shown below
 ![Screenshot 2025-06-28 124420](https://github.com/user-attachments/assets/6559820b-5cf4-44ec-834f-fc1d5d9689b2)

 While the gridsearch have another results as shown below
 ![Screenshot 2025-06-28 124443](https://github.com/user-attachments/assets/ca7d4ce3-7ff0-47cb-b50f-0bfcdeddd13d)

I recommend implementing the Linear Regression model for this dataset based on this, R-squared is a measure of how well the model explains the variance in the data. For the Linear Regression model, the R^2 score is 0.938 on the training data and 0.552 on the test data. This means that the model explains approximately 93.8% of the variance in the training data and 55.2% of the variance in the test data.

I recommend using RMSE (Root Mean Squared Error) to express the model’s performance to a stakeholder.I recommend using RMSE (Root Mean Squared Error) to express the model’s performance to a stakeholder, because it gives us a single number that represents the average size of the prediction errors, in the same units as the target variable (e.g., dollars, units sold, etc.). This makes it much easier to interpret for someone without a technical background.

The model performs very well on the training data, explaining 93.8% of the variation and having a low error (RMSE = 428.651). However, when applied to unseen test data, the performance drops significantly — it explains only 55.2% of the variation, and the error more than doubles (RMSE = 1,111.454).


