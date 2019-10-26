#### Which topic did you choose to apply the data science methodology to? #### 
Credit cards
- - - - 

#### Using the topic that you selected, complete the Business Understanding stage by coming up with a problem that you would like to solve and phrasing it in the form of a question that you will use data to answer. ####
One of the major challenges faced by companies is understanding who their customers are. Customer demographics can help their marketers understand the customer's needs, wants and behaviours, and ultimately what would make them buy something. Once customer needs are identified, it's easier to tailor their products and deliver what is really important to the buyers. But customer demographics requires data on customers. One avenue of getting this data is through credit card usage. So the question is "Can we determine user buying likelihood based on their credit card data?"
- - - -

#### Briefly explain how you would complete each of the following stages for the problem that you described in the Business Understanding stage, so that you are ultimately able to answer the question that you came up with:
1. Analytic Approach
2. Data Requirements
3. Data Collection
4. Data Understanding and Preparation
5. Modeling and Evaluation

#### Analytic Approach: ####
Our objective is to identify the appropriate customer segment likely to buy our products from their credit card usage. This would likely require identification of patterns that distinguish buyers from non-buyers. For this purpose, machine learning could be an appropriate approach in order to perform clustering of similar characteristics. The characteristics identified through the clustering can then be used for predictive modelling in order to be able to tell if a new customer is likely to buy our product.

#### Data Requirements: #####
Since one of our objectives is to identify characteristics associated with a buying pattern, we need data on both buying behavior as well as demographic characteristics. This means our dataset should include the entire credit card history associated with buys as well as demographic info such as age, sex, race, economic status etc. that could make up the characteristics. We'd also need the information to identify buyers and non-buyers.

#### Data Collection:
This phase would require the consolidation of the aforementioned datasets - from credit card history (date, time, transaction amount, product bought, monthly spending etc.) to demographic info (age, sex, race, economic status etc) with the personal identification info removed. In this stage, we will check for any additional information required and decide whether additional data collection is necessary or if it can be improvised. Examples of additional data for this problem could be satisfaction with products bought from the company, frequency of buying, brand loyalty etc.

#### Data Understanding and Preparation:
This stage would involve exploratory data analysis to check for correlations between all the variables we already have and removing highly correlated redundant variables from the dataset. Data visualisation tools such as histograms, barplots, x-y plots would come in handy during this phase. If there is missing information from the dataset, now would be the time to standardise what should be done about it - either remove all non-complete entries or substitute in dummy or computed values if it's a minor variable etc. This phase would also include feature engineering - creating new variables by manipulating raw variables (for example, computing monthly spending by summing up individual transactions) as well as preparatory processes such as principal component analysis in order to simplify the data into a usable format.

#### Modeling and Evaluation:
We will need to label all our data clearly and run it through a clustering algorithm that would identify patterns in the data. The output of this would form the basis for the predictive model. We will then separate our dataset into training data and testing data. The training data would be used to build the predictive model (for instance, multiple linear regression) to predict if the person would be a buyer. The model will then be evaluated for accuracy and satisfaction of assumptions (not overfitting etc). It can then be tested on the testing dataset to ensure its validity for out-of-sample data. If the accuracy is not up to par, we will go back to the data understanding stage to do more exploratory analysis and repeat the steps.
