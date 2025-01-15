# Business Problem

In this section, we will go through the **[Hitters](https://www.kaggle.com/datasets/floser/hitters)** dataset as firstly analyzing the data, then preprocessing it and lastly creating 3 different models with different algorithms which they will be used respectively;
* Ridge
* Lasso
* ElasticNet

To conclude, we will apply a comparison between the models to indicate the performance changes.


# Main Headings

* Dataset Story
* Required Libraries
* Importing the Dataset
* Exploratory Data Analysis (EDA)
  * General Information About the Dataset
  * Analysis of Categorical and Numerical Variables
  * Target Analysis
  * Correlation Analysis
* Data Preprocessing
  * Missing Value Analysis
  * Outlier Analysis
  * Encoding
* Ridge Regression
  * Creating a Base Ridge Model
  * Loading a Base Ridge Model & Prediction
  * Tuning the Ridge Model
  * Loading a Tuned Ridge Model & Prediction
* Lasso Regression
  * Creating a Base Lasso Model
  * Loading a Base Lasso Model & Prediction
  * Tuning the Lasso Model
  * Loading a Tuned Lasso Model & Prediction
* ElasticNet Model
  * Creating a Base ElasticNet Model
  * Loading a Base ElasticNet Model & Prediction
  * Tuning the ElasticNet Model
  * Loading a Tuned ElasticNet Model & Prediction


# Dataset Story

This dataset was originally taken from the StatLib library which is maintained at Carnegie Mellon University. This is part of the data that was used in the 1988 ASA Graphics Section Poster Session. The salary data were originally from Sports Illustrated, April 20, 1987. The 1986 and career statistics were obtained from The 1987 Baseball Encyclopedia Update published by Collier Books, Macmillan Publishing Company, New York.

Format

A data frame with 322 observations of major league players on the following 20 variables.

* AtBat Number of times at bat in 1986
* Hits Number of hits in 1986
* HmRun Number of home runs in 1986
* Runs Number of runs in 1986
* RBI Number of runs batted in in 1986
* Walks Number of walks in 1986
* Years Number of years in the major leagues
* CAtBat Number of times at bat during his career
* CHits Number of hits during his career
* CHmRun Number of home runs during his career
* CRuns Number of runs during his career
* CRBI Number of runs batted in during his career
* CWalks Number of walks during his career
* League A factor with levels A and N indicating player’s league at the end of 1986
* Division A factor with levels E and W indicating player’s division at the end of 1986
* PutOuts Number of put outs in 1986
* Assists Number of assists in 1986
* Errors Number of errors in 1986
* Salary 1987 annual salary on opening day in thousands of dollars
* NewLeague A factor with levels A and N indicating player’s league at the beginning of 1987
