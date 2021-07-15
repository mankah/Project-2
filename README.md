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
 We first clean the data by handling null values and instituting the correct data types.  We also remove outliers that are three or more standard deviations from the mean in the 'bathrooms', 'bedrooms', and 'sqft_living' features.  We perform some EDA by exploring correlations and inspecting features, then make some inferential plots showing relationships between price and various features.  We create a baseline model for reference, and then begin an iterative process of model-making, creating nine models in total.  
    
    
## Results
    
    
    
## Conclusions
    
    
    
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
