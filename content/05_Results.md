# 5. Results 

![We can visually exmine the fit between our **neural network** prediction and the raw data over our entire training dataseet](https://github.com/Kylierb2/SolarEnergy/blob/master/content/images/neural_network_results.png){#fig:neural_results}

![We can visually exmine the fit between our **random forest** prediction and the raw data over our entire training dataseet](https://github.com/Kylierb2/SolarEnergy/blob/master/content/images/random_forest_results.png){#fig:forest_results}

In addition to comparing the results of our two models, we also use a persistence model to asses our models' performance. A persistence model is commonly used as a means of comparison when developing machine learning algorithms. In essence a persistence model assumes that the next time step will be the same as the current. For our purposes we developed a model that predicted that "tomorrow's" solar output will be equal to the solar energy measured "today". The persistence model performed better than our algorithms in all the metrics we used.

| Model Type | RMSE | MAE | R-squared |
| :---: | :---: | :---: | :---: |
| Neural Network | 1486 | 1557 | 0.93 |
| Random Forest | 824 | 634 | 0.97 |
| Persistence Model | 184 | 135 | 0.99|
