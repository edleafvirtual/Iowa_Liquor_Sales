![Banner](https://github.com/edleafvirtual/Project-2.-Iowa_Liquor_Sales/blob/main/Iowa%20Sales%20Banner.png)

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

![Iowa Map](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/VOL%20sold%20sum.png "Iowa Map")


Based on our Pareto Analysis in [Part A:](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Part_A--Exploratory_Analysis.ipynb "Part A:"), we determined which counties represent around 80% of Volume Sold (Gallons) in 2019, 2020, and 2021. Following is a graph showing the top counties, sorted by volume sold, hued by quarter.

![Pareto](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Vol%20Sold%20pareto%20(2).png "Pareto")


## Outcome
#### [Part A:](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Part_A--Exploratory_Analysis.ipynb "Part A:") Data Insights.
1.- According to Iowa State data, the Top 10 counties with the highest volume sale (gallons) were identified. Using the bar chart below, we can see that the highest volume of sales occurs in the last quarter of the year. As we are in August 2022, if the Iowa Alcoholic Beverages Division wants to make improvements, it must be careful not to affect the highest volumes reported by the end of the year.

![Top 10](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Top%2010%20volume%20sold.png "Top 10")


2.- By evaluating profit performance by county, our stakeholder (Iowa Alcoholic Beverages Division) hoped to have a better idea of the focus point, thus reducing checkpoint downtime. In Part A of the study, we developed coding to determine which counties account for 80% of the volume sold, and which counties account for 80% of the state's profit. Using both lists, we identified 22 counties, as shown in the graph below.

![22 counties](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/PROFIT%20pareto%20location.png "22 counties")

According to the packed bubbles graph below, these are the top ten counties in terms of profit and volume sold in 2019, 2020, and 2021.

![Top 10](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Iowa%20Top%2010%20volume%20sold%20profit.png "Top 10")

#### [Part B:](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/Part_B--ML_Modeling.ipynb "Part B:") Predictive Model.
1.- This part of the project produced the best results for each regression model tested. Below are the graphs showing the best results for each model. Based on the results, Random Forest is the model of choice. It has a lower MAE, meaning that is more accurate, and the highest R2 Score meaning is the most precise.   

![ML Metrics](https://github.com/edleafvirtual/Iowa_Liquor_Sales/blob/main/ML%20metrics.png "ML Metrics")

## Recomendations
1.- Select 1% of the data per year (2012 - 2021), concatenate them in order to re-do the Part B of the project. The model should learn from yearly behavior.

2.- Tune the hyperparameters of the predictive model selected, using multiple [cross-validation](https://towardsdatascience.com/hyperparameter-tuning-the-random-forest-in-python-using-scikit-learn-28d2aa77dd74 "cross-validation") methods. 

3.- Once the model is tuned, we would use its predictive values in order to plot more insights and also to show what our predictions look like. Subsequently in January 2023 when real data from 2022 were available in the data [source](https://data.iowa.gov/Sales-Distribution/Iowa-Liquor-Sales/m3tr-qhgy "source"), we will be able to compare our model. This analysis would deliver some insights about the approach to be done by Data Engineering, to then enrich our Machine Learning process in order to deliver a product that could predict more precise and accurate future scenarios.

## Limitations
- Splitting the data for Visual Exploration considering only 2019, 2020, and 2021 because of technical limitations (RAM/memory), is something that could have affected the final result. Trying to use some [ETL tools](https://www.geeksforgeeks.org/top-7-python-etl-tools-to-learn/?ref=gcse "ETL tools") or a cloud environment like AWS sounds to be a great solution.

- By tuning our chosen predictive model, we should find the best environment for this task without burning time because of RAM\memory issues. It's true that Data Engineering could have a better effect on our model than just tuning, but selecting the right hyperparameter is very important.


## Credits
### Eduardo Galindez
<p>
  <a href="https://www.linkedin.com/in/eduardogalindez/" rel="nofollow noreferrer">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="linkedin">
  </a> &nbsp; 
  <a href="https://github.com/edleafvirtual" rel="nofollow noreferrer">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="github">
  </a>
</p>
