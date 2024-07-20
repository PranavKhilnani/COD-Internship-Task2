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
