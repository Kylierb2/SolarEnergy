# 4. Model Development

In order to predict daily solar output, two different models will be used: neural network and random forest regression. In order to assess the accuracy of the model, a persistence model will be used for comparison. The means squared error, R-squared, and correlation will determine which model performs best.


## 4.1 Neural Network

```
x=training_data[["rad_est", "avg_temp", "dew", "min_temp", "max_temp"]]
y=np.ravel(training_data["Site Performance Estimate"])
scaler=MinMaxScaler()
x=scaler.fit_transform(x)

train_ds=tf.data.Dataset.from_tensor_slices((x, y)).batch(batch_size=150)
epochs=500

model=tf.keras.Sequential() 

model.add(tf.keras.layers.Dropout(0.2))

model.add(tf.keras.layers.Dense(units=128, input_shape=(5,)))

model.add(tf.keras.layers.Dense(units=256, activation="relu"))

model.add(tf.keras.layers.Dense(units=256, activation="relu"))

model.add(tf.keras.layers.Dense(1))

model.compile(optimizer=tf.keras.optimizers.Adam(learning_rate=0.01, decay=0.01/epochs), loss="mse" )


history=model.fit(train_ds.shuffle(10), epochs=epochs) 
```

This neural network will utilize five features from the training dataset: radiation estimation (rad_est), average temperature (avg_temp), dew point (dew), minimum temperature (min_temp), and maximum temperature (max_temp). The hidden layers of this network are made up of 256 nodes each and both use the Rectified Linear Unit activation (relu). This is a common activation function in neural networks because it avoids the vanishing gradient problem that may occur with other activations. We also include a dropout layer to avoid overfitting the training data. This dropout layer randomly sets node weights to 0 at a rate of 0.2 for each step in the learning process.

## Random Forest Regression

```
x = df_train[["rad_est", "avg_temp",  "dew", "min_temp", "max_temp"]]
y = np.ravel(df_train["Site Performance Estimate"])

scaler=MinMaxScaler()
x = scaler.fit_transform(x)


train_x, test_x, train_y, test_y = train_test_split(x, y, test_size =.2, random_state = 42)

regr = RandomForestRegressor(n_estimators = 5000, 
                             criterion= 'mse', 
                             max_depth=100, 
                             random_state=0,
                             min_samples_split = 2,
                             min_samples_leaf=1, 
                             max_features = 'auto',
                            bootstrap = True)

regr.fit(train_x, train_y)
```

The second model that was developed is the random forest regression model. This model is interesting because unlike a neural network it takes the datasets and creates multiple decision trees in order to find the best-fit prediction. Random forest models are less likely to overfit because of this. For this project, the same features will be used in order to compare the two models more accurately. These features are as follows: radiation estimation (rad_est), average temperature (avg_temp), dew point (dew), minimum temperature (min_temp), and maximum temperature (max_temp). An interesting hyperparameter that was used is the “bootstrap” function. Bootstrapping is a way of resampling. This model implemented bootstrap = True which will use subsets of the data to form decision trees. If bootstrap = false was utilized then the entire dataset would have been used to form trees. Interestingly, better results were obtained using “True” over “False” which is seldom the case in literature reviews.
