# Intro To Machine Learning

Introduction to machine learning with Python

`pipenv install`

`pipenv run jupyter notebook` -> start notebook in browser.

## General Terms

- `class`: names for different outputs
- `label`: class for a particular data point
- `generalization`: model is able to make accurate predictions on unseen data
- `Overfitting`: Building a model that is too complicated. Usually, one focuses too much
  on individual data points in the training set and does not generalize well.
- `Underfitting`: Building a model that is too simple

### Conventions

`f(X) = y`:

- `X`: Capital X, some data. Typically in math X refers to a 2D Array
- `y`: lower case Y -> Labels. Typically in math y refers to a vector (1D array)

## Supervised ML problems

When to use what? Rule of thumb is if there is a continuity between outputs use regression.

For algorithm refrence, check out chapter 2\*

```
An easy way to distinguish between classification and regression tasks is to ask
whether there is some kind of continuity in the output. If there is continuity between
possible outcomes, then the problem is a regression problem. Think about predicting
annual income. There is a clear continuity [sufficiently small changes in the input of a continuous function result in arbitrarily small changes in its output] in the output. Whether a person makes
$40,000 or $40,001 a year does not make a tangible difference, even though these are
different amounts of money; if our algorithm predicts $39,999 or $40,001 when it
should have predicted $40,000, we don’t mind that much.
By contrast, for the task of recognizing the language of a website (which is a classification
problem), there is no matter of degree. A website is in one language, or it is in
another. There is no continuity between languages, and there is no language that is
between English and French.
```

### Classification

Predict a _class label_ from a predifined list of classes. Binary classification (yes/no) which is often broken into positive and negative classes [not in the sense of value but in the sense of "is this the class im looking for"]

multiclass classification.

### Regression

Goal is to predict a number such as predicting income based on education/age/location.
