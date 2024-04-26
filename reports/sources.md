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
|000207972|4 |5 |3 |1 |12   |One point deducted for merging the report in late|
|000217597|5 |5 |4 |1 |13   |One point deducted for turning the report in late. One point deducted for turning in an extensionless file instead of the required .md|


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
|000207972|5 |4 |3 |4 |15   |One point deducted for merging the report in late|
|000217597|4 |4 |5 |4 |16   |One point deducted for merging the report in late|


## [Report 3](https://arxiv.org/pdf/1201.0220.pdf)

### Possible answers

1. What are the utility and application details of High Dimensional Sparse models for empirical estimation and inference in settings where there is a high-dimensional space of regressors?

2. Strengths and Weaknesses

    2.1. Strengths:

- The paper is highly rigorous with in proving it's claims regarding the convergence and efficiency thereof for the methods described

- The authors use simulations and empirical examples to illustrate the usefulness of the proposed methods and their performance as compared to other, more traditional methods

    2.2. Weaknesses

- The paper is quite technical and verbose in its notation.

3. Initially, the authors present a general model of a setting where there is a high amount of dimensions that can be related to a variable of interest, but only a small fraction of these dimensions are actually useful for estimation of the outcome with a small enough error; the identity of these useful dimensions it not known beforehand. To identify the useful dimensions and estimate the parameters associated with them, they propose several, equally useful, computationally feasible methods that rely on solving convex optimization problems whose criterion function relies linearly on an l-1 penalty term (Lasso), for whom the weight is calculated through several iterations of the Lasso procedure rather than by cross-validation. Their procedure integrates a final post-identification (post-Lasso) step which seeks to reduce bias due to the regularization found in the previous Lasso step. Both of them are capable of converging efficiently to optimal "oracle" estimation results. They illustrate these theoretical results with a Monte Carlo experiment, where they also find that the Lasso and Post-Lasso methods they propose perform better than the estimates with cross-validated penalty weights. They then show how to apply these procedures for treatment and structural effect inference. In these cases, the proposed procedures are capable of performing near optimal oracle estimations and also outperform other simpler methods. Finally, they show some empirical examples that show the usefulness of the proposed procedures for both selection of instruments in highly dimensional environemnts and for direct selection of control covariates.

4. Mainly, it would be interesting to see this approach applied to more empirical research, either for new estimations or for comparing and reassessing the results of previous estimations.

|Code     |Q1|Q2|Q3|Q4|Total|Notes|
|---------|--|--|--|--|-----|-----|
|000169027|  |  |  |  |   ||
|000199908|5 |5 |5 |5 |20   ||
|000216161|5 |3 |3 |1 |12   ||
|000216264|5 |5 |4 |5 |19   ||
|000225586|5 |5 |5 |4 |19   ||
|000231427|5 |4 |5 |5 |19   ||
|000234621|5 |5 |5 |5 |20   ||
|000242904|5 |3 |3 |5 |16   ||
|000242956|5 |4 |3 |4 |16   ||
|000250710|5 |4 |5 |5 |18   |Deducted one point for turning in a .txt file instead of the required .md|
|000199862|  |  |  |  |   ||
|000218002|  |  |  |  |   ||
|000230732|5 |5 |3 |4 |17   ||
|000231577|5 |3 |4 |5 |17   ||
|000242490|2 |3 |4 |4 |13   ||
|000250843|5 |5 |5 |5 |20   ||
|000259077|5 |4 |5 |5 |19   ||
|000220021|5 |5 |4 |3 |16   |Deducted one point for turning in a .docx file instead of .md|
|000220230|5 |3 |4 |3 |15   ||



## [Report 4](https://arxiv.org/pdf/2212.11366.pdf)

### Possible answers:

1. What are the current statistical considerations of estimation methods for Average Treatment Effects in Online Controlled Experiments, given the diversity of challenges they may face?

2. Strengths and Weaknesses:

    2.1. Strengths:

    - Thorough examination of the different methods best fit for different settings in  which an Online Controlled Experiment might be deployed. For each method, benefits and drawbacks are explained succinctly.

    - For each setting, relevant illustrative examples are presented, which helps contextualize the practical considerations behind the methods presented.

    2.2. Weaknesses

    - The exposition of each method is really brief, which might leave many questions open about their theoretical and practical details. However, the literature referenced contains the answers to the theoretical detail, as well as further elaboration about practical examples.

3. For a variety of settings, ranging from the simple application of ATE estimation through difference in averages, to the existence of long term differential effects and spillovers, the paper thoroughly lists the state of the art methods for ATE estimation in OCEs. For each method, a succinct explanation of theoretical and methodological features is provided.

4. Advancing the knowledge on the question could mean further exploring the methods that were left without as much explanation in the paper. For example, sampling techniques for OCEs that ensure optimal treatment assignment (like stratified sampling and bandit-problem approaches through Machine Learning) would aid complement the application of the inferencial methods in the main body of the text. Another path of research would be further explaining the practical examples of OCEs, explaining their strengths and drawbacks and how better inference would have been achieved.

### Grades

|Code     |Q1|Q2|Q3|Q4|Total|Notes|
|---------|--|--|--|--|-----|-----|
|000169027|5 |5 |4 |4 |18   ||
|000199862|  |  |  |  |     ||
|000199908|5 |5 |5 |4 |19   ||
|000207972|5 |4 |4 |5 |18   ||
|000216161|3 |3 |5 |1 |12   |Does not answer Q2 and Q4. Awarded two points in Q2 for thotoughly listing the methodologies, which is one of the strengths of the article and therefor indirectly answers the question|
|000216264|5 |5 |3 |5 |18   ||
|000217597|5 |5 |4 |5 |19   ||
|000218002|  |  |  |  |     ||
|000220021|5 |5 |4 |4 |17   |Deducted a point for turning in an extensionless file instead of the required .md|
|000225586|4 |4 |4 |4 |16   ||
|000230732|4 |5 |5 |5 |19   ||
|000231427|5 |4 |5 |5 |19   ||
|000231577|5 |4 |4 |4 |17   ||
|000234621|3 |4 |5 |5 |17   ||
|000242490|  |  |  |  |     ||
|000242904|5 |2 |2 |5 |14   ||
|000242956|5 |5 |3 |5 |18   ||
|000250710|5 |5 |4 |5 |18   |Deducted a point for turning in a .txt file instead of the required .md|
|000250843|5 |5 |5 |5 |20   ||
|000259077|  |  |  |  |     ||


## [Report 5:](https://netflixtechblog.com/orchestrating-data-ml-workflows-at-scale-with-netflix-maestro-aaa2b41b800c)

1. How does the newly developed Maestro contend against common challenges of scalability, reliability and usability for workflow orchestration?

2. Strengths and Weaknesses:

    2.1. Strengths:

    - Gives a high-level overview of the way Maestro fits withing a large scale infrastructure of data servicing where many workflows consisting of a very large amounts of steps must be set up and ran with the least amount of overhead.

    - Further goes into detail about the specific benefits of orchestration using maestro like workflow templates, integration of several different programming languages and formats, several various ways of integrating event/time scheduling of workflows.

    2.2. Weaknesses:

    - Explanations of the system and, its use and its components include technical jargon specific to the industry, so understanding the specifics might be slightly more complicated for academics and data scientists who wish to adopt similar systems but don´t have the background in software architecture necessary to easily understand the descriptions, even if they are high-level.

3. The document explains the motivation for developing Maestro for workflow orchestration, namely as a way to handle very large and complex data servicing structures that may encompass thousands of workflows, each consisting of steps, each of which may serve as an input, trigger, or parallel subworkflow of any other. It then details the different ways in which it can serve many users of diverse backgrounds and specializations for a variety of workflow-related tasks, like definition, scheduling, triggering, parametrization, among others.

4. It would be interesting to explore how Maestro can help in much smaller scales, like those of academia. Testing and benchmarking Maestro in comparison with other approaches in terms of overhead processing costs.


|Code     |Q1|Q2|Q3|Q4|Total|Notes|
|---------|--|--|--|--|-----|-----|
|000169027|  |  |  |  |     ||
|000199862|4 |4 |4 |5 |17   ||
|000199908|4 |5 |4 |5 |18   ||
|000207972|5 |5 |4 |4 |18   ||
|000216161|4 |3 |4 |4 |15   ||
|000216264|4 |5 |4 |5 |18   ||
|000217597|5 |5 |5 |5 |20   ||
|000218002|  |  |  |  |     ||
|000220021|4 |5 |4 |5 |18   |Deducted one point for turning in an extensionless file instead of the required .md|
|000225586|5 |5 |3 |4 |17   ||
|000230732|5 |5 |5 |5 |20   ||
|000231427|4 |5 |5 |5 |19   ||
|000231577|5 |4 |4 |5 |18   ||
|000234621|5 |5 |5 |4 |19   ||
|000242490|5 |5 |5 |5 |20   ||
|000242904|4 |3 |4 |3 |14   |Does not explicitly answer the questions. Awarded points in each question because correct answers are implied, although incompletely|
|000242956|4 |5 |4 |5 |18   ||
|000250710|5 |5 |5 |5 |20   ||
|000250843|5 |5 |5 |5 |20   ||
|000259077|5 |5 |5 |5 |20   ||


## Report 6

|Code     |Q1|Q2|Q3|Q4|Total|Notes|
|---------|--|--|--|--|-----|-----|
|000169027|  |  |  |  |     ||
|000199862|  |  |  |  |     ||
|000199908|  |  |  |  |     ||
|000207972|  |  |  |  |     ||
|000216161|  |  |  |  |     ||
|000216264|  |  |  |  |     ||
|000217597|  |  |  |  |     ||
|000218002|  |  |  |  |     ||
|000220021|  |  |  |  |     ||
|000225586|  |  |  |  |     ||
|000230732|  |  |  |  |     ||
|000231427|  |  |  |  |     ||
|000231577|  |  |  |  |     ||
|000234621|  |  |  |  |     ||
|000242490|  |  |  |  |     ||
|000242904|  |  |  |  |     ||
|000242956|  |  |  |  |     ||
|000250710|  |  |  |  |     ||
|000250843|  |  |  |  |     ||
|000259077|  |  |  |  |     ||

