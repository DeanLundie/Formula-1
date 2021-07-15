# **Formula-1** 

<p align="center">
  <img src="https://user-images.githubusercontent.com/86531906/125710546-9a95c6e6-4cde-4b68-a3d8-ccfcddc53310.jpeg" alt="ferrari-sf21-f1-2021-f1-cars-2021-formula-one-world-3840x2160-4865"/>
</p>

## **Summary**
There are two primary aims of this project. The first is to predict Formula 1 podium positions using machine learning models. This will involve collecting and preprocessing historical F1 data to make it suitable for model comparisons. The second objective is to use this model to estimate expected returns from betting on driver's performance for an entire F1 test season

## **Workflow**
This project can be broadly split into 4 stages:

* **1\. Data Collection / Acquisition**
* **2\. Exploration**
* **3\. Comparison of machine learning models**
* **4\. Expected return from betting**

Each of these stages will have an accompanying Jupyter notebook

## **Data**
The data was obtained from two main sources; the [Ergast](https://ergast.com/mrd/) API and the official [Formula 1](https://www.formula1.com/en/results.html/1950/races/94/great-britain/race-result.html)
website. From these sources we have been able to convert the dataframes into the following csv files:

* *race.csv* - Contains metadata about historical F1 Grand Prixs since 1950, such as the season, circuit and corresponding wikipedia url
* *results.csv* - Contains information about the results of each race in each Grand Prix, including finishing positions, grid positions, total race time and status
* *drivers_standings.csv* - Contains data about the drivers standings in the Driver's Championship, including variables like current points, number of wins in the current season and their current position in the championship
* *constructor_standings.csv* - Contains identical data as the driver standings csv except in terms of the Constructor's Championship
* *qualifying_results.csv* - Contains the qualifying time for each driver in each race for each season
* *weather_info.csv* - Contains descriptors about the weather (e.g. 'Sunny' or 'Rainy) in each race which has been recoded into binary variables
