---
author-meta:
- Kylie Burkett
- Allisa Hastie
bibliography:
- content/manual-references.json
date-meta: '2020-12-06'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Machine Learning: Solar Energy Output" />

  <meta name="citation_title" content="Machine Learning: Solar Energy Output" />

  <meta property="og:title" content="Machine Learning: Solar Energy Output" />

  <meta property="twitter:title" content="Machine Learning: Solar Energy Output" />

  <meta name="dc.date" content="2020-12-06" />

  <meta name="citation_publication_date" content="2020-12-06" />

  <meta name="dc.language" content="en-US" />

  <meta name="citation_language" content="en-US" />

  <meta name="dc.relation.ispartof" content="Manubot" />

  <meta name="dc.publisher" content="Manubot" />

  <meta name="citation_journal_title" content="Manubot" />

  <meta name="citation_technical_report_institution" content="Manubot" />

  <meta name="citation_author" content="Kylie Burkett" />

  <meta name="citation_author_institution" content="Department of Civil &amp; Environmental Engineering" />

  <meta name="citation_author_institution" content="University of Illinois at Urbana-Champaign" />

  <meta name="twitter:creator" content="@burkett_kylie" />

  <meta name="citation_author" content="Allisa Hastie" />

  <meta name="citation_author_institution" content="Department of Civil &amp; Environmental Engineering" />

  <meta name="citation_author_institution" content="University of Illinois at Urbana-Champaign" />

  <meta name="twitter:creator" content="@AllisaG_Hastie" />

  <link rel="canonical" href="https://Kylierb2.github.io/SolarEnergy/" />

  <meta property="og:url" content="https://Kylierb2.github.io/SolarEnergy/" />

  <meta property="twitter:url" content="https://Kylierb2.github.io/SolarEnergy/" />

  <meta name="citation_fulltext_html_url" content="https://Kylierb2.github.io/SolarEnergy/" />

  <meta name="citation_pdf_url" content="https://Kylierb2.github.io/SolarEnergy/manuscript.pdf" />

  <link rel="alternate" type="application/pdf" href="https://Kylierb2.github.io/SolarEnergy/manuscript.pdf" />

  <link rel="alternate" type="text/html" href="https://Kylierb2.github.io/SolarEnergy/v/ce33194a873ff28a7f7222ec3b7714479ef4435b/" />

  <meta name="manubot_html_url_versioned" content="https://Kylierb2.github.io/SolarEnergy/v/ce33194a873ff28a7f7222ec3b7714479ef4435b/" />

  <meta name="manubot_pdf_url_versioned" content="https://Kylierb2.github.io/SolarEnergy/v/ce33194a873ff28a7f7222ec3b7714479ef4435b/manuscript.pdf" />

  <meta property="og:type" content="article" />

  <meta property="twitter:card" content="summary_large_image" />

  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />

  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />

  <meta name="theme-color" content="#ad1457" />

  <!-- end Manubot generated metadata -->'
keywords:
- markdown
- publishing
- manubot
lang: en-US
manubot-clear-requests-cache: false
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
title: 'Machine Learning: Solar Energy Output'
...






<small><em>
This manuscript
([permalink](https://Kylierb2.github.io/SolarEnergy/v/ce33194a873ff28a7f7222ec3b7714479ef4435b/))
was automatically generated
from [Kylierb2/SolarEnergy@ce33194](https://github.com/Kylierb2/SolarEnergy/tree/ce33194a873ff28a7f7222ec3b7714479ef4435b)
on December 6, 2020.
</em></small>

## Authors



+ **Kylie Burkett**<br>
    · ![GitHub icon](images/github.svg){.inline_icon}
    [Kylierb2](https://github.com/Kylierb2)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [burkett_kylie](https://twitter.com/burkett_kylie)<br>
  <small>
     Department of Civil & Environmental Engineering; University of Illinois at Urbana-Champaign
  </small>

+ **Allisa Hastie**<br>
    · ![GitHub icon](images/github.svg){.inline_icon}
    [ahastie2](https://github.com/ahastie2)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [AllisaG_Hastie](https://twitter.com/AllisaG_Hastie)<br>
  <small>
     Department of Civil & Environmental Engineering; University of Illinois at Urbana-Champaign
  </small>



# 1. Abstract {.page_break_before}




# 1. Introduction {.page_break_before}
Solar generation is an up and coming alternative energy resource. On the campus of the University of Illinois at Urbana-Champaign researchers have created solar farms to try and reduce the University’s carbon dioxide emissions. Solar farm 1.0 is the first UIUC solar farm; it has been operational since December of 2015. It is 20.8 acres of land and produces around 7,200 megawatt-hours of electricity annually. Surprisingly, this is only about 2% of the total megawatt-hours the university requires annually. In order to produce more the university recently published its plans to start work on “Solar Farm 2.0”. Solar farm 2.0 will be around 54 acres and produce as much as 20 thousand megawatt-hours annually; approximately 6% of university demand annually. Solar generation is important to “balancing the grid” and the more one is able to predict this output the more efficient energy usage will be. Knowing when solar energy will “run out” is largely a part of being able to utilize the maximum amount of solar energy generation. The goal of this project is to use machine learning techniques learned in class and publicly available data in order to predict the daily energy output from the UIUC solar farms.


# 2. Literature Review 
In order to better understand the current research on predicting solar generation, a literature review was conducted.
## 2.1 Machine learning methods for solar radiation forecasting: A Review - Cyril Voyant Et Al.
The journal paper explores other journals that have conducted research on predicting solar generation. This mass review found that most people who are doing research on solar generation are using artificial neural networks in order to predict outputs. This method is effective, however, the authors found that regression tree methods are actually performing with better results. Using his information the model for this project will use both neural networks and regression trees to see how they perform against each other. 
## 2.2 Predicting Solar Generation from Weather Forecasts Using Machine Learning - Sharma, N.; Sharma, P.; Irwin, D.; and Shenoy, P
The next journal was a case study from a research group using national weather forecast data.  The biggest issue they found was uncontrollable variability in weather patterns. This is expected in this type of research because the weather is a natural phenomenon that one can only predict toa certain extent. This group exclusively used support vector machines to resample the datasets. Support vector machines take in a large amount of data and then resample them into different smaller datasets in order to easily compare and analyze them. The most interesting aspect of this research was the use of datasets although they did not correlate well with test data.  This is something that the group will keep in mind when making their own models.


# 3. Data Collection and Analysis
This section will discuss the different types of data the group collected, cleaning said data, and the analyses performed on the datasets.
## 3.1 Raw Data Collection
**3.1.1 Solar Data**
--> insert image here
**3.1.2 Daily Weather Observations**
--> insert image here
**3.1.3 Monthly Solar Radiation**
--> insert image here
## 3.2 Exploratory Analysis
This exploratory data analysis will compile weather and solar data into a single cohesive data frame and examine the data themselves to better understand the characteristics of the features and labels and better understand their relationship with each other. Towards these goals, we will use a variety of statistical methods and graphical and tabular representations to identify trends and relationships.
**3.2.1 Clean and compile weather data**
The weather data that was obtained was in a .txt format, which can be difficult to work with. In order to make this file a CSV to analyze with our other CSV files. First, the .txt file needed to be called into the kaggle workspace. Once we were able to read all the files in, we had to remove blank rows, metadata, and any column titles that were poorly formatted we renamed. Following these actions, we were able to take a closer look into the dataset. In order to properly match up columns, the “Unnamed: 0” column was renamed to date to fit in with our other dataset. Lastly, the dataset’s incomplete data frames were dropped, columns without proper names were renamed, and then the smaller data frames were compiled into a larger data frame and the index reset. This allowed us to see a cleaner view and understand what this dataset actually is portraying. Following this, it was clear that the weather and solar data should be combined in order to analyze and explore all aspects of the data.
**3.2.2 Clean and combine weather and soalr data**
In order to read these two CSV files, they needed to be merged on the date column. Upon further inspection, it was observed that some cells in the data frame had the character string “M” attached to the end of the number. This would construe data and our analysis so we removed the M with an empty character. Following this, the dropping of NaN cells had to be performed to make sure the dataset was as complete as possible. There were also columns that were in as an “object” type. This was converted to be a “float” type. Once the index was reset we were able to set up a dictionary of the average daily solar radiation for each month in champaign. This was the data gathers from the IL State Water Survey. One last final touch was to make sure we had no empty cells and that our data frame was organized by the date. Following these actions, we continued to the exploratory data analysis.
**3.2.3 Examine and visualize training data**
These measurements are all taken from historic weather observations, but when predicting solar output we will only be able to use features that we can predict a day ahead or use the previous day’s observed measurements to predict the next day's features. The goal of our examination is to view basic attributes of each column in the data frame, observe any seasonal changes, view the shape of each column distribution, and see what columns are most correlated. Once we find the most correlated we will compare those columns with the solar output.
*3.2.3.1 Observations*
From the basic statistics of the dataset, it was observed that there are large standard deviations for most columns. This is most likely due to the seasonal variation. 
--> Insert histograms here
From the observed histograms, one will notice the variance in distribution type. The most normally distributed histograms are wind direction (dir_wind) and minimum humidity (min_hum). The more logarithmic distributions are average wind (avg_wind), maximum humidity (max_hum), and total precipitation (tot_precip). One will also notice that certain distributions such as the soil temperature measurements favor extremes in their histograms.
Upon analysis of the correlation coefficients between each column in the dataset, it was observed that solar radiation is strongly correlated. This was expected, however, this cannot be predicted ahead of time. Additionally, there was a strong correlation between temperatures and the dew point, both commonly used to predict weather forecasts. Below in figure one will see the time series graphs for the most correlated variables.
--> insert time step graphs here
From the time-series graphs, one can observe the seasonal variability in the graphs. The seasonal trends are apparent, yet not perfect. There is still quite a bit of noise in these observations. The next thing to look at will be the scatter plots of the 4 most correlated features with solar output. Once this is completed a regression analysis will be run to see how each feature affects the variation in solar output.
--> insert correlation graphs here
The results of the linear regressions of these plots were quite interesting. It was observed that the average daily solar radiation in Champaign explains about 93% of the variation in solar output, maximum daily temperature explains 54%, minimum daily temperature explains 53%, average daily temperature explains 56%, and dew temperature explains 45%. Although these values are all around 50% the goal is to use all of them and increase the predictive value as a whole.
**3.2.4 Key take-aways**
The Illinois State Water Survey's estimate of daily solar output in Champaign is a very good predictor of solar output, daily temperature indicators and dew point are also good indicators of solar output and can be predicted ahead of time. These features will be useful in model development. Day-ahead predictions of radiation and evaporation are not easily obtainable, realistically it would be difficult to use these to develop day-ahead prediction of solar output.  Features that are commonly included in weather predictions (temperature and humidity) may be suitable predictors of solar output.  Correlation between solar output and minimum humidity is positive and a linear regression fits the data with an R-squared of 0.62. Maximum daily temperature is positively correlated with solar output and when a linear regression model is developed, that model accounts for approximately 33% of variation in the data. The correlation between average daily temperature and solar output is weaker but still positive. The model created for this project will utilize five features: radiation estimation (rad_est), average temperature (avg_temp), dew point (dew), minimum temperature (min_temp), and maximum temperature (max_temp). From the EDA these seem to be the most promising at achieving an accurate prediction model.


## Model Development


## Conclusion
# This is a test
to see how the font looks

How do paragraphs look?
practice table

| Model Type | RMSE | MAE | R-squared |
| :---: | :---: | :---: | :---: |
| Neural Network | 1486 | 1557 | 0.93 |
| Random Forest | 824 | 634 | 0.97 |
| Persistence Model | 184 | 135 | 0.99|


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
