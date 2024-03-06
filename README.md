# Ames Housing Predict

The purpose of this project is to utilize predictive modeling techniques to forecast the sale prices of houses in Ames, IA. Given the upward trend in house prices over the past decade, the aim is to develop accurate models that can anticipate future sale prices based on various factors, such as overall material and finish quality, first floor square feet, and neighborhood, etc. By analyzing training data and applying several regression methodology, this endeavor aims to furnish accurate house sale price estimates, thereby offering valuable insights for buyers, sellers, and investors in the Ames, IA.



# Data Dictionary


|Feature|Type|Description|
|---|---|---|
|**Overall Qual**|*integer*|Overall material and finish quality|
|**Gr Liv Area**|*integer*|Above grade (ground) living area square feet|
|**Total Bsmt SF**|*float*|Total square feet of basement area|
|**Garage Area**|*float*|Size of garage in square feet|
|**1st Flr SF**|*integer*|First Floor square feet|
|**Garage Cars**|*float*|Size of garage in car capacity|
|**Year Built**|*integer*|Original construction date|
|**Year Remod/Add**|*integer*|Remodel date|
|**Full Bath**|*integer*|Full bathrooms above grade|
|**Garage Yr Blt**|*float*|Year garage was built|
|**Mas Vnr Area**|*float*|Masonry veneer type|
|**TotRms AbvGrd**|*integer*|Total rooms above grade|
|**Fireplaces**|*integer*|Number of fireplaces|
|**BsmtFin SF 1**|*float*|Type 1 finished square feet|
|**House Style**|*object*|Style of dwelling|
|**Neighborhood**|*object*|Physical locations within Ames city limits|
|**MS Zoning**|*object*|Identifies the general zoning classification of the sale|
|**Roof Matl**|*object*|Roof material|
|**Kitchen Qual**|*object*|Kitchen quality|
|**Foundation**|*object*|Type of foundation|
|**Lot Frontage'**|*float*|Linear feet of street connected to property|
|**Open Porch SF**|*integer*|Open porch area in square feet|
|**Wood Deck SF**|*integer*|Wood deck area in square feet|
|**Lot Area**|*integer*|Lot size in square feet|
|**SalePrice**|*integer*|The property's sale price in dollars|



# Executive Summary

Project Goal:

The objective of this project is to predict house sale prices in Ames, IA, utilizing historical training data.

Methodology:

The methodology involves several steps:

1. Data cleaning: Ensuring data quality by addressing missing values and outliers.
2. Imputation: Missing data is filled using the mean of the respective feature.
3. Feature selection: Calculating correlations between numeric features and sale price to identify influential factors.
4. Train-test split: Dividing the data into training and testing sets to evaluate model performance.
5. Model evaluation: Utilizing linear regression and LASSO regression to predict sale prices.
6. Performance metrics: Assessing model performance using metrics such as Root Mean Squared Error (RMSE), R-square, and cross-validation scores.

Key Findings:

Features such as overall quality, above ground living area square feet, total square feet of basement area, total rooms above grade, original construction date, house style, neighborhood, and foundation significantly influence both regression models.
LASSO regression outperforms linear regression with a 5-fold cross-validation score of 87.463%.

Conclusion:

Fitting all features into the LASSO model aids in generalizing to new data. The testing dataset's R-square of 88.81% suggests that approximately 88.81% of the sale price can be explained by the features in the testing dataset. Additionally, the square rooted Mean Squared Error (MSE) in the testing data for predicting sale price is 25548. These results indicate the effectiveness of the LASSO regression model in predicting house sale prices in Ames, IA.