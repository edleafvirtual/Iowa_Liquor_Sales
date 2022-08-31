![](https://www.leafwebstudio.com/wp-content/uploads/2022/08/Iowa-Sales-Banner.png)

## Iowa Alcoholic Beverages Division - 2022 Income Prediction
#### Since 2020, humanity has been facing epic challenges. The pandemic spread division within the community, making it harder to socialize and keep the microeconomics running. Our stakeholder, [Iowa Alcoholic Beverages Division](https://abd.iowa.gov/ "Iowa Alcoholic Beverages Division"), has been requested a predictive model using Machine Learning in order to be prepared for possible future scenarios.

#### Disclaimer: We must keep clear that our objective is not to design, create, and/or develop a Machine Learning model & Data Analytics to promote alcohol consumption or sales. The agreement with the stakeholder is to identify, room for improvement in order to determine how to implement an agile process to reduce non-productive time caused by Quality Control checkpoints.


<img src="https://raw.githubusercontent.com/matiassingers/awesome-readme/master/icon.png" align="right" />

## Author
#### Name: Eduardo Galindez.
#### Date: August 2022.

<img alt="GitHub followers" src="https://img.shields.io/github/followers/edleafvirtual?style=social"> <img alt="GitHub User's stars" src="https://img.shields.io/github/stars/edleafvirtual?style=social"> <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/edleafvirtual/sales_predictions2023?style=social">

## Case Study Information
#### Iowa Liquor Sales Project is an exercise that is part of Coding Dojo: Data Science Bootcamp, where I'm trying to show how Industrial Engineering and Data Science would be merged when we want to improve business process/KPI performances in current Industry 4.0.
#### 
#### General Objective:
- Prepare the data for Machine Learning to predict [Iowa Alcoholic Beverages Division](https://abd.iowa.gov/ "Iowa Alcoholic Beverages Division") 2022 income from Class E alcohol liquor sales across licensed vendors using historical data (2019, 2020, and 2021) from Iowa [Liquor Sales](https://console.cloud.google.com/marketplace/product/iowa-department-of-commerce/iowa-liquor-sales?project=lively-clover-358509 "Liquor Sales").
#### Specific Objectives:
- Set up the dataset in order to make it manageable. The [main](https://data.iowa.gov/Sales-Distribution/Iowa-Liquor-Sales/m3tr-qhgy "main") dataset has 24+ million rows, which includes the sales from January 1st, 2012 to current, making it pretty hard to work with Google Colaboratory or Jupyter.
- Choose a Target for our predictive model.
- Report insights using Visual Exploration.
- Determine which prediction model would be used to be compared with real 2022 data in January 2023.

#### Scope:
- Our study consists of two parts:
   - [Part A:](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Part_A--Exploratory_Analysis.ipynb "Part A:") Identify which counties, Iowa Alcoholic Beverages Division would implement new procedures to agile payment and inspection processes.
   - [Part B:](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Part_B--ML_Modeling.ipynb "Part B:") Create a model to predict future income from sales (Gallons).

#### General Description
A [Licensed Vendor](https://abd.iowa.gov/licensing/licensepermit-fees "Licensed Vendor") sells alcoholic liquor to a store, being responsible for paying to Iowa State the fee per bottle sold (column 'State Bottle Retail' in our dataset). The State wants to agile administrative checkpoints, whose counties are more profitable. Part of the new procedures could be extending the deadline to pay the fees.

There are a few concepts/elements that we should clarify:
  - Class E is the license to sell an unopened alcoholic liquor bottle off-premises in Iowa.
  - The 'State Bottle Retail' is a fee based on the size of the 'Pack' and the 'Bottle Volume (ml)'.
  - The ' Sale (Dollars)' is 'Bottles Sold' times 'State Bottle Retail'. This is the amount the stores pay to the Iowa Alcoholic Beverages Division per bottle sold. It's not the income per sale for store/vendor.
  - 'Volume Sold (Gallons)' represents gallons sold by a transaction (row).

Based on Iowa State's sales through 2019, 2020, and 2021, the map below shows the amount of gallons sold per county.

![Iowa Map](https://www.leafwebstudio.com/wp-content/uploads/2022/08/VOL-sold-sum-1.png "Iowa Map")


Based on our Pareto Analysis in [Part A:](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Part_A--Exploratory_Analysis.ipynb "Part A:"), we determined which counties represent around 80% of Volume Sold (Gallons) in 2019, 2020, and 2021. Following is a graph showing the top counties, sorted by volume sold, hued by quarter.

![Pareto](https://www.leafwebstudio.com/wp-content/uploads/2022/08/Vol-Sold-pareto-2.png "Pareto")


## Outcome
### [Part A:](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Part_A--Exploratory_Analysis.ipynb "Part A:"): Data Insights.


### [Part B:](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Part_B--ML_Modeling.ipynb "Part B:") Predictive Model.

## Recomendations
- *Work in progress*

## Limitations
- *Work in progress*
