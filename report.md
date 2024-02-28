# Homework 2 Report

## Basics
External resources used on this assignment:
* Stack overflow for syntax questions

Classmates you talked to about this assignment:
*

How many hours did you spend on this assignment?
Around 5 hours

### Group Member #1 Chloe Katz
* Your middlebury email: ctkatz@middlebury.edu
* How many hours did you spend on outside of class on CS 457 this week, _excluding this assignment_?
4 hours

### Group Member #2 Carly Mcadam
_Delete this section if you worked alone_
* Your middlebury email: cmcadam@middlebury.edu
* How many hours did you spend on outside of class on CS 457 this week, _excluding this assignment_?
2 hours
## Report
### Evaluating evaluation metrics
#### What is one advantage of using accuracy over a confusion matrix to evaluate your model?

Accuracy gives us a single targeted number which is the percent correctly predicted over the total, so it gives a specific number for a broad overview.

#### What is one advantage of using a confusion matrix over accuracy to evaluate your model?

A confusion matrix will be more specific and will paint a better picture of what languages were correctly and incorrectly predicted, and how those were examined.


#### Interpreting your confusion matrix
_Choose a language from the data set. Given any knowledge that you have about properties about that language (e.g., writing system, language families), explain any unique properties of its row in the confusion matrix, including (a) performance compared to other languages, (b) languages that it is more likely to be predicted as than others, and (c) anything else you think is relevant._

![Screenshot 2024-02-27 at 5 16 12 PM](https://github.com/ctkatz/report2/assets/100157146/8754adcb-02ce-4ad2-a2e6-429740da2ecf)

Language: Italian
(a)  Italian is a romance language, and uses a latin alphabet, which is also used by a lot of the languages in the set of languages, so it has a high amount of mistakes compared to other languages.
(b) It is most likely to be predicted incorrectly to spanish, which makes sense because spanish is also a romance language and uses similar word and verb structure, so we aren't suprised about a lof of confusion here.
(c) I'm suprised it only made one mistake in french versus italian, which suprises me because french is also a romance language, so it shares similar sentence structure.
### Effects of priors
Update your code so that your prior is uniform, e.g., the probability for each of the 8 languages is $log\left(\frac{1}{8}\right)$. Then, answer the following questions.

![Screenshot 2024-02-27 at 8 02 38 PM](https://github.com/ctkatz/report2/assets/100157146/d97d602e-4ea4-4944-a8dd-8fb570ecab10)

#### How do your results change? Why?

The confusion table shows overall a greater spread of languages than the first one, but overall the matricies are very similar, which is suprising. We would expect that an uniformly even prior would predict more incorrect languages for langauges that appear less in the corpus.


#### Describe a situation in which you might _want_ to use a uniform prior.

A uniform prior would be useful when we think the testing data is evenly distributed. Using a uniform prior as well might cancel out biases in training data that don't exist in the test data. 
