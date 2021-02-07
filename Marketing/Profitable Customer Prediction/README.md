# Predicting-Profitable-Customers

### Context <br>
**Marketing is a key component of every modern business. Companies continuously re-invest large cuts of their profits for marketing purposes, trying to target groups of customers who have the potential to bring back the highest Return On Investment for the company. The cost of marketing can be very high though, meaning that the decision about which customer group to target is of great financial importance.**

**This dataset was made available by an online retail company that has collected historical data about such groups of customers, tracked the profitability of each individual group after the respective marketing campaign and retrospectively assessed whether investing on marketing spend for that group was a good choice.**

### Datastet Structure
Each row is a comparison between two groups of potential customers:
1) Column names starting with "g1" represent characteristics of the first customer group (these were known before the campaign was run) 2) Column names starting with "g2" represent characteristics of the second customer group (these were known before the campaign was run)
3) Column names starting with "c_" are features representing some comparison of the two groups (also known before the campaign was run)

The last column, named "target", is categorical, with 3 categories:<br>
0 - none of the two groups were profitable <br>
1 - group1 turned out to be more profitable <br>
2 - group2 turned out to be more profitable <br>

**Goal** Build a machine learning classifier that accurately predicts which of the 2 groups (if any) will turn out to be more profitable?

Result:
Based on my Analysis model would suggest to go for Customers in Group 1. Reason being:

1. Our Model Accuracy being 59% says about 59% of time it correctly labelled the customer in respective groups.
The precision of Model for Class1(0.63) > Class 0(0.36) & Class 2(0.57) which says among the labelled customers as Class 1. Model correctly predicts them as class 1 with score of 63% i.e 63 out of every 100 class 1 customers are correctly predicted.
2. In this scenario we want our assumptions to be more correct rather than false negatives and true negative( i.e we want to be more confident in our decisions so based on True Positive rates we can see 80% True Positive Scores.). Though it would also depend on customer behaviour and other demographic and social factors.
3. Also the Recall Score of Class 1 Group is better than other two group which says (False Positive better than False Negative).

Suggestion: Should perform A/B Testing.
