For this homework, I worked with Masooma, Paula and Rayta. We also discussed it a bit with Willow during office hours. In terms of dealing with the missing data in the
dataset, I used the method of getting rid of all 11 columns containing missing data, Rayta got rid of the 7 columns with the most missing data, and then the rows with missing
data from the remaining dataset, while Masooma and Paula got rid of the 10 columns with the most missing data, and then just the rows containing missing data to account for
the 11th column with missing data. Compared to Paula, we had different AUC values in the ROC graph (0.82 in Paula’s vs. 0.88 in mine). Paula’s best parameters were
n_estimators=10, max_features=’auto’ and max_depth=10, with a best score of 0.71. Mine were n_estimators=100, max_features=’sqrt’ and max_depth=10, with a best score of 0.82.
It seems like overall, my model predicted at a slightly better rate than Paula’s.

This homework tasked us with using Random Forest and Gradient Boosted Tree models on the Higgs-Boson dataset to predict a categorical variable “Label” and a numerical variable
“Weight.” Then we had to determine the most important features in the dataset, and then determine the best hyperparameters to create the random forest model, and create an ROC
curve to visualize the accuracy of the model with the best parameters. The parameters considered were n_estimators (number of trees in the forest), max_depth (how many layers
each tree has) and max_features (the maximum number of features that are considered for splitting a node). In the beginning, we had to do data wrangling and determine the best
way to deal with the missing values in the dataset. We decided to deal with them in the two methods previously stated.

A difficult part of this task for me was honestly keeping track of all the different labels I had to use throughout this project. Some of the interpretations of the results
were also difficult. For example, I had some trouble interpreting the confusion matrix. I had to first figure out that there were only two possible labels in the Label column
of the Higgs-Boson dataset, making it a binary feature. Then I had to figure out which was being used as the “Positive” class and which was being used as the “Negative” class,
which I figured out by comparing the counts in the confusion matrix with the counts for each label in the original dataset.

Besides keeping track of the labels, I think that creating the Random Forest and Gradient Boosted Tree models were not difficult.

This homework gave me a better understanding of tree models and how to interpret the results from them. It also gave me a better understanding of the important hyperparameters
for tree models and how each one affects the model.
