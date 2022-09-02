# Hawaii-Airbnb-Price-Predication

 This paper will develop a model for price prediction
based on the features that hosts offer in Airbnb listings. The goal
is to help Airbnb hosts to set their prices more effectively and
understand the pricing market in Airbnb better with different
aspects. The algorithms that this paper will use are Linear
regression, Random Forest, and Neural Network. The metrics to
evaluate the performance of the models are MAE, RMSE, and Rsquared scores. 

## Dataset
[Data source: Inside airbnb](http://insideairbnb.com/get-the-data.html)

The dataset for this paper is multiple datasets in
months combined. I merged all the datasets between May 2020
to April 2021 to create a large dataset for Hawaii Airbnb
listings.

The dataset is split into two different ranges:

1. low-price range from $11 to $999 per night
2. high-price range, from $1,000 to $25,000 per night

## Data Preprocessing / Analysis
1. Remove unwanted symbols, fill or drop missing values, etc.
2. Extract Amenities and host_verifications into binary features: 
ex, has_pool, has_kitchen, etc. 
3. Drop unwanted price. The range for the price per night is from 0 to 94016. It does not make sense if the price is 0, and all the
price with a 0 is removed. The highest price is researched manually, and this price is found to be the wrong price tag. It is difficult to check which listing is wrong and which is not, especially when there are over 200k of data. All
the incorrect price tags are spotted manually and with some simple common sense. 
4. Data analysis, for detail, go to the [Hawaii Airbnb Price Prediction](https://github.com/selienamei/Hawaii-Airbnb-Price-Predication/blob/main/Hawaii%20Airbnb%20Price%20Prediction.pdf) paper.

## Result

Low-price: 

![Low-price results](https://github.com/selienamei/Hawaii-Airbnb-Price-Predication/blob/main/images/Capture3.JPG)

High-price:

![High-price results](https://github.com/selienamei/Hawaii-Airbnb-Price-Predication/blob/main/images/Capture4.JPG)

Full-dataset:

![All-price results](https://github.com/selienamei/Hawaii-Airbnb-Price-Predication/blob/main/images/Capture5.JPG)


