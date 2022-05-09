# Exoplanet-Exploration-with-ML

I am going to use several ML models to predict exoplanets. 

The column name explanations can be found here; https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html#pdisposition

I will use **sklearn** and **tensorflow**

I removed all "error" columns from the feature list.

I split the data into **train** and **test** datasets and scaled the data using **MinMaxScaler**, encode the data using **LabelEncoder** and converted encoded labels to one hot encoding using **to_categorical**.

I trained the data and made predictions on the test. 

I applied **Random Forest, KNN, Neural network** and **deep learning** to my dataset. 

I got very good result with Random Forest. 

I checked the importance of each **feature** and removed the bottom 4 that had little impact on the model. 

I *fine tuned* the model with trying several **grid parameters** and saw that it is not improving after 89%. 

For this data set the Random Forest model works very well. 

I further tuned the model by choosing the best features and doing **grid search** on it. 

Neural network and deep learning models are in NeuralNetworkModel and DeepLearning folders respectively.

To open the Neural Network and Deep learning models use ```keras.models.load_model(filepath)``` 

and you need to have ```from tensorflow import keras```


