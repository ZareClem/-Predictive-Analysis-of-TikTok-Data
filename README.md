# Predictive Analysis using Random Forest and GridSearchCV
The main objective is to develop a machine learning model capable of distinguishing whether a TikTok video contains a factual claim or expresses an opinion. A successful prediction model will enable TikTok to streamline the processing of user reports, prioritizing them more effectively by leveraging machine learning to predict a binary outcome variable.

The purpose of this model is to mitigate misinformation in videos on the TikTok platform.

The goal of this model is to predict whether a TikTok video presents a "claim" or an "opinion".

This project follows the PACE framework (Plan, Analyze, Construct, Execute) and is divided into three parts:

# Business Need and Modeling Objective
## Business Need:
TikTok aims to enhance its content moderation process to better handle the high volume of user reports regarding misinformation. By efficiently identifying whether videos contain factual claims or personal opinions, TikTok can prioritize reports that potentially involve misleading information, thereby reducing the backlog and improving the platform's reliability and user trust.

Analysis indicates that authors who violate the terms of service are significantly more likely to be presenting a claim rather than an opinion. Therefore, it is crucial to distinguish between videos that make claims and those that offer opinions.

TikTok aims to develop a machine learning model to identify claims and opinions in videos. Videos identified as opinions will be less likely to be reviewed by human moderators. In contrast, videos classified as claims will undergo a further sorting process to determine their review priority. For instance, claim-classified videos might be ranked based on the number of reports they receive, with the top percentage being reviewed by human moderators each day.

## Modeling Objective:
The objective is to develop a machine learning model that predicts whether a TikTok video contains a "claim" or an "opinion." This binary classification model will leverage advanced machine learning techniques, such as GridSearchCV and Random Forest, to ensure high accuracy and reliability. The ultimate goal is to integrate this model into TikTok's moderation workflow, allowing for automated, real-time content assessment and more effective allocation of moderation resources.

## Modeling Workflow and Model Selection Process
Previous work with this data set, consisting of approximately 20,000 videos, indicates that it is sufficient for conducting a rigorous model validation workflow. The workflow involves the following steps:

Split the data into training, validation, and test sets (60/20/20).
Fit models and tune hyperparameters using the training set.
Perform final model selection using the validation set.
Assess the performance of the best model on the test set.

## Select an appropriate evaluation metric.
False positives: The model predicts a video is a claim when it is actually an opinion.

False negatives: The model predicts a video is an opinion when it is actually a claim.

The full explanation of code is available [here](https://github.com/ZareClem/-Predictive-Analysis-of-TikTok-Data/blob/main/tiktok-data-predictive-analysis-gridsearchcv.ipynb)
