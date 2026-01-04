# final-___project
This project is a system that predicts whether a user will reorder a specific product or not, based on "Instacart" data.
We performed the following steps:
•	Data Preparation: We imported the essential libraries (Pandas, Numpy, Scikit-learn) and loaded the orders, products, and departments data.
•	Merging Tables: Linking data together (Merge) to create a single table containing order details (such as hour and day) along with product details and its corresponding department.
•	Memory Cleaning: Used gc.collect() and del to remove temporary tables to save memory space, which is a smart move given the large data size.
•	Exploratory Data Analysis (EDA): Drawing charts that show the distribution of reordered products, the number of products per order, and the peak hours and days for ordering.
•	Feature Engineering: We calculated important metrics such as:
o	For the user: Total orders, total products purchased, and their reorder rate.
o	For the product: How many times it was ordered and its reorder frequency.
o	For the relationship: How many times this specific user bought this specific product.
•	Model Building:
o	Took a sample (300,000 records) to speed up training.
o	Split the data into training and testing sets (80/20).
o	Used the Logistic Regression model as a starting point.
o	Used the Decision Tree model to improve results.
•	Evaluation: Calculated Accuracy, and plotted the Confusion Matrix and AUC curve to verify the quality of the model's predictions.

