# Welcome to CattleTEC!


Helping you take control of your herd's tomorrow, today!

![CattleTEC](CattleTEC-PNG.png "CattleTEC Logo")

## Background
Goal is to use Data to Help Cow/Calf Producers Make Better Management Decisions to Increase Profitability

* Extremely volatile and uncertain markets for agricultural commodities
  * Unexpected weather
  * Global politics
* Many cow/calf producers today don’t have records of their operation
  * Time / Other priorities
  * Numerous variables making it difficult to be organized
* Factors on Profitability
  * Weather Patterns  :x:
  * Markets :x:
  * Input / Feed Costs  :white_check_mark:

## Data Analysis Task
An important feature of CattleTEC is being able to market forecast. The goal of this project is to bring in commodity values that matter to cow/calf producers and display them in a quick and easy to understand format that allows the user to refine and select out what timeframe of the markets they would like to explore. In addition, we are also developing a machine learning algorithm that will analyze the commodity trends from previous years in order to forecast out what the markets will do before they occur. This will  give farmers a competitive advantage when marketing their animals.

## Data Inputs
The Farmer can decide:
* Timeframe of the Market
* Commodities
* Point of Interest

So we brought in Quandl data on the CME for Corn, Live Cattle, and Feeder Cattle. This gave us information including opening price, closing price, highest daily price, lowest daily price, volume traded, and daily change for all three commodities. 


## Project Workflow
Here you can see a brief layout of how we intend
to accomplish our project for ABE 516X this semester


![Project Workflow](516-Project.png "WorkFlow")

## Results
First we started by pulling in cattle prices for both feeder and live cattle from September 2010 to September 2019 so that we could display this.
![Cattle Prices](CattlePrices.png "Cattle Prices")
We also brought in corn prices during that time frame
![Corn Prices](CornPrices.png "Corn Prices")
We used LSTM neural network training for our machine learning algorithm and started with our baseline prediction which essentially just averaged the last 50 days closing price to predict the next days
![Baseline Predictions](BaselinePrediction.png "Baseline Predictions")
We then moved to a slightly more elaborate model which took into account all of the data we were giving it and attempted to predict one point a set amount of days later. For this one we took 300 days worth of data and attempted to go 30 days forward. The results are seen below.
![Single Step Predictions](SingleStepPredictions.png "Single Step Predictions")
Finally we wanted to try to predict every day to see how well our trends matched. So we again used all of the data for the last 300 days but tried to predict each of the next 30 days. This was a disappointing result as you can see below as it didn't appear to correlate well at all.
![Multi Step Predictions](MultiStepPredicitons.png "Multi Step Predictions")

## Topics Relevant to ABE 516X 
Incorporation of topics relevant to this class  - what from the class did you use in this project and why might it be useful for research projects like this?  What are the advantages and disadvantages?  Were there any assumptions or transformations needed?



## Automate and Reproduce Analysis
Ability to automate and reproduce your analysis (if the file input were to change, could this analysis be reproduced and how easily?)  - how will someone else reproduce this analysis?  Is the data stored somewhere?  Can I reproduce the figures easily?



## Assignment
Creation of one assignment based on your dataset for the class to complete - one can think of this of a task or homework assignment based on your project.



