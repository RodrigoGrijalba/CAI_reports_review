### Questions: 
1. What is the research question of the article?
2. What are the strengths and weaknesses of the document's approach to answering that question? 
3. How does this paper advance knowledge about the question, i.e. what is the contribution?
4. What would be one or two valuable and specific next steps to advance this question?

## [Report 1](https://www.annualreviews.org/docserver/fulltext/economics/11/1/annurev-economics-080217-053433.pdf?expires=1713216498&id=id&accname=guest&checksum=609F0A2C6FDA057057538670762D1500):

### Model Answers:

1. How can econometricians diversify their toolset with ML Methods?

"In this review, we want to make the case that economists and econometricians also (...) 'need to move away from exlusive dependence on data models and adopt a more diverse set of tools.' We discuss some of the specific tools that empirical researchers should benefit from" (p. 686).

2. Strengths & weaknesses:

2.1. Strengths

- Makes an exhaustive list of current (at the time of writing the article) ML methods relevant to econometrics

- Explains the application of each method to different goals and settings for econometrics

2.2. Weaknesses

- Does not do a deep dive into the nuances of each method and how they can be modified for different econometric goals and data settings

- Lacks illustrative examples for the listed methods.

3. Exhaustively lists ML methods that economists and econometricians should be aware for a variety of settings.

4. For each of the listed methods and their corresponding applications, a deeper dive into the nuances, like data requirements, assymptotic characteristics of the estimators, tuning of algorithms in response to specific settings, etc, would be very useful resources. Another useful addition would be more illustrative examples for the use of the different methods.

### Grades

|Code     |Q1|Q2|Q3|Q4|Total|Notes|
|---------|--|--|--|--|-----|-----|
|000169027|5 |4 |4 |5 |18   ||
|000199908|5 |5 |5 |5 |20   ||
|000216161|4 |5 |4 |4 |17   ||
|000216264|4 |5 |5 |5 |19   ||
|000225586|4 |4 |4 |4 |16   ||
|000231427|3 |4 |5 |5 |17   ||
|000234621|3 |4 |5 |5 |17   ||
|000242904|5 |2 |5 |1 |13   |Does not explicitly answer Q2 and Q4. One point awarded in Q2 mentioning a disagreement with the paper, even if not fully developed|
|000242956|5 |5 |5 |4 |19   |
|000250710|5 |5 |5 |5 |19   |One point deducted for turning in a .txt file instead of .md|
|000199862|4 |3 |5 |3 |15   ||
|000218002|3 |2 |4 |1 |10   |Does not explicitly answer Q2 and Q4. One point awarded in Q2 for summarizing the listing of models|
|000230732|5 |3 |5 |4 |17   ||
|000231577|5 |3 |5 |3 |16   ||
|000242490|5 |5 |5 |5 |20   ||
|000250843|4 |5 |5 |3 |17   ||
|000259077|4 |5 |5 |5 |19   ||


## [Report 2](https://arxiv.org/pdf/1907.12665.pdf)

### Model Answers

1. What is an effective Machine Learning approach to predict pricing of Airbnb rental units based on their features.

2. Strengths and Weaknesses

2.1. Strengths

- It explores a variety of predictive models and compares their performance for the task at hand, finding the most capable one.

- It uses several approaches to pre-select relevant features for prediction in order to optimize computational load

- Makes use of sentiment analysis of reviews of the rental properties to add another dimension to the feature space

2.2. Weaknesses

- It leaves out some important and relevant approaches to prediction like Random Forests

- Some of the approaches for pre-selection of relevant features are arbitrary (e.g. picking 100 lowest p-values, hand-picking of features by authors)

- There are no explanations on the choice of hyperparamenters for each model. It is implied, by the existence of a validation subsample, that they are picked through cross-validation, but then this process is not mentioned. For example, for the K-means Clustering with Ridge Regression algorithm, it is not explained how they arrive at the optimal amount of centroids or the optimal penalization coefficient.

- Other approaches to cross-validation, like k-fold CV, might render better out-of-sample results. 

3. The authors test several predictive models through a variety of algorithms (Ridge Regression, Discontinuous Ridge Regression through K-means clustering, Neural Network, Vector Support Regression, and Gradient Boosting), all of which take features related to the rental properties in the Airbnb platform and output a prediction of their price. Before training the models, the authors split the sample such that the validation and testing sub-samples account for 5% of observations, and the training sample accounts for the rest. Then, they select the relevant features in three ways: hand-picking them, utilizing a LASSO regression with the best performing penalty factor as assessed by cross-fitting, by picking the features with the highest p-values after fitting an OLS regression. Through thesefeature selection methods, it was assessed that those selected with the LASSO proceedure were the mos relevant ones, and they would be used for training the models. Through thesefeature selection methods, it was assessed that those selected with the LASSO proceedure were the mos relevant ones, and they would be used for training the models. After training all the models and comparing their performances, the authors find that the best predictions were rendered with the SVR algorithm.

4. It would be interesting to try other models and feature selection schemes. Different cross-validation schemes might render better results, like k-fold CV. Finally, training the models in systems with higher computational capacity and with the full set of features may better showcase the effectiveness of the algorithms.

### Grades

|Code     |Q1|Q2|Q3|Q4|Total|Notes|
|---------|--|--|--|--|-----|-----|
|000169027|5 |5 |5 |4 |19   ||
|000199908|5 |5 |5 |5 |20   ||
|000216161|4 |3 |3 |3 |13   ||
|000216264|5 |5 |4 |5 |19   ||
|000225586|4 |4 |2 |3 |13   ||
|000231427|5 |5 |4 |4 |18   ||
|000234621|5 |5 |4 |5 |19   ||
|000242904|4 |4 |4 |4 |16   ||
|000242956|5 |4 |5 |5 |19   ||
|000250710|5 |5 |4 |5 |19   ||
|000199862|3 |3 |5 |4 |15   ||
|000218002|3 |3 |4 |4 |14   ||
|000230732|5 |5 |5 |5 |20   ||
|000231577|5 |4 |4 |4 |17   ||
|000242490|5 |4 |4 |5 |18   ||
|000250843|4 |4 |4 |5 |17   ||
|000259077|5 |4 |5 |5 |19   ||

## [Report 3](https://arxiv.org/pdf/1201.0220.pdf)


|Code     |Q1|Q2|Q3|Q4|Total|Notes|
|---------|--|--|--|--|-----|-----|
|000169027| | | | |   ||
|000199908| | | | |   ||
|000216161| | | | |   ||
|000216264| | | | |   ||
|000225586| | | | |   ||
|000231427| | | | |   ||
|000234621| | | | |   ||
|000242904| | | | |   ||
|000242956| | | | |   ||
|000250710| | | | |   ||
|000199862| | | | |   ||
|000218002| | | | |   ||
|000230732| | | | |   ||
|000231577| | | | |   ||
|000242490| | | | |   ||
|000250843| | | | |   ||
|000259077| | | | |   ||




## [Report 4](https://arxiv.org/pdf/2212.11366.pdf)


|Code     |Q1|Q2|Q3|Q4|Total|Notes|
|---------|--|--|--|--|-----|-----|
|000169027| | | | |   ||
|000199908| | | | |   ||
|000216161| | | | |   ||
|000216264| | | | |   ||
|000225586| | | | |   ||
|000231427| | | | |   ||
|000234621| | | | |   ||
|000242904| | | | |   ||
|000242956| | | | |   ||
|000250710| | | | |   ||
|000199862| | | | |   ||
|000218002| | | | |   ||
|000230732| | | | |   ||
|000231577| | | | |   ||
|000242490| | | | |   ||
|000250843| | | | |   ||
|000259077| | | | |   ||







