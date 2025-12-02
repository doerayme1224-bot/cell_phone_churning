<div style="display: flex; align-items: center; justify-content: center; text-align: center;">
  <img src="https://coursereport-s3-production.global.ssl.fastly.net/uploads/school/logo/219/original/CT_LOGO_NEW.jpg" width="100" style="margin-right: 10px;">
  <div>
    <h1><b>🧪 Lab - Cell Phone Churning</b></h1>
  </div>
</div>

## Data Set: 
The dataset contains information on customers' cell phone plan usage, including details such as call duration, text message counts, data usage, and any additional features that might be indicative of customer behavior.

## Objective: 
In the context of cell phone plan churning, the objective is to build a predictive model that anticipates whether a customer is likely to unsubscribe or switch to another cell phone plan. Churning, in this scenario, refers to the customer discontinuing their current plan. The primary goal is to develop a predictive model that can classify customers as either potential churners or non-churners based on their plan usage patterns. Identifying potential churners in advance allows the service provider to take proactive measures, such as targeted marketing promotions or personalized retention offers, to retain customers and minimize subscription losses.

---

## PART 1: Data Cleaning
Before diving into the modeling process, it's crucial to ensure that your data is clean and ready for analysis.

- **Check null values:** Examine the dataset for any missing values. Addressing null values is essential to prevent issues during model training and evaluation.

- **Check dtypes:** Ensure that the data types of your features are appropriate. This step is important for avoiding potential discrepancies between the expected and actual data types.

## PART 2: Exploratory Data Analysis (EDA)
Exploring your data helps you gain insights and identify patterns or trends. Consider the following steps:

- **Visualize the data:** Utilize seaborn's `pairplot` to create a visual representation of relationships between different variables. This can offer a preliminary understanding of how features correlate with each other.
- Feel free to create other visualizations as well!
  
## PART 3: Modeling

Now that your data is clean and you've explored its characteristics, it's time to build and evaluate your models.

- **Establish baseline accuracy score:** Before training any models, establish a baseline accuracy score. This provides a benchmark for evaluating the performance of your models.

- **Train-test-split with `random_state = 42`:** Split your data into training and testing sets using `train_test_split` with a specified random state. This ensures reproducibility in your results.

- **Normalize your data with `StandardScaler`:** Standardize your features using `StandardScaler` to ensure that they are on a similar scale. This step is particularly important for algorithms sensitive to the scale of input features, such as K-Nearest Neighbors.

- **Evaluate K-Nearest Neighbors (KNN):**
  - Set \( k = 5 \) and calculate the training/testing accuracy scores. Explore whether the model performs better with other values of \( k \). <br>

- **Try Logistic Regression and RandomForestClassifier:**
  - Experiment with alternative models such as Logistic Regression and RandomForestClassifier. Compare their performance against the KNN model to identify the most suitable algorithm for your specific classification task.
  - For each model, include a confusion matrix to assess its performance in terms of true positives, true negatives, false positives, and false negatives.
