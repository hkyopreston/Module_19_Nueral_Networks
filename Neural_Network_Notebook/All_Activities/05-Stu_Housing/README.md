# Housing Price Prediction

* In this activity, you will predict housing prices from the Ames Housing dataset using a neural network and deep learning model.

## Instructions

* Use the existing code to import the [AmesHousing.csv](../Resources/AmesHousing.csv) dataset and print out the datatypes for each column.

* Make a list of all columns with categorical data, and save their names to the `category_columns`. Caution! Some columns may be stored as numeric data types, but hold categorical information. For example, `MS SubClass` imports as `int64`, but contains categorical information. Use the metadata at [https://rdrr.io/cran/AmesHousing/man/ames_raw.html](https://rdrr.io/cran/AmesHousing/man/ames_raw.html) to determine which values should be treated as categorical variables.

* Make a list of all columns that contain numeric data, and save it to the `numeric_columns` variable.

* Create an `X` dataset by merging the dummy variables for the category columns with the numeric columns. Use the `get_dummies()` function from sci-kit learn.

* Fill in missing values in `X` with zeroes.

* Create a `y` series from `SalePrice`.

* Use `train_test_split()` to split `X` and `y` into training and testing sets.

* Scale `X_train` and `X_test` using `MinMaxScaler()`.

* Create a neural network model with twice as many neurons in the hidden layer as there are input neurons. Use `relu` for the activation function.

* Create an output neuron with a `linear` activation function.

* Check the model with `summary()`.

* Compile the model with the `adam` optimizer and `mean_squared_error` loss function.

* Train the model with 100 epochs. Note: you may need to convert your y values using `np.asarray()`.

* Get the R-squared score on the training and testing predictions using `r2_score()`.

* Create a deep learning model with two hidden layers, both with twice the number of neurons as the input layer. Use `relu` for the activation function.

* Train the model with 100 epochs. Get the R-squared score on the training and teting predictions. Compare to the neural network model.

# Bonus: compare the amount of time taken to train each model. Given the same amount of time to train the model, which model do you think would perform better?