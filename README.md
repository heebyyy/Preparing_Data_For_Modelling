# Preparing_Data_For_Modelling


This repo contains preparing numeric data to feed into machine learning. The techniques involved includes standadiztion and scaling. Another techniques used is normalization which involves converting feature vectors to unit norm.This can be the L1, L2 or themax norm. Certain machine learning algorithm require that the input data be linearly distributedor normally distributed. Dimensionality reduction using factor analysis fornumeric data is also explored 

Normalization is a row wise operation while standaddization is column wise operation. 

- Power transformer maps features from any distribution to be a close to Gussian distribution as possible, useful whenzero-mean, uunit variance normally distributed features are preferable

- Quantile transformer transform features tofollow a uniform or a normal distribution using quantile information, non-linear and might distort correlations andlinear relationships.

One of the data used is gotten from <a href=https://www.kaggle.com/uciml/pima-indians-diabetes-database target='_blan'>here</a>.

If your dataset contains a lot of outliers, the robust scaler is recommended for scaling the dataset

Normalizationis an importtant preprocessing techniques for Data that involve similairity calculation such as cosine similairty. 

Machine learning such as liear regression work well when the numeric features are normally distributed. Transformer are applied in other to convert data with different distribution to a form that is uniform or normally ditributed. The Quantile tranformer is used in this repository

This repository also contains working with outliers and novelties.

An outliers is a datapoint that differs significantly fromother dataset point in the samedataset.
A novelty is a data point encountered in prediction or testing that differs significantly from data points in training.
Algorithms used for determining outliers are unsupervised while algorithms used for novelties are semi-supervised
Three algorithmsare implemented in this study,they are the
- local outlier factor which uses nearest neighbor algorithm under the hood
- Elliptic envelope which tries to fit an ellipse around the dense point and
- Isolation forest which uses a randomforestof decision trees toidentify outliers

All these algoriths canbe used to identify novelties too