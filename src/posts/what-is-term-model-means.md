---
title: What is the term "model" means? 0.1.0
description: Here I will try to understand what the term "model" means.
date: "2021-01-31"
tags: ["definition"]
---

Here the sentence: "Decision Trees are a type of model".

OK, seems true.

But what is a model?  
As I understand, model - is a function. And this function take data in and return something out.
But this function not "static", it is not just a piece of code or some mapping for values. It is a mathematical function that can be "trained". So it could improve over time by Machine Learning algorithms.

```python
model = DecisionTreeModel()
model.fit(training_data, results)
results = model.predict(test_data)
```

👆 it is just an example, where model is an object with several methods. But, as I understand, it makes for comfortable model usage in code.

Here is what Wikipedia writes about it:  
A mathematical model is **a description** of a system using mathematical concepts and language.
