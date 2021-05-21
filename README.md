![image](https://github.com/sgautam666/Brand_Sentiment_Analysis_with_NLP/blob/main/images/photo-1595287137144-cf60a87f39d9_unsplash_Chris%20J.%20Davis.jpg)

# Brand_Sentiment_Analysis_with_NLP

**Author**: [Suman Gautam](mailto:smngeo@gmail.com)

## Overview

Using LSTM and GRU network to perform sentiment classification from Twitter data


## Project Summary

X-Insight is an analytical company which provides analytical solutions to the major companies regarding there products, market analysis, sales analysis. Pine-Apple has hired X-insight to perform a large-scale market sentiment analysis on their products. 
In order to perform such analysis, X-insight is relying on Machine Learning to predict public sentiment from text data. For this purpose, X-insight is looking into twitter text data to predict if the given text has positive or negative sentiment towards a particular brand. More importantly, they want to test whether the project is feasible to invest more on large scale data collection and modelling. 


## Data

The datasets for this project is provided by [data.world](https://data.world/crowdflower/brands-and-product-emotions). The dataset includes twitter text related to Apple and Google products with user sentiment ranked between 'positive', 'negative', 'neutral', and 'no_idea' sentiments. Amongst these, the 'neutral' class occupies 60% of the class label whereas 'negative' class is about 6% of data resulting into a highly imbalanced class labels.

## Sentiment Classification 
Initial modeling effort showed that the our models suffers from the class imbalance. Therefore, few extra tweets with 'negative' class label were collected from different dataset (same source) and appended to the dataframe.
Tradition classification algorithms: Naive Bayes and Random Forest were tested as well as more sophisticated LSTM and GRU were tested. Traditional methods suffers from training overfit. The neural network improves on the overfit slightly but the accuracy is limited to 70%.

![image](https://github.com/sgautam666/Brand_Sentiment_Analysis_with_NLP/blob/main/images/text_predict.PNG)

## Future Improvements
The size of the training data is relatively very small to overcome the training over-fit. However, the neural LSTM and GRUs show promising results.It would be beneficial to test BERT and latest GPT-3 models in these data. But, prior to that, a significant amount of work needs to done in data collection with reduced class imbalance. 


## For More Information

See the full analysis in the [Jupyter Notebook](./final_model.ipynb) or review this [presentation](./Water_Pump_Failure_Prediction_notebook.pdf).



## Repository Structure

```
├── data
├── images
├── Tweeted text exploration.ipynb
├── Brand_Sentiment_Analysis_with_Final_Model.ipynb
├── Brand_Sentiment_Analysis_with_Final_Model.pdf
└── README.md
```