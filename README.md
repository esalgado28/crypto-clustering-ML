# unsupervised-ml-challenge
Eddy's folder for unsupervised learning homework
## Cryptocurrency Clusters
### Background
- You are on the Advisory Services Team of a financial consultancy. One of your clients, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. They’ve asked you to create a report that includes what cryptocurrencies are on the trading market and determine whether they can be grouped to create a classification system for this new investment.
- You have been handed raw data, so you will first need to process it to fit the machine learning models. Since there is no known classification system, you will need to use unsupervised learning. You will use several clustering algorithms to explore whether the cryptocurrencies can be grouped together with other similar cryptocurrencies. You will use data visualization to share your findings with the investment bank.
### Data Preparation
- Dataset was obtained from [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist) and is saved in `crypto_data.csv`
- Rows with null values were discarded as well as the first two columns which are not useful features for learning
- Only actively traded currencies were looked at
- Remaining categorical features were converted to numerical data and scaled
### Dimensionality Reduction
- PCA was used to reduce the number of features while retaining 90% explained variance
- Further reduction was done using t-SNE on the principal components
### Clustering
- K-means was used to identify clusters
- For this data, clustering does not seem possible
