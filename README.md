# COD-Internship-Task2

Name : Pranav Khilnani Domain : Data Science ID : CT12DS213 Duration : 8 weeks

Descryption:

In this analysis, we aimed to predict car prices using various features from our dataset. Here’s a step-by-step breakdown of our approach:

**1. Data Loading and Preparation**:
- We started by importing essential libraries and loading our car price dataset from Google Drive. We then checked the first and last few rows of the data to understand its structure.
- We examined the shape of the dataset, column names, data types, and validated missing values. We found no missing values but identified duplicate rows and removed the 'car_ID' column, which was unnecessary for our analysis.

**2. Descriptive Statistics and Categorical Features**:
- We displayed descriptive statistics to summarize the central tendency, dispersion, and shape of the dataset’s distribution.
- We identified categorical features and calculated the number of unique values for each category column. These categorical features were then encoded using LabelEncoder to convert them into numerical values suitable for our regression model.

**3. Feature Correlation**:
- We visualized the correlation of various features with the target variable 'price' using a bar plot. This helped us identify the most influential features affecting car prices.
- The correlation matrix provided insights into how strongly each feature was related to the price, guiding us in feature selection.

**4. Model Building and Evaluation**:
- We defined our feature vector (X) and target variable (y). The features were then scaled using StandardScaler to standardize the dataset.
- The data was split into training and testing sets, with 80% for training and 20% for testing. We used a Linear Regression model, training it on the training set.
- Predictions were made on both training and testing sets. We evaluated the model’s performance using Mean Squared Error (MSE) and R-squared (R²) metrics for both sets. The results provided an understanding of the model’s accuracy and generalizability.

**5. Visualization**:
- We visualized actual vs. predicted prices for both training and testing sets using scatter plots. These plots illustrated how well the model’s predictions aligned with the actual prices.
- Additionally, we visualized the regression line for a single feature, ‘engine size,’ to demonstrate the relationship between this feature and car prices in the training data.

Through this analysis, we gained insights into the factors affecting car prices and built a predictive model to estimate car prices based on these features.

Conclusions: 

Here are the key points and conclusions derived from the analysis:

1) Data Quality and Integrity:

Missing Values: There are no missing values in the dataset, ensuring data completeness.
Duplicate Rows: No duplicate rows were found, indicating data uniqueness.

2) Descriptive Statistics:

The dataset includes 205 observations and 25 features (after dropping the car_ID column).
The mean price of the cars is approximately 13,276.71 $, with a standard deviation of 7,988.85 $.
The dataset covers a wide range of prices, from 5,118 $ to 45,400 $ .

3) Categorical Features:

There are several categorical features such as CarName, fueltype, aspiration, doornumber, carbody, drivewheel, enginelocation, enginetype, cylindernumber, and fuelsystem.
The CarName feature has the highest number of unique values (147), indicating a diverse set of car models.

4) Feature Correlations with Price:

Strong Positive Correlations: Features like enginesize (0.874), curbweight (0.835), and horsepower (0.808) have strong positive correlations with the price.
Moderate Positive Correlations: Features like carwidth (0.759), carlength (0.683), and drivewheel (0.578) show moderate positive correlations.
Negative Correlations: Features like citympg (-0.686) and highwaympg (-0.698) have strong negative correlations with price, indicating that higher fuel efficiency tends to be associated with lower prices.

5) Model Performance:

Training Set Performance:

Mean Squared Error (MSE): 6,278,621.90
Root Mean Squared Error (RMSE): 2,505.72
Mean Absolute Error (MAE): 1,833.32
R-squared: 0.8854
Testing Set Performance:

Mean Squared Error (MSE): 10,739,032.94
Root Mean Squared Error (RMSE): 3,277.05
Mean Absolute Error (MAE): 2,427.73
R-squared: 0.8860

The model performs well on both the training and testing sets, with high R-squared values indicating that the model explains approximately 88.5% of the variance in the car prices. However, the higher RMSE and MAE values on the testing set suggest room for improvement in predictive accuracy.
