# Hands-On Machine Learning with R, 2nd Edition (In Progress)

[![Status](https://img.shields.io/badge/status-work%20in%20progress-orange.svg)](https://github.com/bradleyboehmke/homl_2e)
[![License](https://img.shields.io/badge/license-TBD-lightgrey.svg)](./LICENSE)
[![Website](https://img.shields.io/badge/book-read%20online-brightgreen.svg)](https://boehmke.github.io/homl_2e/)

This is the public repository for the in-development second edition of **Hands-On Machine Learning with R** by Brad Boehmke and Brandon Greenwell.

> **Note: This is a Work in Progress**
>
> This book is being actively written and revised. The content is subject to significant changes, chapters may be incomplete, and code examples may be updated. We welcome feedback, but please be aware of the project's developmental nature.

---

## About the Second Edition

The goal of this second edition is to create a thoroughly modern, practical, and long-lasting guide to machine learning in R. Building on the foundation of the first edition, this version introduces several key enhancements:

* **A Modern `tidymodels` Core:** The book is now built entirely on the `tidymodels` framework, providing a cohesive, modular, and modern approach to the entire modeling workflow.
* **Focus on the Full Lifecycle:** We go beyond just training models to cover the end-to-end machine learning process, from feature engineering to production deployment and monitoring.
* **New, Advanced Topics:** To prepare you for the challenges of modern data science, we've added entirely new chapters on:
    * **MLOps:** Deploying, monitoring, and managing models in production.
    * **Ethical & Responsible AI:** Understanding and auditing for bias, fairness, and transparency.
    * **Glass-Box Models:** Using powerful, inherently interpretable models like Explainable Boosting Machines (EBMs).
    * **Specialized Domains:** Applying ML to time series, text, and survival analysis problems.
* **Engaging Case Studies:** We've replaced older datasets with fresh, modern case studies that are woven throughout the book, allowing you to apply concepts as you learn them.

This book is being written openly and will be freely available online. A print version is planned for publication with **CRC Press (Chapman & Hall/CRC Data Science Series)** upon completion.

## How to Read the Book

The latest rendered version of the book is always available to read online, thanks to [Quarto](https://quarto.org/) and GitHub Pages:

**[https://boehmke.github.io/homl_2e/](https://boehmke.github.io/homl_2e/)**

## Using this Repository

This repository contains all the source code, data, and Quarto documents used to generate the book. We've designed it for maximum reproducibility.

### Reproducibility with `renv`

This project uses the `renv` package to ensure that you can use the exact same package versions that were used to write the book, guaranteeing that the code will always work as intended.

To get started:

1.  Clone or download this repository.
2.  Open the `homl_2e.Rproj` file in RStudio.
3.  Run `renv::restore()` in the console. This will install all required packages at their correct versions into a project-specific library.

## Feedback and Contributions

Your feedback is invaluable in helping us make this the best book possible. If you find typos, code errors, or have suggestions for clarification, please feel free to **[open a GitHub Issue](https://github.com/bradleyboehmke/homl_2e/issues)**.

At this time, we are not accepting direct pull requests for new content, but all suggestions in the Issues will be reviewed and considered.

## Authors

**Brad Boehmke** is a data scientist, educator, and author known for his work in making complex data science topics accessible.

**Brandon Greenwell** is a statistician and the author of several popular R packages for machine learning and model interpretability.

---

*The first edition of Hands-On Machine Learning with R can be found [here](https://www.routledge.com/Hands-On-Machine-Learning-with-R/Boehmke-Greenwell/p/book/9781138495685).*

---

## Table of Contents (WIP)

### Part I: Foundations of the Machine Learning Process
*Your toolkit for building robust and reproducible models.*

* **Chapter 1: The Machine Learning Landscape**
    * 1.1 What is Machine Learning?
    * 1.2 Supervised, Unsupervised, & Other Learning Types
    * 1.3 Why R for the Full Data Science Cycle?
    * 1.4 Our Approach: The End-to-End Workflow
    * 1.5 Introducing the Case Studies

* **Chapter 2: A Tidy Modeling Workflow**
    * 2.1 The `tidymodels` Philosophy
    * 2.2 Spending Your Data Wisely: Splitting with `rsample`
    * 2.3 Resampling for Robust Validation
    * 2.4 The Cardinal Rule: Avoiding Data Leakage
    * 2.5 Measuring Performance with `yardstick`
    * 2.6 Case Study Application: Setting a Baseline

* **Chapter 3: Feature & Target Engineering**
    * 3.1 The Power of a `recipe`
    * 3.2 Engineering the Target Variable
    * 3.3 Dealing with Missing Data
    * 3.4 Transforming Numeric Features: Skewness & Scale
    * 3.5 Encoding Categorical Features
    * 3.6 Case Study Application: Building a Preprocessing Pipeline

---

### Part II: Supervised Learning Algorithms
*From interpretable classics to flexible black boxes.*

* **Chapter 4: Linear Models**
    * 4.1 The Mechanics of Linear Regression
    * 4.2 Generalizing to Logistic Regression
    * 4.3 Implementation with `parsnip`
    * 4.4 Interpretation and Assumptions
    * 4.5 Case Study Application: Fitting a First Model

* **Chapter 5: Regularized Regression**
    * 5.1 The Problem with Many Features
    * 5.2 Ridge, Lasso, and the Elastic Net
    * 5.3 Tuning Regularization Penalties
    * 5.4 Using Regularization for Feature Selection
    * 5.5 Case Study Application: Improving the Linear Model

* **Chapter 6: Interpretable Glass-Box Models (NEW)**
    * 6.1 When Linear Isn't Enough
    * 6.2 Explainable Boosting Machines (EBMs)
    * 6.3 Rule-Based Models
    * 6.4 Bridging Ecosystems: Using Python Models in R with `reticulate`
    * 6.5 Case Study Application: Building a High-Performance Interpretable Model

* **Chapter 7: Non-Linear Classics: SVM & KNN**
    * 7.1 Support Vector Machines & The Kernel Trick
    * 7.2 K-Nearest Neighbors & Distance Metrics
    * 7.3 Tuning and Application
    * 7.4 Case Study Application: Trying Flexible Methods

* **Chapter 8: Tree-Based Methods: From Single Trees to Random Forests (CONDENSED)**
    * 8.1 The Anatomy of a Decision Tree
    * 8.2 The Ensemble Idea: Wisdom of the Crowd
    * 8.3 Bagging
    * 8.4 Random Forests
    * 8.5 Tuning and Interpretation
    * 8.6 Case Study Application: Harnessing the Power of Ensembles

* **Chapter 9: Gradient Boosting**
    * 9.1 Boosting: Learning from Mistakes
    * 9.2 How Gradient Descent Drives Performance
    * 9.3 Key Hyperparameters
    * 9.4 Implementations: XGBoost and LightGBM
    * 9.5 Case Study Application: Pushing for Maximum Performance

* **Chapter 10: Stacked Ensembles**
    * 10.1 Advanced Ensembling
    * 10.2 Building Base Models & Training a Meta-Learner
    * 10.3 Implementation with the `stacks` Package
    * 10.4 Case Study Application: Combining Our Best Models

* **Chapter 11: Neural Networks & Deep Learning (RENAMED)**
    * 11.1 From the Perceptron to Deep Architectures
    * 11.2 Building Networks with `keras`
    * 11.3 The Backpropagation Engine: Loss Functions & Optimizers
    * 11.4 A Disciplined Tuning Workflow: Regularization & Dropout
    * 11.5 A Glimpse into Modern NLP: Transformers & Large Language Models (LLMs) (NEW)

---

### Part III: Advanced Topics & Specializations
*Applying your skills to diverse data and complex problems.*

* **Chapter 12: Unsupervised Learning**
    * 12.1 Principal Component Analysis (PCA)
    * 12.2 Clustering: K-Means & Hierarchical
    * 12.3 Non-Linear Dimension Reduction: UMAP
    * 12.4 Anomaly Detection

* **Chapter 13: Post-Hoc Interpretability for Black-Box Models (REFRAMED)**
    * 13.1 Why We Need to Explain Black Boxes
    * 13.2 Global Interpretation: Permutation Importance & Partial Dependence Plots (PDP)
    * 13.3 Local Interpretation: LIME & SHAP
    * 13.4 Case Study Application: Explaining Our Best Black-Box Model

* **Chapter 14: Causal Inference with Machine Learning (NEW)**
    * 14.1 Beyond Prediction: Asking "What If?"
    * 14.2 The Potential Outcomes Framework
    * 14.3 Practical Application: Double Machine Learning

* **Chapter 15: Machine Learning with Text (NEW/EXPANDED)**
    * 15.1 Feature Engineering for Text with `textrecipes`
    * 15.2 Sentiment Analysis
    * 15.3 Topic Modeling
    * 15.4 Introduction to Word Embeddings

* **Chapter 16: Time Series Forecasting with ML (NEW/EXPANDED)**
    * 16.1 Framing Forecasting for Machine Learning
    * 16.2 Time-Based Feature Engineering
    * 16.3 Resampling for Time Series
    * 16.4 The `modeltime` Ecosystem

* **Chapter 17: Machine Learning with Censored Data: Survival Analysis (NEW)**
    * 17.1 The Challenge of Time-to-Event Data
    * 17.2 The Kaplan-Meier Curve & Cox Proportional Hazards Model
    * 17.3 Modern Approaches: Survival Forests & Boosted Survival Trees
    * 17.4 Evaluation Metrics for Survival Models
    * 17.5 Case Study Application: Predicting Customer Churn Over Time

---

### Part IV: From Model to Production
*Bringing your work to life, responsibly.*

* **Chapter 18: MLOps: Deploying and Monitoring Models (NEW)**
    * 18.1 The Full Model Lifecycle
    * 18.2 Reproducibility with `renv`
    * 18.3 The `vetiver` Framework for Model Deployment
    * 18.4 Creating a Model API with `plumber`
    * 18.5 Monitoring for Model Drift
    * 18.6 Case Study Application: Deploying Our Best Model

* **Chapter 19: Ethical & Responsible AI (NEW)**
    * 19.1 Bias, Fairness, and Accountability
    * 19.2 Sources of Bias in the ML Pipeline
    * 19.3 When Technical Debt Becomes Ethical Debt: The Impact of Data Leakage (NEW)
    * 19.4 Auditing Models for Fairness
    * 19.5 Case Study Application: Auditing Our Model for Bias

---

### Appendices

* **A: R and RStudio Setup**
* **B: A `tidymodels` Quick-Start Guide**
* **C: Bibliography**