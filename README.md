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
* Convert the non-numric columns into numbers so they can be used in clustering logic.

