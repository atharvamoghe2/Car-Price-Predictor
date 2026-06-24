Link to Predictor:
https://huggingface.co/spaces/Atharva6767/Car-Price-Predictor

Link to dataset:
https://github.com/rajtilakls2510/car_price_predictor/blob/master/quikr_car.csv

Model Used: Linear Regression Model

Steps:
1: Data Cleaning (dropping missing values, removing commas, changing data type)

2. Model:
  a) Used sci kit learn for training and testing splits

  b) r2 score for determining model optimality
  
  c) one hot encoder for converting the categorical data into 1s and 0s
  
  d) making a column transformer to use OHE on select columns and letting others "passthrough"
  
  e) Letting the pipeline call the column transformer to make sure the columns are transformed and sending those to the LR model.
  
  f) Directly fitting the model on training data since everything is handeled by pipeline
  
  g) Dumping the pipeline on to our website 
