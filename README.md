# Predicting Real Estate Sale Prices in King County, WA *<Appraisal Firm>*
 
**Authors**: *Ben Bowman, Anthony Conte, Nina Vergara, Manav Kahlon*
  
## Overview
- [Overview](#Overview)
- [Business Problem](#Business-Problem)
- [Data](#Data)
   - [House_Data](#Housing-Data)
- [Methods](#Methods)
- [Results](#Results)
    - [](#<>)
    - [<>](#<>)
    - [<>](#<>)
- [Conclusions](#Conclusions)
- [For More Information](#For-More-Information)
- [Repository Structure](#Repository-Structure)
  

## Business Problem
Acme Appraisals wants to find a more efficient way to predict the price of a house in Seattle when doing its appraisals. We are tasked with making a model that will be the best at predicting the price of a house while limiting the predictions error.   
 
## Data
21597 records of home sales in King County, WA.  
#### Housing Data
    * kc_house_data.csv
    
    
## Methods
 We first clean the data by handling null values and instituting the correct data types.  We also remove outliers that are three or more standard deviations from the mean in the 'bathrooms', 'bedrooms', and 'sqft_living' features.  We perform some EDA by exploring correlations and inspecting features, then make some inferential plots showing relationships between price and various features.  We create a baseline model for reference, and then begin an iterative process of model-making, creating nine models (plus one baseline model) in total.  For each model, we create training and test data, use cross-validation, and calculate R2 and RMSE.  
    
    
## Results
Models 7 and 9 are polynomic, the others are not.  The models produced the R2 training scores and RMSE's as follows:

  ![image](https://user-images.githubusercontent.com/82840623/125812005-debaf0eb-40e9-439c-846a-10924b635668.png)

    
    
## Conclusions
The average home price in King County is $540,297, with an average price per square foot of $264.  Using this square foot price to predict each house price (a commonly used benchmark) produces a RMSE of $262,267. In order to be useful, our model needs to perform better than this.  Every one of our nine models does this, so based on this metric our model(s) would be useful to the appraisal company.  Model 9 gives the lowest RMSE and just over $100k, though we suspect that there is some overfitting due to discrepancies between R2 scores for the train and test data.  Model 6 is our best non-polynomic model with an RMSE of around $120k, so that is a good option. Overall, the overfitting in model 9 concerns us, so we will accept a higher bias in exchange for less variance and recommend model 6 to the appraisal firm.  
    
    
## For More Information
    
Please review our full analysis in [our Jupyter Notebook](./Notebook.ipynb) or our [Microsoft Powerpoint](./Microsoft_powerpoint.pdf).    
    
## Repositroy Structure
 ```
├── data                                <- Sourced from an external source
├── gitignore                           <- python files to ignore 
├── Group_1_Technical_Notebook.ipynb    <- The steps taken to acheive our endgoal
├── Microsoft_powerpoint.pdf            <- PDF of our project presentation                        
└── README.md                           <- The README.md

```
