# Predicting the Age of Crabs: A Machine Learning Approach

This repository contains a machine learning project focused on predicting the age of crabs based on various physical characteristics. The goal of this study is to develop a predictive model that can accurately estimate the age of crabs using features such as length, diameter, height, weight, and sex.

## Overview
The dataset initially provided only included seven input features and a target column for prediction, which was not sufficient. To improve the predictive capabilities, feature engineering techniques were applied. Additionally, five different machine learning algorithms were utilized with their respective hyperparameters, and the best model for age prediction was determined. The model was then saved using the pickle library for future use.

## Problem Statement
The objective of this project is to build a machine learning model that can accurately predict the age of crabs based on various physical measurements. The dataset contains information on the gender, weight, carapace length, carapace width, and abdomen width of crabs, as well as their actual age. The model should be able to take in these features as input and output a prediction of the crab's age in years. This type of predictive model could be useful in the fishing and seafood industry, where the age of crabs is an important factor in determining their quality and market value.

## Data Cleaning
Data cleaning steps were performed to prepare the dataset for analysis. Outliers were identified and removed using the interquartile range (IQR) method. 

## Exploratory Data Analysis\

In this project, we conducted an Exploratory Data Analysis (EDA) to gain insights into the dataset and understand the relationship between various physical characteristics and crab age.

### Scatter Plot: Relationship between Length and Age
![Scatter Plot](scatter plot.png)

Using a scatter plot, we explored the relationship between the length of the crab and its age. Although there appears to be a positive correlation, we cannot determine causality from the scatter plot alone.

### Histogram: Distribution of Age
![Hist Plot](hist plot.png)

We generated a histogram to visualize the distribution of age. The histogram reveals a normal distribution of age in the dataset.

### Violin Plot: Age by Sex
![Violin Plot](violin plot.png)

By using a violin plot, we examined the distribution of age based on the crab's sex. The plot shows a bulge in the middle, indicating that the median age is more common than other values. This suggests that the distribution may be skewed towards the median or have more observations around it.

### Box Plot: Distribution of Age by Sex
![Box Plot](box plot.png)

We created a box plot to compare the distribution of age between male and female crabs, as well as intermediate crabs. The box plots indicate that the median, quartiles, and outliers for male and female crabs are almost the same when compared to intermediate crabs.

### Pairplot: Pairwise Relationships
![Pairplot](pair plot.png)

The pairplot illustrates the pairwise relationships between the variables length, diameter, height, weight, and age, with the points colored by the sex variable. Upon examining the age pairwise with other columns, we observed better correlations between age and other features.

### Heatmap: Correlation Matrix
![Heatmap](correlation matrix.png)

Using a heatmap, we visualized the correlation matrix to measure the linear relationship between different features and crab age. The heatmap highlights that shell weight and diameter have the highest correlation with age.

The EDA provided valuable insights into the dataset, allowing us to identify potential relationships and important features for predicting the age of crabs.



## Feature Engineering
Feature engineering techniques were applied to create additional features that could enhance the predictive performance of the models. This included the calculation of the body mass index (BMI), ratios of different measurements, interactions between measurements, and polynomial features. These new features were incorporated into the models to capture complex patterns and relationships.

## Best Model Selection
Five different machine learning algorithms were trained and evaluated using appropriate evaluation metrics such as mean absolute error, mean squared error, and R-squared. The performance of each model was compared, and the random forest algorithm was found to provide the best performance with an R-squared value of 0.58.

## Conclusion
The developed machine learning model using the random forest algorithm demonstrated the potential to accurately predict the age of crabs based on physical characteristics. However, further improvements can be made to enhance the model's accuracy. The project highlights the application of machine learning techniques in predicting crab age and their potential use in the fishing and seafood industry.

## Repository Contents
-  [notebook.ipynb](https://github.com/Aravinth-Megnath/Crab_age/blob/crab1/crab_age_prediction.ipynb) - Jupyter Notebook containing the complete analysis.
- [data](https://github.com/Aravinth-Megnath/Crab_age/blob/crab1/CrabAgePrediction.csv) - Folder containing the dataset used in the analysis.
- [models](https://github.com/Aravinth-Megnath/Crab_age/blob/crab1/rf_model.pkl) - Folder containing the saved machine learning model.



## Usage
To replicate the analysis and run the Jupyter Notebook, follow these steps:
1. Clone this repository: `git@github.com:Aravinth-Megnath/Crab_age.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the Jupyter Notebook: `jupyter notebook notebook.ipynb`

Please note that the dataset and saved model files should be placed in the appropriate folders as specified in the notebook.

## Future Work
- Further fine-tuning of the model's hyperparameters to improve prediction accuracy.
- Experimenting with additional feature engineering techniques to capture more complex relationships.
- Collecting additional data to expand the dataset and enhance the model's generalizability.

## Credits
This project was developed by [Aravinth Meganathan](https://github.com/Aravinth-Megnath). If you have any questions or suggestions, please feel free to contact me.

