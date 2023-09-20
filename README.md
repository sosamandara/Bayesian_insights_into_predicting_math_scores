# Bayesian_insights_into_predicting_math_scores

It appears that there may be some errors in the PDF document provided in the README file. These errors may be attributed to the fact that the original file was in HTML format.
If possible take a look of the html file 'math_score'.

## Brief Introduction
The major objective of this project is to construct a regression model that makes use of Bayesian inference to forecast results in mathematics depending on available factors. Understanding the variables that affect arithmetic performance can give educators and decision-makers new perspectives on how to raise student achievement

Why this study can be helpful:

- Math score predictions can offer insightful information about a student’s academic achievement, according to the *Academic achievement Assessment*. It enables teachers to recognise kids who might require more assistance or resources in mathematics and to design interventions accordingly.

- *Identifying Influential elements*: Examining the correlation between math test results and different demographic and academic variables can aid in determining which elements have the greatest influence on a student’s success. This knowledge can direct educational initiatives and policies aimed at enhancing math instruction.

## The data set

The dataset consists of the following variables:

- *Gender*: Categorical variable indicating the gender of the student.

- *Race/Ethnicity*: Categorical variable representing the race or ethnicity of the student.

- *Parental Level of Education*: Categorical variable indicating the highest level of education attained by the student’s parents.

- *Lunch*: Categorical variable indicating whether the student receives free/reduced lunch or standard lunch.

- *Test Preparation Course*: Categorical variable indicating whether the student completed a test preparation course.

- *Reading Score*: Numerical variable representing the score obtained by the student in the reading subject.

- *Writing Score*: Numerical variable representing the score obtained by the student in the writing subject.

- *Math Score*: Numerical variable representing the target variable, the score obtained by the student in the math subject.

Some plots for the Exploratory Data Analysis
|       |       | 
:-------------------------:|:-------------------------: 
<img width="485" alt="plot1" src="https://private-user-images.githubusercontent.com/113529675/269402793-f56fd172-b217-4fd4-92b0-d7819d92e00e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTUyNDM3MzIsIm5iZiI6MTY5NTI0MzQzMiwicGF0aCI6Ii8xMTM1Mjk2NzUvMjY5NDAyNzkzLWY1NmZkMTcyLWIyMTctNGZkNC05MmIwLWQ3ODE5ZDkyZTAwZS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMwOTIwJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMDkyMFQyMDU3MTJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT04OTI4MTBmYjJkZDVmZDA3NmYwZDcyNzlkODZhODg4NDRjMGZjZTFhNDk5MzczMWZjZDRkMDA0MDIzMmYzNmEzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.SshKMuEQ4VNxU4vQjl5wjDJ_2eeKAXneQc_P7QVsl9g"> | <img width="485" alt="plot2" src="https://github.com/sosamandara/Bayesian_insights_into_predicting_math_scores/issues/1#issuecomment-1728355763">

The scatter plots between the Math Score (target variable) and the Writing Score, as well as the Reading Score, clearly demonstrate a strong positive correlation. This correlation can be observed from the overall upward trend in the scatter plots, as well as the fitted regression lines that show a positive slope.

<img width="485" alt="plot3" src="https://github.com/sosamandara/Bayesian_insights_into_predicting_math_scores/issues/1#issuecomment-1728357215"> | <img width="485" alt="plot4" src="https://github.com/sosamandara/Bayesian_insights_into_predicting_math_scores/issues/1#issuecomment-1728358448">

See the `math_score.pdf` file for a deeper analysis.

## The models 

In the `math_score.rmd` file you can find the bayesian analysis (complete of convergence analysis of the MCMC).
By examining the relationship between the Math Score and the predictors, we can estimate the model coefficients and make predictions on the Math Score for new observations.

Traceplots and posterior distributions can be examined to determine the reliability of MCMC samples. These graphs offer useful details about the convergence and behaviour of the MCMC chain.

To ensure the accuracy of the posterior estimates, it was essential to evaluate the convergence of MCMC samples. The Geweke diagnostic, which compares the means of the early and late regions of the Markov chain, is one often used diagnostic technique, and we opted for that.

By calculating the auto-correlation at various lags, we were able to determine the level of independence between MCMC samples.

# Used technologies

![RStudio](https://img.shields.io/badge/RStudio-4285F4?style=for-the-badge&logo=rstudio&logoColor=white)
![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white)

