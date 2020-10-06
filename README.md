# David House Homework 2 due 10/8/2020

## How to Navigate this Project

---

* **Code** - Folder for Jupyter notebooks.
    * [Cleaning.ipynb](https://github.com/DavidBrynnHouse/Data_601_HW-2/blob/master/Code/Cleaning.ipynb) - Jupyter notebook used to pull data from API and save as csv.
    *  [Executive Analysis.ipynb](https://github.com/DavidBrynnHouse/Data_601_HW-2/blob/master/Code/Executive%20Analysis.ipynb) - Jupyter notebook containing the main analysis for this project.
* **Data** - List used to collect specific data and data pulled from api
    * [temp_humidity.csv](https://github.com/DavidBrynnHouse/Data_601_HW-2/blob/master/Data/temp_humidity.csv) - csv file with with float values of temperature and humidity data taken from several thousand U.S cities at 7pm October 5, 2020
    * [us_cities.csv](https://github.com/DavidBrynnHouse/Data_601_HW-2/blob/master/Data/us_cities.csv) - A list of several thousand U.S Cities pulled from [this](https://www.britannica.com/topic/list-of-cities-and-towns-in-the-United-States-2023068) site.
* [LICENSE](https://github.com/DavidBrynnHouse/Data_601_HW-1/blob/master/LICENSE) - MIT License
* [README.md](https://github.com/DavidBrynnHouse/Data_601_HW-1/blob/master/README.md) - A description of the project goals requirements and limitations.



## My goals for this project

---

The data set that I chose to work with was the full text of Special Counsel Robert Mueller's Report on Russian Interference in the 2016 Presidential Election. I retrieved a CSV of this file from https://www.kaggle.com/paultimothymooney/mueller-report. My analysis was conducted to determine where investigators were focusing their attention. A large feature of the report is that much of it is redacted. For each redacted section a reason is given. I wanted to see what were the major reasons for redactions. Previous analysis of this document included looking at the word frequency of the document. I wanted to determine the number and type of sections that were redacted.

## Summary

The Special Counsel Rober Mullers Investigation into Russian Interference in the 2016 Presidential Election was a landmark report which has been analyzed by many who seek to understand the Trump 2016 presidential campaign and Russia's involvement. By obtaining the frequency of unique words in the document one can learn much about what the investigation involved and what its main focus was. Because much of the report was redacted there are still large segments that are unknown to the public. By observing what sort of information was withheld readers can better understand what may be missing from the report.


## Limitations and Basic Info of the Report

---

* The document is a conversion from pdf to CSV format. Because of this conversion, some words have been corrupted and therefore are uncountable. By visual inspection of the CSV however, I determined that it is not a significant amount of words that have been corrupted.
* The document has 19196 rows and 3 columns labeled page, line, and text. page and line are both integers while text contains strings


## Requirements

---

The software used in this analysis included:

1) Python
2) Pandas package for python
3) nltk package for python
