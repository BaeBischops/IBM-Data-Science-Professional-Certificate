# House Sales in King County, USA

## Introduction
The aim of this analysis is to assist a Real Estate Investment Trust in determining the market price of houses in King County, USA. This report presents an overview of the dataset used, data cleaning steps, exploratory data analysis, and the development of predictive models for house prices.

## Dataset Overview
The dataset contains information on house sale prices in King County, including attributes such as square footage, number of bedrooms, bathrooms, floors, waterfront view, and others. It spans from May 2014 to May 2015. The dataset has been preprocessed and modified for analysis purposes.

## Methodology
The analysis follows a structured approach outlined in the project instructions. This includes:

1. Importing necessary libraries such as pandas, matplotlib, seaborn, and scikit-learn.
2. Data cleaning steps, including handling missing values and dropping unnecessary columns.
3. Exploratory data analysis to understand the distribution of features and their relationships with the target variable (house prices).
4. Building linear regression models to predict house prices based on various features.
5. Evaluation of model performance using metrics such as R-squared.

## Results and Findings
### Data Cleaning
* The dataset contained missing values in the 'bedrooms' and 'bathrooms' columns, which were replaced with the mean values of their respective columns.
* Columns 'id' and 'Unnamed: 0' were dropped as they provided no relevant information for the analysis.
### Exploratory Data Analysis
* The distribution of the number of floors in houses was analyzed, revealing the frequency of houses with unique floor values.
* A boxplot analysis showed that houses with a waterfront view tend to have more price outliers compared to those without.
* A scatterplot analysis indicated a positive correlation between the square footage above ground ('sqft_above') and house prices.
* The correlation matrix highlighted features most correlated with house prices, with 'sqft_living' having the highest correlation.
### Linear Regression Modeling
* A simple linear regression model was built to predict house prices based on the square footage of living space ('sqft_living'), resulting in an R-squared value of 0.493.
* A multiple linear regression model using a set of features achieved an R-squared value of 0.658.
* Utilizing a pipeline approach with cross-validation, a Ridge regression model achieved an R-squared value of 0.659 on the training data.
* Employing second-order polynomial transformation followed by Ridge regression led to an R-squared value of 0.742 on the testing data.

## Conclusion
The analysis provides valuable insights into factors influencing house prices in King County, USA. Features such as square footage, number of bedrooms, bathrooms, waterfront view, and location play significant roles in determining house prices. The developed predictive models demonstrate reasonable accuracy in estimating house prices based on these features, with the polynomial regression model yielding the highest performance. Further refinement and validation of the models could enhance their predictive capabilities, aiding the Real Estate Investment Trust in making informed investment decisions.