# Cryptocurrencies
This project analyzes cryptocurrencies in order to find investable cryptocurrencies. The model design is aimed at finding a grouping logic to create a classification of the available cryptocurrencies.
## Methodology
Since the model is not designed to answer a specific question, the traditional statistical model methodologies are not applicable. A supervised machine learing methodology is ruled out for the same consideration. Since the model is free form and would be used to classify cryptocurrencies based on derived criteria unsupervised machine learning methodology is used to build the model.
## Data  Processing
the initial dataset contained 1252 cryptocurrencies, However, not all the datapoints were complete and the dataset needed to be processed to be suitable for unsupervised ML language.
#### Data Processing Steps
* Filter to keep onnly currencies that are trading.
* Drop the trading indicator column as that has no role in the groupng.
* Filter to keep the currencies that have a working algorithm.
* Drop incomplete data i.e drop any currency that contains a null value.
* Filter the dataset to keep only the currencies that have been mined.
* Copy the coin names and then drop the name column from the data set as the names shoud not contribute in clustering logic.
* Proxy the non-numric columns by numeric values so they can be used in clustering logic.
The next step is scale data to have mean 0 and standard deviation 1. 
### Analysis
After the input data is processed it could be used for ML models. </br>
First a PCA (Principal Component Analysis) is conducted retaining three factors. Then to find the optimal number of cluster groups an elbow curve is constructed. 
![image](https://user-images.githubusercontent.com/31217096/202909029-e762cf41-f8eb-4375-a43c-a25423cb9c5c.png)
The next step involves creating 4 groups as per pricipal component factors. The 3-D representation is following:
![image](https://user-images.githubusercontent.com/31217096/202909340-d16e089e-7a2a-406f-8fd5-3a3455efaf01.png)
At the final stage Total coins mined column is reintegrated and a scatter plot is built to compare total coins mined vs. total coins supply. This comparison would provide an idea regrading the demand and trading volume and also prospect of a crypto currency.
![image](https://user-images.githubusercontent.com/31217096/202909440-97857adf-f5f9-4ed7-a584-9f19a552e61f.png)

## Summary
The project did not aim to select any specific cryptocurrency for trading as that would depend on the ivestment funds and risk appetite.
The goal of the model was to provide an idea of features(although derived through PCA and not transparent and directly measurable) of the available currencies.



