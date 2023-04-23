# Creating a Viral TikTok Video

This repository contains the code for the "Creating a Viral TikTok Video" project. The project uses a dataset of TikTok videos to identify the key factors that influence the popularity of a TikTok video.

### Dataset

The dataset used for this project is "Tiktok.csv". It contains information on various attributes of TikTok videos and their popularity scores.


### Tools and Technologies

The project is built in R language using RStudio. The following R packages have been used in this project:

- dplyr
- ggplot2
- xgboost
- AICcmodavg
- ROCR
- pROC

### Goals

- The main goals of this project are:

- To employ EDA, AIC and BIC to choose the best predictors and models for this dataset

- To employ regression models, ANOVA, PCA, clustering, logistic regression, SVM and XGBoost to find out which factors influence the popularity of a TikTok video the most.

- To evaluate the results of the above models using AUC ROC, F1 score, heatmap and a confusion matrix.

- To predict the likelihood that a Tiktok will be popular based on the variables of interest.

- To compare the results of these models with varying numbers of predictors to conclude the minimum number of predictors which are key to creating a popular TikTok video.


### Findings

The dependent variable popularity, when plotted as a histogram did not show any strong violation of the assumptions of normality, even though it did not have a perfect bell-shaped curve. Thus the models that we used in this project were appropriate. Although it was a continuous numerical variable, it looked more like an ordinal variable due to the values assigned to popularity as a metric. Hence fitting this data set with an ordinal regression model would do more justice to the data set. So we would consider fitting this data set using an ordinal regression model in future studies, and it would be interesting to see if the results of that model differ from the results presented in this project.

The F1 score and heatmap were used to compare the results of the SVM and XGBoost models. The SVM model had an F1 score of 0.78, while the XGBoost model had an F1 score of 0.83. The heatmap showed that the XGBoost model had a higher accuracy than the SVM model for predicting the popularity of a TikTok video.

From the results of the above models, we can conclude that a model with predictors playlist, loudness, energy, danceability, speechiness, decade, liveness, valence is the best model to predict the popularity of a TikTok. The results of this project indicate that an ordinal regression model would be appropriate for future studies to predict the popularity of a TikTok video. However, the XGBoost model using the predictors playlist, loudness, energy, danceability and liveness was found to be the best model for predicting the popularity of a TikTok video in this project. Thus, if one could get these 8 predictors correct - choosing a song from addictive playlist, keeping the loudness, energy, danceability, liveness and valence high, keeping the speechiness low and choosing a song from the correct decade, then they are sure to create a TikTok that will become popular.

### Files

``TikTok.Rmd`` : R Markdown file containing the code and results of the project.

``Tiktok.csv`` : Dataset used for the project.


### Conclusion

This project shows that it is possible to identify the key factors that influence the popularity of a TikTok video. By using appropriate regression models and evaluating the results using various metrics, we can predict the likelihood that a TikTok will become popular. The results of this project can be used by content creators to increase
