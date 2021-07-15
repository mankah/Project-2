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
 We first clean the data by handling null values and instituting the correct data types.  We also remove outliers that are three or more standard deviations from the mean in the 'bathrooms', 'bedrooms', and 'sqft_living' features.  We perform some EDA by exploring correlations and inspecting features, then make some inferential plots showing relationships between price and various features.  We create a baseline model for reference, and then begin an iterative process of model-making, creating nine models (plus one baseline model) in total.  For each model, we created training and test data, used cross-validation, and calculated R2 and RMSE.  
    
    
## Results
Models 7 and 9 are polynomic, the others are not.  The models produced the R2 training scores and RMSE's as follows:

 
	Train Score	Test Score	 RMSE 
Model 1	0.692		 $168,660 
Model 2	0.756		 $164,378 
Model 3	0.871		 $121,705 
Model 4	0.871		 $121,678 
Model 5	0.871		 $121,678 
Model 6	0.869		 $120,124 
Model 7	0.859		 $133,793 
Model 8	0.858		 $137,291 
Model 9	0.918		 $104,136 ![image](https://user-images.githubusercontent.com/82840623/125812005-debaf0eb-40e9-439c-846a-10924b635668.png)

    
    
## Conclusions
The average home price in King County is $540,297, with an average price per square foot of $264.  Using this square foot price to predict each house price (a commonly used benchmark) produces a RMSE of $262,267. In order to be useful, our model needs to perform better than this.  
    
    
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
