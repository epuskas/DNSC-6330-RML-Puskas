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
