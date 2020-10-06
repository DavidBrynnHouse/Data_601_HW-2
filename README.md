# David House Homework 2 due 10/8/2020

## How to Navigate this Project

* **Code** - Folder for Jupyter notebooks.
    * [Cleaning.ipynb](https://github.com/DavidBrynnHouse/Data_601_HW-2/blob/master/Code/Cleaning.ipynb) - Jupyter notebook used to pull data from API and save as csv.
    *  [Executive Analysis.ipynb](https://github.com/DavidBrynnHouse/Data_601_HW-2/blob/master/Code/Executive%20Analysis.ipynb) - Jupyter notebook containing the main analysis for this project.
* **Data** - List used to collect specific data and data pulled from api
    * [temp_humidity.csv](https://github.com/DavidBrynnHouse/Data_601_HW-2/blob/master/Data/temp_humidity.csv) - csv file with with float values of temperature and humidity data taken from several thousand U.S cities at 7pm October 5, 2020
    * [us_cities.csv](https://github.com/DavidBrynnHouse/Data_601_HW-2/blob/master/Data/us_cities.csv) - A list of several thousand U.S Cities pulled from [this](https://www.britannica.com/topic/list-of-cities-and-towns-in-the-United-States-2023068) site.
* [LICENSE](https://github.com/DavidBrynnHouse/Data_601_HW-1/blob/master/LICENSE) - MIT License
* [README.md](https://github.com/DavidBrynnHouse/Data_601_HW-1/blob/master/README.md) - A description of the project goals requirements and limitations.


---

## Overview

The API that I chose to work with was the [Open Weather API](https://openweathermap.org/api) which provides information about current and past weater conditions. I used the requests library to pull data from their API on several thousand U.S. cities in order to get an idea of the relationship between temperature and humidity. 

---

## My goals for this project

By gathering this data using an API and the python requests library I hoped to get a better understanding of how API's function, and how to use them. I also hoped to determine how temperature and humidity are related by calculating the correlation coefficient.

---

## Motivation and Background

I chose to use the Open Weather API as I have worked with it in the past to create an apple app which informs the user of the weather in their city. I have hear anecdotes that a wet heat is worse than a dry heat, but I wondered weather there was any relationship between humidity and temperature. [This](https://trustyjoe.com/how-does-humidity-affect-temperature-in-your-house/) article explains that hotter air can hold more water which would indicate that hotter temperatures should be more humid than colder ones. 


## Limitations


* The data was collected all during one 30 minute period, this means that there could be a difference due to one city being measured 30 minutes later than another.
* Another issue is that the cities being measured are in different timezones so they are being measured at different times of day which could impact the results
* Finally we are only looking at a snapshot of data from one day in October. it is possible that if this experiment were repeated on a different day we could get different results.
* The final data set contains 2 columns and 1344 rows

---

## Basic Info of the Report

* The final data set contains 2 columns and 1344 rows
* The API required a free account and provied an API key
* There was a limit of 60 pulls in one minute, to address this I added a wait function in my code to pause the script for one second between pulls.

---

## Requirements

The software used in this analysis included:

1) Python
2) Pandas package for python
3) requests package for python

---
