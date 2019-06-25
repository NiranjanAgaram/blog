---
title: "Machine Learning Project Workflow"
date: 2019-02-02T08:08:50-04:00
excerpt_separator: "<!--more-->"
categories:
  - Machine Learning
tags:
  - project workflow
  - machine learning
  - data science
---

Given a data science / machine learning project, what steps should we follow? Here's how I would tackle it:

<!--more-->



<strong>Specify business objective:</strong> Are we trying to win more customers, achieve higher satisfaction, or gain more revenues?<br/>
<strong>Define problem:</strong> What is the specific gap in your ideal world and the real one that requires machine learning to fill? Ask questions that can be addressed using your data and predictive modeling (ML algorithms).<br/>
<strong>Create a common sense baseline:</strong> But before you resort to ML, set up a baseline to solve the problem as if you know zero data science. You may be amazed at how effective this baseline is. It can be as simple as recommending the top N popular items or other rule-based logic. This baseline can also server as a good benchmark for ML algorithms.<br/>
<strong>Review ML literatures:</strong> To avoid reinventing the wheel and get inspired on what techniques / algorithms are good at addressing the questions using our data.<br/>
<strong>Set up a single-number metric:</strong> What it means to be successful - high accuracy, lower error, or bigger AUC - and how do you measure it? The metric has to align with high-level goals, most often the success of your business. Set up a single-number against which all models are measured.<br/>
<strong>Do exploratory data analysis (EDA):</strong> Play with the data to get a general idea of data type, distribution, variable correlation, facets etc. This step would involve a lot of plotting.<br/>
<strong>Partition data:</strong> Validation set should be large enough to detect differences between the models you are training; test set should be large enough to indicate the overall performance of the final model; training set, needless to say, the larger the merrier.<br/>

<strong>Preprocess:</strong> This would include data integration, cleaning, transformation, reduction, discretization and more.<br/>
<strong>Engineer features:</strong> Coming up with features is difficult, time-consuming, requires expert knowledge. Applied machine learning is basically feature engineering. This step usually involves feature selection and creation, using domain knowledge. Can be minimal for deep learning projects.<br/>
<strong>Develop models:</strong> Choose which algorithm to use, what hyperparameters to tune, which architecture to use etc.<br/>
<strong>Ensemble:</strong> Ensemble can usually boost performance, depending on the correlations of the models/features. So it’s always a good idea to try out. But be open-minded about making tradeoff - some ensemble are too complex/slow to put into production.<br/>
<strong>Deploy model:</strong> Deploy models into production for inference.<br/>
<strong>Monitor model:</strong> Monitor model performance, and collect feedbacks.<br/>
<strong>Iterate:</strong> Iterate the previous steps. Data science tends to be an iterative process, with new and improved models being developed over time.
