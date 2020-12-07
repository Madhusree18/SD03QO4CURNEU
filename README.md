# SD03QO4CURNEU
### Social networks ad
The datasets describe of which users purchased or not purchased for the particular product.
In a decision tree, split points are chosen by finding the attribute and the value of that attribute that results in the lowest cost.
For classification problems, this cost function is often the Gini index, that calculates the purity of the groups of data created by the split point. A Gini index of 0 is perfect purity where class values are perfectly separated into two groups, in the case of a two-class classification problem.
Finding the best split point in a decision tree involves evaluating the cost of each value in the training dataset for each input variable.
For bagging and random forest, this procedure is executed upon a sample of the training dataset, made with replacement. Sampling with replacement means that the same row may be chosen and added to the sample more than once.
k-fold cross validation is used to estimate the performance of the learned model on unseen data. This means that we will construct and evaluate k models and estimate the performance as the mean model error. Classification accuracy will be used to evaluate each model.
mplementation of the Classification and Regression Trees (CART) algorithm adapted for bagging including the helper functions test_split() to split a dataset into groups, gini_index() to evaluate a split point, our modified get_split() function discussed in the previous step, to_terminal(), split() and build_tree() used to create a single decision tree, predict() to make a prediction with a decision tree, subsample() to make a subsample of the training dataset and bagging_predict() to make a prediction with a list of decision trees.
A new function name random_forest() is developed that first creates a list of decision trees from subsamples of the training dataset and then uses them to make predictions.
Deep trees were constructed with a max depth of 10 and a minimum number of training rows at each node of 1. Samples of the training dataset were created with the same size as the original dataset, which is a default expectation for the Random Forest algorithm.

### Malaria prediction
The datasets describes to explore whether the number of deaths , deaths CFR .. of malaria increases every year.
Feature engineering process is done where label encoder is used to convert the "country" and "WHO region" features from categorical to numerical.
log transform and box cox features have been added to the reported dataframe.
For model prediction ,Multilayer Perceptron used  with 3 hidden layers, 3 dropouts which have a dropout rate of 0.325 and an output activation of sigmoid. The loss is a binary cross entropy and the optimizer is an Adam which has a learning rate of 0.0001 and an epsilon of 2e-06.
