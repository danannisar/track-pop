# Predicting Spotify Track's Popularity from Korean Music Groups <br>based on the Music Features and Group Profiles

## Introduction

Spotify as the global streaming platform distributed k-pop songs to all over the world. Kpop songs frequently charting and become popular stream in Spotify. Every year in Korea, many entertainment companies make debuts their produced k-pop groups. This analysis began for predicting k-pop track's popularity on Spotify with regression method. The track's popularity in Spotify is a range from 0 to 100, with 100 being the most popular. For independent variables we're using song/track's profile (musicality, duration, artists popularity, spotify followers) and k-pop group's profile (average age of members, days from debut, and company).

This analysis predict Spotify tracks popularity by applying Linear Model (with Ridge and Lasso Regularization) and Ensemble Model (Decision Tree, Bagging, and Random Forest). Linear Model was decided to be applied first because from exploratory process there are some linear correlations between dependent and independent variables. After modifying with Ridge and Lasso Regularization, there are not much differences in mean squared error. 

![Spotify](images/Spotify_Logo_CMYK_Green.png)

## Related Work
[Middlebrook and Sheik (2019)](https://arxiv.org/pdf/1908.08609.pdf) used Spotify Popularity Track data alongside with Billboard Charts data to classify which track would be a hit in Billboard. The data splitted into train-validation-test without cross validation process, then use four different models, Logistic Regression, Neural Network, SVM, and Random Forest for predicting. The result showed SVM and RF outperform the two other models. This analysis used one of ensemble model, Random Forest, which has been decided to use 8 maximum number of features, 80 estimators, and minimum split condition of two samples under Gini Criterion.

[Nujkamp, 2018](http://essay.utwente.nl/75422/1/NIJKAMP_BA_IBA.pdf) investigates the relationship between track popularity (stream count) and audio features in Spotify using linear regression approach. The analysis preceded by obtain correlation analysis between variables. By using step-wise method, only 9 relevant variables selected. This analysis found the relationship between streaming popularity and audio features in Spotify was weak. Its R^2 or explanatory power is 20.2% or the model explains 20.2% of the variation in stream count. The model concluded not effective to explaining stream count on its own. The other Spotify analysis is from [Ochi et al, 2021](https://arxiv.org/ftp/arxiv/papers/2108/2108.02370.pdf), with additional data about top songs by Country in Billboard chart. The analysis concluded, most influential features are valence and tempo, songs with high value of valence and tempo has high probability of being a hit in music charts.

## Dataset and Features

This analysis is using two separate datasets, spotify data set and korean music groups dataset. After merging and preparation, the final data has 

These are the source links of Spotify and Korean music Data :
- [Spotify Dataset 1921-2020, 600k+ Tracks](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks)
- [Kpop Database](https://dbkpop.com/) (The data have been scraped, the scraping code can be seen in `scrape_data.ipynb`)

Dataset and Features

Metode

Experiment/Result/Discussion

Conclussion/Future Work


