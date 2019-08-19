# MSDS Practicum II: Text Analytics on Drug Reviews
In partial fulfillment of the requirements for the degree of Master of Science in Data Science the following project is to use natural language processing (NLP) to perform sentiment analysis and classification on two different datasets containing patient reviews of drugs. The purpose of this type of review would be twofold. One benefit would be to eventually enhance reviews of drugs after they have been put to the market to better understand side effects and benefits. Another outcome from this type of analysis could be to help patients and doctors choose the best type of drug for their needs.

## Purpose of Study 
FILL IN HERE

## Datasets
There are two different sources of drug reviews. One comes from the website Drugs.com and contains over 200,000 reviews. Each review entry has the text of the review along with the user rating on a scale of 1-10, the drug name, the condition the drug was used to treat, date the review occurred, and a usefullness score where others can vote on whether the comments were helpful. The other dataset is much smaller with just over 4,000 total reviews coming from Drugslib.com. These reviews have three different types of text comments, one for benefits, one for side effects and one for overall experience. As with the Drugs.com dataset, this dataset has a user rating column with scores between 1-10. However, Drugslib.com does not include the usefullness or date columns, but have variables for effectiveness and a severity of side effects. 

Both sources are pre-split by the authors into training (75%) and testing (25%) sets that have fairly uniform distributions of ratings in comparison to each other. The datasets are not uploaded in this repository because they are freely available at the UCI Machine Learning Archive with the approriate citations. 
- [Drugslib.com](https://archive.ics.uci.edu/ml/datasets/Drug+Review+Dataset+%28Druglib.com%29)
- [Drugs.com](https://archive.ics.uci.edu/ml/datasets/Drug+Review+Dataset+%28Drugs.com%29)

## Data Science Task

The first step of the project was to perform pre-processing of the text so that it could be vectorized and turned into a feature set for classification purposes. Next, I performed exploratory data analysis to understand the similarities and differences between the test and training sets and also between the two different sources of drug reviews. Next, I built a supervised classification model using k-fold cross validation techniques to select the best feature set, model type and parameter optimization. With the model I made predictions across sources and across different subsets of conditions. I also compared these models to a standard sentiment analysis.

To perform all of the above analyses I used Python in Jupyter notebooks that are individually uploaded to this repository.
