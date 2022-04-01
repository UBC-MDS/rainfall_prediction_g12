# Rainfall Prediction-group 12
## Overview
This is a group project for DSCI 525-Web and Cloud Computing, Master of Data Science, University of British Columnbia.
The project mainly focus on building and deploying ensemble machine learning models in the cloud, the dataset used in the project is the daily rainfall in Australia, which can be found [here](https://figshare.com/articles/dataset/Daily_rainfall_over_NSW_Australia/14096681). 
## Observations
Our observations can be found [here](https://github.com/UBC-MDS/rainfall_prediction_g12/blob/main/notebooks/rainfall_prediction.ipynb), including the runtime on different machine.

### Load csv and perform EDA on different machines
We tried two different approaches to reduce memory usage while performing EDA, they are:

- Loading in chunks

- Changing datatype

Both of the methods use less memory, note that we do not know which datatype consume the least memory in advance.

## Transfer dataframe from Python to R
Here we choose to use a parquet file to transfer the dataframe from Python to R for the following reasons:

- `Parquet` has already well implemented in `pandas`, we can perform the transformation by the function `to_parquet` directly.
-  `Parquet` files work well with rarrow. By default rarrow reads and processes data in chuncks, which will greatly improve the loading time. 

## Contributors
The following people contributed to the rainfall prediction project:
- VeraCui [@suuuuperNOVA](https://github.com/suuuuperNOVA)
- Jasmine Ortega [@JasmineOrtega](https://github.com/jasmineortega)
- Lynn Wu [@lynnwbl](https://github.com/lynnwbl)
- Maeve Shi [@MaeveShi](https://github.com/MaeveShi)

## License

This project is created by Vera Cui, Jasmine Ortega, Lynn Wu and Maeve Shi. It is licensed under the `MIT License`.