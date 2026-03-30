##### Assignment 1 README

#### AI disclosure:
Some of the code was helped changed with ChatGPT, all code was reviewed and all comments, analysis, and interpretations were done on my own

## Purpose of the Analysis
The purpose of this project is to reproduce the analytical workflow from Lecture 01 R code into Python. 
The workflow includes loading the COMPAS dataset, cleaning and processing the data, performing exploratory data analysis (EDA), fitting a logistic regression model, and evaluating the model using confusion matrices and fairness-related error metrics across racial groups.
A key focus in the COMPAS dataset is to investigate whether there are differences in COMPAS scores and prediction errors across racial groups. This is important in understanding fairness and decision making in high-stakes scenarios like in the criminal justice system. 

## Python libraries Used
I used the followig python libraries for this project:
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- sklearn

## Instructions for Reproducing Results
1. Open the Jupyter Notebook file in Google Colab, Jupyter Notebook, or whatever notebook is compatible with python code.
2. Run the cells from top to bottom in order.
3. The notebook reads the COMPAS dataset directly from the ProPublica GitHub url source, so no separate dataset or csv download is required.
4. The notebook will reproduce the full workflow, including:
   - data and library installments
   - preprocessing and filtering
   - descriptive stats and visualizations
   - logistic regression modeling
   - confusion matrix evaluation
   - fairness analysis by race

##### Assignment 2 README

#### AI disclosure:
Some of the code was assisted by ChatGPT, but all code was reviewed and all comments, analysis, and interpretations were completed independently.

## Purpose of the Analysis
The purpose of this project is to build and analyze a COMPAS replacement model using Python.  
The workflow includes preprocessing the data, fitting machine learning models, and evaluating model performance using fairness-related metrics across racial groups.

A key focus of this analysis is to understand how the model makes predictions and whether there are differences in outcomes across groups. To do this, the project uses interpretability methods such as LIME, SHAP, and DiCE to explain predictions at both the global and individual level. This is important for evaluating fairness in high-stakes settings like the criminal justice system.

## Python Libraries Used
I used the following Python libraries for this project:
- pandas  
- numpy  
- matplotlib  
- scikit-learn  
- lime  
- shap  
- dice-ml  

## Instructions for Reproducing Results

1. Open the Jupyter Notebook file in Google Colab, Jupyter Notebook, or another compatible environment.

2. Install required libraries if needed. Some may need !pip installments which just require removing the # in the code before the line.
   
3. Run all cells from top to bottom in order.

4. The notebook will reproduce the full workflow, including:
- data preprocessing and feature engineering  
- model training (logistic regression and gradient boosting)  
- evaluation using confusion matrices and fairness metrics (FPR, FNR, AUC)  
- LIME explanations for individual predictions  
- SHAP summary and waterfall plots  
- DiCE counterfactual analysis  

5. Review the outputs and written interpretations within the notebook for final results and conclusions.
6. Write a governance memo by addressing a hypothetical court auditor summarizing the results of the models, limitations, and additional monitoring recommendations.
