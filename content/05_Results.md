# 5. Results 

In order to compare our models we developed two figures to observe. The first being a graph of our predicted results and the actual results. This graph displays the overlap of the data and how accurate our model was at predicting the correct values. 

*insert line graphs here*

As you can see the random forest regression produced a more accurate graph. The more defined line in blue is the actual results and the orange more noisy line is the prediction the model produced. For the most part, the two lines follow the same path, which is a good sign. The prediction doesn't do as well with the extreme values which are due to overfitting in the neural network. In the random tree regression the extreme values are a bit more accurate, but at the very tip are still off.
The next graph type we looked at was the correlation betwene our actual data and the model's predicted data.

*insert correlation graphs*


A truly correlated graph will be a tight exact line. Both of our models produced a linearly increasing line, which shows correlation. The graph for random forest is much more tight than the neural network, this is because our random forest regression is more accurate. 
Further inspection of the data allows us to compare the root means squared, mean absolute error, and the R-squared values for each model.

![We can visually exmine the fit between our **neural network** prediction and the raw data over our entire training dataseet](content/images/neural_network_results.png){#fig:neural_results}

![We can visually exmine the fit between our **random forest** prediction and the raw data over our entire training dataseet](content/images/neural_network_results.png){#fig:forest_results}


| Model Type | RMSE | MAE | R-squared |
| :---: | :---: | :---: | :---: |
| Neural Network | 1486 | 1557 | 0.93 |
| Random Forest | 824 | 634 | 0.97 |
| Persistence Model | 184 | 135 | 0.99|


As you can see in the table above the random forest regression out performs the neural network.  It is noted that the mean absolute error and root mean squared error are both lower than the neural network results. This is the first indication that the model is out performing the neural network. The R-squared value is quite impressive at 0.97. This means that the predicted values of the model explain about 97% of the variance. A high r-squared value indicates that the model values fit the actual values very well, a result one hopes for when predicting future values. Obviously, the more correlated the actual values are to the predicted values the more accurate the model is. However, one cannot only rely on correlation graphs because as seen in the neural network the correlation was still high even though the r-squared was 0.93. 
