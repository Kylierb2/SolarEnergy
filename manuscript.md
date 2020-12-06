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

  <link rel="alternate" type="text/html" href="https://Kylierb2.github.io/SolarEnergy/v/db69ed1df65f4594fd730c24b8f44961631de292/" />

  <meta name="manubot_html_url_versioned" content="https://Kylierb2.github.io/SolarEnergy/v/db69ed1df65f4594fd730c24b8f44961631de292/" />

  <meta name="manubot_pdf_url_versioned" content="https://Kylierb2.github.io/SolarEnergy/v/db69ed1df65f4594fd730c24b8f44961631de292/manuscript.pdf" />

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
([permalink](https://Kylierb2.github.io/SolarEnergy/v/db69ed1df65f4594fd730c24b8f44961631de292/))
was automatically generated
from [Kylierb2/SolarEnergy@db69ed1](https://github.com/Kylierb2/SolarEnergy/tree/db69ed1df65f4594fd730c24b8f44961631de292)
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


## Data Collection and Analysis


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
