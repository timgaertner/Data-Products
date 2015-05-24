Train Your Model Application
===
author: Tim Gaertner
date: May 24 2015
transition: rotate

Selecting Training Population
===
transition: linear
- An important task in any supervised modeling exercise is selecting data to train a model

- The common question for this task is what proportion of the available data should a modeler use to train their model?

- That's where the "Train Your Model" Application comes in to play

- The "Train Your Model" App allows a predictive modeler to efficiently test out training proporitons to see what portion of the data yields the highest accuracy on the test data

How does it work?
===
transition: linear

- Example: iris data with .5 proportion of the data used for model building

Confusion Matrix Results:

```
              (actual) setosa veriscolor virginica
(pred) setosa              25          0         0
veriscolor                  0         23         2
virginica                   0          3        22
```

Model Accuracy on Test data:

```
[1] 0.933
```


How does it work? Cont...
===
transition: linear
What if we increased the proportion of the data used for model building to .6 instead?

Confusion Matrix Results:

```
              (actual) setosa veriscolor virginica
(pred) setosa              20          0         0
veriscolor                  0         20         0
virginica                   0          1        19
```


Model Accuracy on Test data:

```
[1] 0.983
```

- The result is an increase in model accuracy. The modeler might conclude that including more data in the training partition better describes the target classes and it would be wise to allow for a higher training proportion.


Appendix
===
transition: linear
[Take "Train Your Model" for a Spin](https://timgaertner.shinyapps.io/TrainYourModel)
