# Assignment 1 README

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

# Assignment 2 README

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

# Assignment 3 README

## AI Disclosure
AI in the form of ChatGPT was used to help debug errors that were occuring when writing code from lecture slides to my own script. All analysis, interpretations, etc. are done entirely on my own.

## Purpose of the Analysis
The purpose of thie project is to view disparte impact for COMPAS risk assessment model. The analysis focuses on identifying if the model produces unfair or unequal outcomes across protected groups, focusing on race and sex.


## Python Libraries Used
I used the following Python libraries for this project:
- pandas
- numpy
- matplotlib
- statsmodels
- sklearn
- solas-ai

## Instructions for Reproducing Results
1. Open the Jupyter Notebook file in Google Colab, Jupyter Notebook, or another compatible environment.

2. Install required libraries if needed. Some may need !pip installments which just require removing the # in the code before the line.

3. Run all cells from top to bottom in order.

4. The notebook will reproduce the full analysis, including:
- data cleaning and preprocessing
- creation of binary outcome (high risk)
- computation of AIR, ME, and SMD
- error-rate disparity analysis (FPR/FNR)
- statistical testing using two-proportion z-tests
- intersectional subgroup analysis (race × sex)
- fairness visualizations (bar charts)

5. Review the outputs and written interpretations within the notebook for final results and conclusions.
6. Write a compliance memo addressed to a hypothetical regulator summarizing findings, metrics used, and limitations.

# Assignment 4 README
## Purpose of the Analysis
The purpose of this project is to stress test the COMPAS prediction models built in previous lectures and evaluate whether they hold up beyond just performing well on a test set. The analysis covers five areas: distribution drift, generalization and overfitting, spurious correlations, robustness under stress, and slice-based fairness evaluation. A key focus is moving from just reporting metrics to actually reasoning about what they mean — specifically whether the models are reliable enough to be deployed responsibly in a high-stakes criminal justice setting.

## Python Libraries Used
I used the following Python libraries for this project:
- pandas
- numpy
- matplotlib
- scipy
- scikit-learn

## Instructions for Reproducing Results
1. Open the Jupyter Notebook file in Google Colab, Jupyter Notebook, or another compatible environment.
2. Run all cells from top to bottom in order.
3. The notebook reads the COMPAS dataset directly from the ProPublica GitHub URL, so no separate download is needed.
4. The notebook will reproduce the full audit workflow, including:
Part A: PSI and KS tests for numeric feature drift, MMD in encoded feature space, and train vs. test score distribution comparison
Part B: Train vs. test AUC, accuracy, and log loss with overfitting diagnosis using performance gaps
Part C: Counterfactual swap sensitivity for race, gender, and crime type
Part D: Stress testing priors_count with delta scenarios, ICE curves, and global sensitivity index
Part E: Slice-based evaluation by race, gender, and age with FPR, FNR, and AUC per group

5. Review the written interpretations after each section for analysis and conclusions.
