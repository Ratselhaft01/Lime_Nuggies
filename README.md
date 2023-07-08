# Lime_Nuggies
How to use model explainers

"In the beginning machines learned in darkness, and data scientists struggled in the void to explain them.
Let there be light." - https://pypi.org/project/interpret/

## Resources
* https://github.com/marcotcr/lime
* https://lime-ml.readthedocs.io/en/latest/
* https://www.geeksforgeeks.org/introduction-to-explainable-aixai-using-lime/
* https://www.ibm.com/watson/explainable-ai
* https://interpret.ml/docs/lime.html

## Why are Model Explainers Helpful?

//A brief explanation of what model explainers are, an overview of Lime, and how they can be used.

### Video Overview
* https://youtu.be/hUnRCxnydCc

"There are many advantages to understanding how or why an AI-enabled system has led to a specific output. Explainability can help developers ensure that the system is working as expected, it might be necessary to meet regulatory standards, or it might be important in allowing those affected by an decision to challenge or change that outcome. There can also be trade-offs or challenges involved in creating explainable AI: there may be a need to manage concerns about privacy, to consider access to intellectual property, or to put in place checks to ensure the explanations provided are reliable. " - https://royalsociety.org/topics-policy/projects/explainable-ai/

## Applying LIME

//A guide on how to apply LIME to their current models to understand what is happening.

## What Does This Info Mean?

Your Lime output should look something like this:

![Lime regression output example](images/LimeRegressionOutputEx.png)

When you call the `explain_instance` method, Lime creates a linear model for the specific instance of the data that you gave it and makes a prediction.

The intercept is the prediction the model Lime created would have made if the weights of all the features were zero. Prediction_local is the prediction that the model Lime created made. Right is the prediction that your actual model made.

Looking at the charts, that chart on the far right is the prediction that the model made. The chart in the middle displays each of the features and their weights, as well as whether those weights are positive or negative. The longer the bar, the larger the weight is, which indicates that the feature had greater importance when determining the predicted value. The chart on the far right displays each feature and their actual weights.

## Resources
* [Lime GitHub Repo](https://github.com/marcotcr/lime)
* [Lime Documentation](https://lime-ml.readthedocs.io/en/latest/)
* [Lime Tutorial (GeeksforGeeks)](https://www.geeksforgeeks.org/introduction-to-explainable-aixai-using-lime/)
