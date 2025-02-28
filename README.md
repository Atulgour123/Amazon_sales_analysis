# Amazon_sales_analysis
This project performs exploratory data analysis (EDA) and predictive modeling on Amazon sales data.

**Data Loading and Preprocessing:**

1.  Loads the Amazon sales data from a CSV file.
2.  Handles missing values (though the specific method isn't shown).
3.  Converts date columns to datetime objects.
4.  Creates new features: 'Order Month', 'Order Year', 'Order Day of Week'.
5.  Renames columns for better readability.

**Exploratory Data Analysis (EDA):**

The EDA section visualizes various aspects of the sales data:

*   **Sales Analysis:** Monthly, yearly, and weekly sales trends are plotted using bar charts and line plots.  Sales are broken down by category and sub-category, using bar charts and pie charts.
*   **Profit Analysis:** Similar visualizations are created for profit, analyzed by month, year, week, category and sub-category.  Profit by category is visualized using a treemap.
*   **Sales Channel Analysis:**  Compares sales and total profit across different sales channels using grouped bar charts and a pie chart of the sales to profit ratio.

**Predictive Modeling:**

1.  Uses 'Order Month', 'Order Year', 'Order Day of  Week', and 'Sales' as features to predict 'Total Profit'.
2.  Splits the data into training and testing sets.
3.  Trains a linear regression model on the training data.
4.  Evaluates the model using Mean Squared Error (MSE) and R-squared (R2) on the test set.

**Libraries Used:**

*   **Data Manipulation:** NumPy, Pandas
*   **Visualization:** Matplotlib, Seaborn, Plotly
*   **Treemaps:** squarify
*   **Machine Learning:** scikit-learn (for linear regression and model evaluation)


**Potential Improvements:**

*   **Missing Value Imputation:** The code shows identifying missing values but doesn't show how they're handled.  Consider using appropriate imputation techniques.
*   **Feature Engineering:**  Explore additional features that might improve the predictive model (e.g., customer demographics, seasonality indicators).
*   **Model Selection:** Experiment with other regression models (e.g., Random Forest, Gradient Boosting) to compare performance.
*   **Hyperparameter Tuning:**  Optimize the hyperparameters of the chosen model to further improve performance.
*   **Model Evaluation Metrics:** Include additional evaluation metrics (e.g., MAE, RMSE).
*   **Data Cleaning:**  More in-depth data cleaning, including outlier detection and treatment, could improve results.
*   **Clarity of profit visualization:** The profit visualizations are not very informative with the current hardcoded values. They should be consistent with the original dataframe.
