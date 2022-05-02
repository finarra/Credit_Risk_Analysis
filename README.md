# Credit Risk Analysis

## Overview
The purpose of this project is to apply supervised machine learning to estimate credit risk. 
This is a novel approach to a common problem, to identify credit card risk, a process which has been done for decades, through manual and time consuming labor, which results in long waiting for approval.
Nowadays FinTech institutions have shifted this paradigm towards an all digital and fast credit approval, so having an automated risk score that can come up with an answer almost instantly, is advantageous to any financial institution.

## Results
Since the number of high risk loans is vastly smaller than the safe loans, different methods had to be used, with different results, which will be summarized in the following list:

 - Random Oversampling:
	 - High risk: 
		 - Precision: 0.01
		 - Recall: 0.64
		 - F1: 0.02
	 - Low risk: 
		 - Precision: 1.00
		 - Rrecall: 0.66
		 - F1: 0.79
		 
 - SMOTE Oversampling:
	 - High risk: 
		 - Precision: 0.01
		 - Recall: 0.59
		 - F1: 0.02
	 - Low risk: 
		 - Precision: 1.00
		 - Recall: 0.67
		 - F1: 0.80
		
 - Undersampling:
	 - High risk:
		 - Precision: 0.01
		 - Recall: 0.57
		 - F1: 0.01
	 - Low risk:
		 - Precision: 1.00
		 - Recall: 0.46
		 - F1: 0.63
		 
 - SMOTEENN:
	 - High risk: 
		 - Precision: 0.01
		 - Recall: 0.67
		 - F1: 0.01
	 - Low risk:
		 - Precision: 0.01
		 - Recall: 0.55
		 - F1: 0.71
 - Balanced Random Forest Classifier:		 
	 - High risk:
		 - Precision: 0.04
		 - Recall: 0.71
		 - F1: 0.08
	 - Low risk: 
		 - Precision: 1.00
		 - Recall: 0.92
		 - F1: 0.96
 - Easy Ensemble AdaBoost Classifier:
	 - High risk:
		 - Precision: 0.08
		 - Recall: 0.91
	 - Low risk:
		 - Precision: 1.00
		 - Recall: 0.94
		 - F1: 0.97

## Summary
With this findings, I conclude that the best performance is the Easy Ensemble AdaBoost Classifier, as it has the best precision and recall for adequatelly identifying a low risk credit.

In this particular setting being able to identify the low risk credits is critical for a financial institution, since credit is their main source of income, and letting go low risk clients, turns away the profit to the competition.
